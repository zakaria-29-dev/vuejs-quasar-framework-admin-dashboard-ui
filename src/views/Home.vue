<template>
  <div class="q-pa-md">
   <div class="row q-col-gutter-md">
     <div class="col-4">
<q-card class="my-card  q-py-sm">
      <q-item>
        <q-item-section avatar>
          <q-avatar square>
            <img src="https://cdn.quasar.dev/img/boy-avatar.png">
          </q-avatar>
        </q-item-section>

        <q-item-section>
          <q-item-label><strong>AAE IdeaPro</strong> </q-item-label>
          <q-item-label caption>
            UI/UX Designer
          </q-item-label>
        </q-item-section>
        <q-item-section>
          <q-btn color="light-blue-8" label="Edit"   class="q-px-md" />
        </q-item-section>
      </q-item>

      <q-separator />
      <q-item>
        <q-item-section>
          <q-item-label class="text-center"><strong>69</strong> </q-item-label>
          <q-item-label class="text-center" caption>
            Shots
          </q-item-label>
        </q-item-section>
        <q-item-section>
          <q-item-label class="text-center"><strong>2747</strong> </q-item-label>
          <q-item-label class="text-center" caption>
            Followers
          </q-item-label>
        </q-item-section>
         <q-item-section>
          <q-item-label class="text-center"><strong>678</strong> </q-item-label>
          <q-item-label class="text-center" caption>
            Following
          </q-item-label>
        </q-item-section>
         <q-item-section>
          <q-item-label class="text-center"><strong>78</strong> </q-item-label>
          <q-item-label class="text-center" caption>
            Lithning
          </q-item-label>
        </q-item-section>
      </q-item>
    <q-separator />
    <q-item>
       <q-item-section>
         <q-btn color="primary" icon="mail" label="Message" flat/>
        </q-item-section>
         <q-item-section>
          <q-btn color="grey" label="Folloaw"/>
        </q-item-section>
    </q-item>
    </q-card>

        </div>
        <div class="col-4">
<q-card class="my-card " >
      <q-item>
        <q-item-section>
          <q-item-label caption>
            Give your support
          </q-item-label>
        </q-item-section>
      </q-item>
      <q-separator />
      <q-item>
        <q-item-section avatar>
          <q-btn round color="blue-2" text-color="blue-8" icon="fas fa-bolt"/>

        </q-item-section>
       
         <q-item-section>
          <q-badge color="white text-black">
      Quantity:
    </q-badge>

    <q-slider
      v-model="value"
      :min="-20"
      :max="20"
      :step="4"
      label
      label-always
      color="light-green"
    />
        </q-item-section>
      </q-item>
    <q-separator />
    <q-item>
       <q-item-section>
         <q-btn color="primary" icon-right="fas fa-chevron-right" label="SUPPORT" flat/>
        </q-item-section>
    </q-item>
    </q-card>
        </div>
        <div class="col-4">
          <q-card class="my-card q-py-sm">
            <q-item>
              <q-item-section>
                <q-btn color="light-blue-8" icon="fab fa-facebook-f" label="Share with facebook" />
              </q-item-section>
              <q-item-section avatar>
                <q-btn flat round color="grey-6" icon="fas fa-times" size="sm" />
              </q-item-section>
            </q-item>
            <q-item>
              <q-item-section>
                <q-btn color="grey-6" icon="fab fa-twitter" text-color="black" label="Tweet with twitter" outline />
              </q-item-section>
              <q-item-section avatar>
                <q-btn flat round color="grey-6" icon="fas fa-times" size="sm" />
              </q-item-section>
            </q-item>
            <q-item>
              <q-item-section>
                <q-btn color="grey-6" icon="fab fa-pinterest-p" text-color="black" label="Save with pinterest" outline />
              </q-item-section>
              <q-item-section avatar>
                <q-btn flat round color="grey-6" icon="fas fa-times" size="sm" />
              </q-item-section>
            </q-item>
          </q-card>
        </div>

   </div>
   <div class="row q-col-gutter-md">
      <div class="col-8">
        <q-toolbar >
        <q-toolbar-title class="text-overline">ACTIVE PROJECTS</q-toolbar-title>
        <q-btn flat text-color="light-blue-8" label="Show All" />
      </q-toolbar>
    
