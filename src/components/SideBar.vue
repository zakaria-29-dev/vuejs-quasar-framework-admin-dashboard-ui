<template>
    <nav>
        <q-header class="bg-grey-2 text-dark" bordered>
            <q-toolbar>
                <q-input borderless v-model="text" input-class="text-left" class="q-ml-md" label="Search shots..">
                    <template v-slot:prepend>
                        <q-icon name="search" />
                    </template>
                </q-input>
                <q-space></q-space>
                <q-separator vertical />
                <q-btn dense round flat icon="far fa-bell" class="q-mx-lg">
                    <q-badge color="green" floating transparent>4</q-badge>
                </q-btn>
                <q-separator vertical />
                <q-avatar class="q-ml-lg">
                    <img src="https://cdn.quasar.dev/img/avatar.png">
                </q-avatar>
                <q-btn color="dark" icon-right="fas fa-chevron-down" label="Jan Strassmann" flat />
            </q-toolbar>
        </q-header>
        <q-drawer v-model="leftDrawerOpen" show-if-above bordered>
            <div class="q-mt-md q-ml-md">
                <q-btn dense flat round icon="lens" size="8.5px" color="red" />
                <q-btn dense flat round icon="lens" size="8.5px" color="yellow" />
                <q-btn dense flat round icon="lens" size="8.5px" color="green" />
            </div>
            <q-list>
                <div class="text-center q-py-md">
                    <q-btn color="light-blue-8" icon="fas fa-cloud-upload-alt" label="Upload" class="q-px-lg"></q-btn>
                </div>
                <q-item clickable active-class="my-menu-link" v-ripple :active="link === 'My page'" @click="link = 'My page'">
                    <q-item-section avatar>
                        <q-icon name="fas fa-book" />
                    </q-item-section>
                    <q-item-section>
                        <q-item-label>My page</q-item-label>
                    </q-item-section>
                </q-item>
                <q-item clickable 
                active-class="my-menu-link"
                v-ripple
                :active="link === 'Dashboard'"
                @click="link = 'Dashboard'">
                
                <q-item-section avatar>
                    <q-icon name="fas fa-tachometer-alt" />
                </q-item-section>
                <q-item-section>
                    <q-item-label>Dashboard</q-item-label>
                </q-item-section>
                </q-item>
                <q-item clickable 
                active-class="my-menu-link"
                v-ripple
                :active="link === 'Edit Page'"
                @click="link = 'Edit Page'">
                
                <q-item-section avatar>
                    <q-icon name="fas fa-pencil-alt" />
                </q-item-section>
                <q-item-section>
                    <q-item-label>Edit Page</q-item-label>
                </q-item-section>
                </q-item>
                <q-item clickable 
                active-class="my-menu-link"
                v-ripple
                :active="link === 'Chat'"
                @click="link = 'Chat'">
                
                <q-item-section avatar>
                    <q-icon name="fas fa-comments" />
                </q-item-section>
                <q-item-section>
                    <q-item-label>Chat</q-item-label>
                </q-item-section>
                </q-item>
                <q-item clickable 
                active-class="my-menu-link"
                v-ripple
                :active="link === 'Community'"
                @click="link = 'Community'">
                
                <q-item-section avatar>
                    <q-icon name="fas fa-satellite-dish" />
                </q-item-section>
                <q-item-section>
                    <q-item-label>Community</q-item-label>
                </q-item-section>
                </q-item>
                <q-item clickable 
                active-class="my-menu-link"
                v-ripple
                :active="link === 'Settings'"
                @click="link = 'Settings'">
                
                <q-item-section avatar>
                    <q-icon name="fas fa-cog" />
                </q-item-section>
                <q-item-section>
                    <q-item-label>Settings</q-item-label>
                </q-item-section>
                </q-item>
                <q-item clickable 
                active-class="my-menu-link"
                v-ripple
                :active="link === 'Creators'"
                @click="link = 'Creators'">
                
                <q-item-section avatar>
                    <q-icon name="fas fa-user" />
                </q-item-section>
                <q-item-section>
                    <q-item-label>Creators</q-item-label>
                </q-item-section>
                </q-item>
            </q-list>
            <q-space></q-space>
            <div class="q-py-md" style="position: absolute; bottom:0; margin-left:75px">
                <q-btn color="light-blue-8" label="Lagout" class="q-px-lg" outline />
            </div>
        </q-drawer>
    </nav>
</template>
<script>
export default {
    name: 'LayoutDefault',
    data () {
        return {
            leftDrawerOpen: false,
            link: 'My page',
            text: ''
        }
    }
}
</script>
<style scoped>
.my-menu-link {
    border-left: 4px solid #2698D6
}
</style>