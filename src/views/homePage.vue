<template>
  <div id="app" class="container-fluid">
  <navbar></navbar>
  <slider-home class="mb-3"></slider-home>
  <div class="row ">
    <div class="col-8">
     <sections style="width:96%"  ></sections>
    </div>
    <div class="col-3 mt-2">
      <div class="row">
        <div class="col-12 card shadow-sm border-0">
          <span class="mt-1">
            Common seperate
          </span>
          <hr>
          <div class="mt-3 mb-3 row d-flex justify-content-center">
            <div class="col-4 text-center" >
              <div class="m-auto d-flex align-items-center justify-content-center" style="background-color:skyblue;border-radius:50%;width:50px;height:50px">
                <img src="/to-do-list.png"/>
              </div>
              <span style="font-size:12px">360 QC review</span>
            </div>
            <div class="col-3 text-center"> 
              <div class="m-auto d-flex align-items-center justify-content-center" style="background-color:skyblue;border-radius:50%;width:50px;height:50px">
              <img src="/letter.png"/>
              </div>
              <span style="font-size:12px">QEHS reverse inspection</span></div>
            <div class="col-3 text-center"> 
              <div class="m-auto d-flex align-items-center justify-content-center" style="background-color:skyblue;border-radius:50%;width:50px;height:50px">
              <img src="/hardware.png"/>
              </div>
              <span style="font-size:12px">QEHS reverse standard matching</span></div>
            <div class="col-4 text-center"> 
              <div class="m-auto d-flex align-items-center justify-content-center" style="background-color:skyblue;border-radius:50%;width:50px;height:50px">
              <img src="/reconciliation.png"/></div>
              <span style="font-size:12px">QEHS Passport</span></div>
            <div class="col-3 text-center">
              <div class="m-auto d-flex align-items-center justify-content-center" style="background-color:skyblue;border-radius:50%;width:50px;height:50px">
            <img src="/quality-control.png"/>
            </div>
              <span style="font-size:12px">EHS Mangers assessment</span>
            </div>
            <div class="col-3 text-center"> 
              <div class="m-auto d-flex align-items-center justify-content-center" style="background-color:skyblue;border-radius:50%;width:50px;height:50px">
              <img src="/to-do-list.png"/></div>
              <span style="font-size:12px">DQA Mangers Certification</span></div>
          </div>
          <div class="row">
            <div class="col-md-4 col-sm-12">
              <div></div>
            </div>
            <div class="col-md-4 col-sm-12"></div>
            <div class="col-md-4 col-sm-12"></div>
            <div class="col-md-4 col-sm-12"></div>
            <div class="col-md-4 col-sm-12"></div>
            <div class="col-md-4 col-sm-12"></div>
          </div> 
          <hr/>
        </div>
        <div class="col-12 mt-5 card shadow-sm border-0">
          <header class=" d-flex justify-content-between">
            <div  @click="selectedSection = 'Bulletin'"
                  class="section"
                  :class="[selectedSection == 'Bulletin' ? 'selected' : '']">Bulletin</div>
            <div @click="selectedSection = 'hot'"
                class="section"
                :class="[selectedSection == 'hot' ? 'selected' : '']">Hot</div>
            <div @click="selectedSection = 'QEHS'"
                class="section"
                :class="[selectedSection == 'QEHS' ? 'selected' : '']">QEHS guide</div>
          </header>
          <div class="mt-2" v-if="selectedSection == 'Bulletin'">
          <ul>
            <li>[6/30]IT Monthly Security Patch Bulletin (2020.6)
            </li>
            <li>[5/27]IT Monthly Security Patch Bulletin (2020.5)

            </li>
          </ul>
          </div>
            <div class="mt-2" v-if="selectedSection == 'hot'">Hot section</div>
            <div class="mt-2" v-if="selectedSection == 'QEHS'">QEHS section</div>
        </div>
        <div class="col-12  mt-3 card shadow-sm border-0">
          Peripheral support tool
          <hr/>
          <div class="mt-3 mb-3 row d-flex justify-content-center">
            <div class="col-4 text-center" >
              <div class="m-auto d-flex align-items-center justify-content-center" style="background-color:orange;border-radius:50%;width:50px;height:50px">
                <img src="/to-do-list.png"/>
              </div>
              <span style="font-size:12px">Onsite Operation Video Platform</span>
            </div>
            <div class="col-3 text-center"> 
              <div class="m-auto d-flex align-items-center justify-content-center" style="background-color:greenyellow;border-radius:50%;width:50px;height:50px">
              <img src="/letter.png"/>
              </div>
              <span style="font-size:12px">Rollout plan</span></div>
            <div class="col-3 text-center"> 
              <div class="m-auto d-flex align-items-center justify-content-center" style="background-color:orange;border-radius:50%;width:50px;height:50px">
              <img src="/hardware.png"/>
              </div>
              <span style="font-size:12px">HW RM Workspace</span></div>
            <div class="col-4 text-center"> 
              <div class="m-auto d-flex align-items-center justify-content-center" style="background-color:skyblue;border-radius:50%;width:50px;height:50px">
              <img src="/reconciliation.png"/></div>
              <span style="font-size:12px">Daily Reconciliation</span></div>
            <div class="col-3 text-center">
              <div class="m-auto d-flex align-items-center justify-content-center" style="background-color:plum;border-radius:50%;width:50px;height:50px">
            <img src="/quality-control.png"/>
            </div>
              <span style="font-size:12px">QC</span>
            </div>
            <div class="col-3 text-center"> 
              <div class="m-auto d-flex align-items-center justify-content-center" style="background-color:peru;border-radius:50%;width:50px;height:50px">
              <img src="/to-do-list.png"/></div>
              <span style="font-size:12px">FWCC</span></div>
          </div>
        </div>
      </div>
    </div>
  </div>
  </div>
</template>
<script>

import navbar from "../components/navbar.vue"
import sections from '../components/sections.vue'
import sliderHome from "../components/sliderHome.vue"
export default{
  name:'App',
  components:{
    sections,
    navbar,
    sliderHome
    }
    , 
    data(){
      return{
        selectedSection :'Bulletin'
      }
    }
}
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');
#app{
  font-family: Poppins;
}
.selected{
  border-bottom: 3px solid rgb(75, 184, 227);
  color:rgb(75, 184, 227)
}
.section:hover{
cursor: pointer;
}
</style>