<q-card class="my-card" style="padding: 33px 0px 33px 0px;">
      <q-item>
        <q-item-section avatar>
           <q-btn round color="blue-2" text-color="blue-8" icon="fas fa-bolt"/>
        </q-item-section>

        <q-item-section>
          <q-item-label><strong>Solar Management Dashboard</strong> </q-item-label>
          <q-item-label caption>
            UI/UX Redesign
          </q-item-label>
          <q-item-label><strong>4 Weeks</strong> </q-item-label>
        </q-item-section>
        <q-item-section>
         <q-item-label class="text-green"><strong>Budget: $1200</strong> </q-item-label>
        </q-item-section>
        <q-item-section>
          <q-btn color="light-blue-8" label="Deliver"    />
          <q-btn  text-color="black" label="Cancel"   outline class="q-mt-sm"/>
        </q-item-section>
      </q-item>
    </q-card>
        </div>
        <div class="col-4">
          <q-toolbar>
            <q-toolbar-title class="text-overline">WORKS AVAILABLE</q-toolbar-title>
            <q-btn flat text-color="light-blue-8" label="Show All"></q-btn>
          </q-toolbar>
          <q-card class="my-card q-py-sm">
            <q-item>
              <q-item-section avatar>
                <q-btn round color="green-2" text-color="green-8" icon="fas fa-cannabis" ></q-btn>
              </q-item-section>
              <q-item-section>
                <q-item-label><strong>Starbucks</strong></q-item-label>
                <q-item-label caption>Website UI Redesign</q-item-label>
              </q-item-section>
              <q-item-section>
                <q-btn text-color="black" label="Quote" outline class="q-mt-sm" />
              </q-item-section>
            </q-item>
          </q-card>
          <q-card class="my-card q-py-sm q-mt-sm">
            <q-item>
              <q-item-section avatar>
                <q-btn round color="yellow-2" text-color="yellow-8" icon="fas fa-utensils" />
              </q-item-section>
              <q-item-section>
                <q-item-label><strong>Untapped</strong></q-item-label>
                <q-item-label caption>
                  Wensite Design
                </q-item-label>
              </q-item-section>
              <q-item-section>
                <q-btn text-color="black" label="Quote" outline class="q-mt-sm" />
              </q-item-section>
            </q-item>
          </q-card>
        </div>
   </div>
   <q-toolbar>
     <q-toolbar-title><strong>My shots</strong></q-toolbar-title>
     <q-btn color="dark" icon-right="fas fa-chevron-down" label="Latest" flat />
   </q-toolbar>
   <div class="row q-col-gutter-md">
     <div class="col-3">
       <q-card class="my-card">
         <q-img src="1.jpg">
           <div class="absolute-bottom">
             <div class="text-subtitle1">Merketing Landing page</div>
             <div class="text-subtitle2">03 August 2018</div>
           </div>
         </q-img>
       </q-card>
     </div>
     <div class="col-3">
       <q-card class="my-card">
         <q-img src="2.jpg">
           <div class="absolute-bottom">
             <div class="text-subtitle1">Community Dashboard</div>
             <div class="text-subtitle1">03 August 2018</div>
           </div>
         </q-img>
       </q-card>
     </div>
     <div class="col-3">
       <q-card class="my-card">
         <q-img src="3.jpg" height="156px">
           <div class="absolute-bottom">
             <div class="text-subtitle1">Movie Booking App</div>
             <div class="text-subtitle2">03 August 2018</div>
           </div>
         </q-img>
       </q-card>
     </div>
     <div class="col-3">
       <q-card class="my-card">
         <q-img src="4.png" height="156px">
           <div class="absolute-bottom">
             <div class="text-subtitle1">Pattern Grandients</div>
             <div class="text-subtitle2">03 August 2018</div>
           </div>
         </q-img>
       </q-card>
     </div>
   </div>
  </div>
</template>

<script>


export default {
  name: 'Home',
 data: () => ({
   value: 0
 })
}
</script>
