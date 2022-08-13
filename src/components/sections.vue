<template>
  <div class="container-fluid ml-1">
    <headrer class="d-flex justify-content-between mb-3 mt-2 section-header">
      <div class="section py-1" 
      @click="selectedSection = 'CNBG'" 
      :class="[selectedSection == 'CNBG' ? 'selected' : '']">
        CNBG
      </div>
      <div class="section py-1" 
      @click="selectedSection = 'EBG'"
      :class="[selectedSection == 'EBG' ? 'selected' : '']">
        EBG
      </div>
      <div class="section py-1" 
          @click="selectedSection = 'Customer group'"
          :class="[selectedSection == 'Customer group' ? 'selected' : '']">
          Customer group
      </div>
      <div class="section py-1" 
      @click="selectedSection = 'Risk projects'"
      :class="[selectedSection == 'Risk projects' ? 'selected' : '']">
      Risk projects
      </div>
      <div class="section py-1" @click="selectedSection = 'Network security'"
      :class="[selectedSection == 'Network security' ? 'selected' : '']">
      Network security
      </div>
    </headrer>
    <div class="row  mx-2 " style="margin-top:15%"  v-show="selectedSection=='CNBG'">
      <div class="col-4 m-auto">
        <div class="row">
          <div class="col-12 mb-5 card border-0 shadow-sm CNBG-section">
            <div class="text-center mt-2 first-link">Some link here</div>
            <div class="text-center mt-1 second-link">Some link here</div>
            <div class="text-center mt-1 third-link">Some link here</div>
            <div class="text-center mt-1 mb-2 fourth-link">Some link here</div>
          </div>
          <div class="col-12 mt-5 card border-0 shadow-sm CNBG-section">
            <div class="text-center mt-2 first-link">Some link here</div>
            <div class="text-center mt-1 second-link">Some link here</div>
            <div class="text-center mt-1 third-link">Some link here</div>
            <div class="text-center mt-1 mb-2 fourth-link">Some link here</div>
          </div>
        </div> 
      </div> 
      <div class="col-3 text-center m-auto"> circle section</div>         
      <div class="col-4 m-auto">
        <div class="row">
          <div class="col-12 mb-5 card border-0 shadow-sm CNBG-section">
            <div class="text-center mt-2 first-link">Some link here</div>
            <div class="text-center mt-1 second-link">Some link here</div>
            <div class="text-center mt-1 third-link">Some link here</div>
            <div class="text-center mt-1 mb-2 fourth-link">Some link here</div>
          </div>
          <div class="col-12 mt-5 card border-0 shadow-sm CNBG-section">
            <div class="text-center mt-2 first-link">Some link here</div>
            <div class="text-center mt-1 second-link">Some link here</div>
            <div class="text-center mt-1 third-link">Some link here</div>
            <div class="text-center mt-1 mb-2 fourth-link">Some link here</div>
          </div>
        </div> 
      </div>         
    </div>
    <div v-show="selectedSection=='EBG'">
      hello from EBG           
    </div>
    <div v-show="selectedSection=='Customer group'">
      hello 3          
    </div>
    <div v-show="selectedSection=='Risk projects'">
      hello 4           
    </div>
    <div v-show="selectedSection=='Network security'">
      hello 5         
    </div>
                        
  </div>
</template>

<script>
export default {
  
  data () {
    return {
      selectedSection : 'CNBG'
    }
  },
}
</script>
<style scoped>
.section:hover{
  cursor:pointer
}
.selected{
  border-bottom: 3px solid rgb(75, 184, 227);
}
.section-header{
  /* border-bottom: 2px solid rgb(192, 190, 190); */
}
.CNBG-section{
  border-radius: 28px;
  margin: auto;
}
.first-link{
  width:90%;
  border-radius: 28px;
  background-color: rgb(125,193,122);
  color:white;
  margin:auto
}
.second-link{
  width:90%;
  border-radius: 28px;
  background-color: rgb(226,197,28);
  color:white;
  margin:auto
}
.third-link{
  width:90%;
  border-radius: 28px;
  background-color: rgb(105,184,221);
  color:white;
  margin:auto
}
.fourth-link{
  width:90%;
  border-radius: 28px;
  background-color: rgb(175,118,198);
  color:white;
  margin:auto
}
.fifth-link{
  width:90%;
  border-radius: 28px;
  background-color: rgb(224,74,59);
  color:white;
  margin:auto
}
</style>


