<template>
  <div id="app">
   
    <b-navbar  type="dark" variant="info">
      <b-row cols-sm="1" cols-md="1" cols-lg="1" >
    <b-navbar-brand href="#"><h1 class="black"><router-link to="/">ChenShop</router-link></h1> </b-navbar-brand></b-row >
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-form>
        <b-row cols-sm="1" cols-md="2" cols-lg="1" >  <b-form-input size="sm" class="mr-sm-2" placeholder="Search"></b-form-input></b-row>
         <b-row cols-sm="1" cols-md="2" cols-lg="1"> <b-button size="sm" class="my-2 my-sm-2" type="submit">Search</b-button></b-row>
        </b-nav-form>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
<router-view/>
 
 
 
  <div class="container">
    <h1 align="center">จำนวน {{dataproduct1.amount+dataproduct2.amount+dataproduct3.amount+dataproduct4.amount+dataproduct5.amount+dataproduct6.amount+dataproduct7.amount+dataproduct8.amount+dataproduct9.amount}} ชิ้น </h1>
     <b-row cols-sm="1" cols-md="2" cols-lg="3">
    <b-card>
      <div class="card-header">
        <h4 class="my-0 fw-normal" align="center">{{dataproduct1.name}}</h4>
      </div>
      <div class="card-body">
        <img src="https://secure.ap-tescoassets.com/assets/TH/381/8850718801381/ShotType1_540x540.jpg"  width="300"  height=“300”>
        <ul class="list-unstyled text-small">50 บาท</ul>
        <div id="example-1">
          <button type="button" class="w-30 btn btn-lg btn-outline-primary" v-on:click= "dataproduct1.amount ++" >เพิ่มสินค้า</button>
           {{ dataproduct1.amount }} 
           <button type="button" class="w-30 btn btn-lg btn-outline-primary" v-on:click= "dataproduct1.amount--" >ลดสินค้า</button>
        </div>
      </div>
  </b-card>
    <b-card>
      <div class="card-header">
        <h4 class="my-0 fw-normal" align="center">{{dataproduct2.name}}</h4>
      </div>
      <div class="card-body">
        <img src="https://secure.ap-tescoassets.com/assets/TH/056/8851727003056/ShotType1_540x540.jpg" width="300"  height=“300”>
        <ul class="list-unstyled text-small">40 บาท</ul>
        <div id="example-1">
          <button type="button" class="w-30 btn btn-lg btn-outline-primary" v-on:click= "dataproduct2.amount ++" >เพิ่มสินค้า</button>
           {{ dataproduct2.amount }} 
           <button type="button" class="w-30 btn btn-lg btn-outline-primary" v-on:click= "dataproduct2.amount--" >ลดสินค้า</button>
        </div>
      </div>
    
    </b-card>
    <b-card >
   
      <div class="card-header">
        <h4 class="my-0 fw-normal" align="center">{{dataproduct3.name}}</h4>
      </div>
      <div class="card-body">
        <img src="https://secure.ap-tescoassets.com/assets/TH/060/8850425000060/ShotType1_540x540.jpg" width="300"  height=“300”>
        <ul class="list-unstyled text-small">55 บาท</ul>
        <div id="example-1">
          <button type="button" class="w-30 btn btn-lg btn-outline-primary" v-on:click= "dataproduct3.amount ++" >เพิ่มสินค้า</button>
           {{ dataproduct3.amount }} 
           <button type="button" class="w-30 btn btn-lg btn-outline-primary" v-on:click= "dataproduct3.amount--" >ลดสินค้า</button>
        </div>
      </div>
    
    </b-card>
    <b-card >
    
      <div class="card-header">
        <h4 class="my-0 fw-normal" align="center">{{dataproduct4.name}}</h4>
      </div>
      <div class="card-body">
        <img src="https://secure.ap-tescoassets.com/assets/TH/059/8851727002059/ShotType1_540x540.jpg" width="300"  height=“300”>
        <ul class="list-unstyled text-small">75 บาท</ul>
        <div id="example-1">
          <button type="button" class="w-30 btn btn-lg btn-outline-primary" v-on:click= "dataproduct4.amount ++" >เพิ่มสินค้า</button>
           {{ dataproduct4.amount }} 
           <button type="button" class="w-30 btn btn-lg btn-outline-primary" v-on:click= "dataproduct4.amount--" >ลดสินค้า</button>
        </div>
      </div>
 
    </b-card>
    <b-card>
     
      <div class="card-header">
        <h4 class="my-0 fw-normal" align="center">{{dataproduct5.name}}</h4>
      </div>
      <div class="card-body">
        <img src="https://secure.ap-tescoassets.com/assets/TH/007/8851019010007/ShotType1_540x540.jpg" width="300"  height=“300”>
        <ul class="list-unstyled text-small">45 บาท</ul>
        <div id="example-1">
          <button type="button" class="w-30 btn btn-lg btn-outline-primary" v-on:click= "dataproduct5.amount ++" >เพิ่มสินค้า</button>
           {{ dataproduct5.amount }} 
           <button type="button" class="w-30 btn btn-lg btn-outline-primary" v-on:click= "dataproduct5.amount--" >ลดสินค้า</button>
        </div>
      </div>
    
    </b-card>
    <b-card>

      <div class="card-header">
        <h4 class="my-0 fw-normal" align="center">{{dataproduct6.name}}</h4>
      </div>
      <div class="card-body">
        <img src="https://secure.ap-tescoassets.com/assets/TH/107/8850157400107/ShotType1_540x540.jpg" width="300"  height=“300”>
        <ul class="list-unstyled text-small">80 บาท</ul>
        <div id="example-1">
          <button type="button" class="w-30 btn btn-lg btn-outline-primary" v-on:click= "dataproduct6.amount ++" >เพิ่มสินค้า</button>
           {{ dataproduct6.amount }} 
           <button type="button" class="w-30 btn btn-lg btn-outline-primary" v-on:click= "dataproduct6.amount--" >ลดสินค้า</button>
        </div>
      </div>
   </b-card>
   <b-card>
      <div class="card-header">
        <h4 class="my-0 fw-normal" align="center">{{dataproduct7.name}}</h4>
      </div>
      <div class="card-body">
        <img src="https://secure.ap-tescoassets.com/assets/TH/501/8852052110501/ShotType1_540x540.jpg"  width="300"  height=“300”>
        <ul class="list-unstyled text-small">60 บาท</ul>
        <div id="example-1">
          <button type="button" class="w-30 btn btn-lg btn-outline-primary" v-on:click= "dataproduct7.amount ++" >เพิ่มสินค้า</button>
           {{ dataproduct7.amount }} 
           <button type="button" class="w-30 btn btn-lg btn-outline-primary" v-on:click= "dataproduct7.amount--" >ลดสินค้า</button>
        </div>
      </div>
  </b-card>
   <b-card>
      <div class="card-header">
        <h4 class="my-0 fw-normal" align="center">{{dataproduct8.name}}</h4>
      </div>
      <div class="card-body">
        <img src="https://secure.ap-tescoassets.com/assets/TH/408/8852052220408/ShotType1_540x540.jpg"  width="300"  height=“300”>
        <ul class="list-unstyled text-small">30 บาท</ul>
        <div id="example-1">
          <button type="button" class="w-30 btn btn-lg btn-outline-primary" v-on:click= "dataproduct8.amount ++" >เพิ่มสินค้า</button>
           {{ dataproduct8.amount }} 
           <button type="button" class="w-30 btn btn-lg btn-outline-primary" v-on:click= "dataproduct7.amount--" >ลดสินค้า</button>
        </div>
      </div>
  </b-card>
     <b-card>
      <div class="card-header">
        <h4 class="my-0 fw-normal" align="center">{{dataproduct9.name}}</h4>
      </div>
      <div class="card-body">
        <img src="https://secure.ap-tescoassets.com/assets/TH/927/8850425002927/ShotType1_540x540.jpg"  width="300"  height=“300”>
        <ul class="list-unstyled text-small">20 บาท</ul>
        <div id="example-1">
          <button  type="button" class="w-30 btn btn-lg btn-outline-primary" v-on:click= "dataproduct9.amount ++" >เพิ่มสินค้า</button>
           {{ dataproduct9.amount }} 
           <button type="button" class="w-30 btn btn-lg btn-outline-primary" v-on:click= "dataproduct9.amount--" >ลดสินค้า</button>
        </div>
      </div>
  </b-card>
     </b-row>  
     <div>
        
  <b-button  align="center" block variant="primary" @click="$bvModal.show('bv-modal-example')">ยืนยัน</b-button>
<b-modal id="bv-modal-example" size="lg" hide-footer>
    <div class="d-block text-center">
      <h3> <p class="h4 my-0 me-md-auto fw-normal">รายการสินค้า</p>
  <header  class="d-flex flex-column flex-md-row align-items-mide p-3 px-md-4 mb-3 bg-body border-bottom shadow-sm">
  <b-row cols-lg="1" cols-md="1" cols-sm="1">     
  <div v-if="dataproduct1.amount >= 1" >
    <p1>{{dataproduct1.name}}</p1>
    <img src="https://secure.ap-tescoassets.com/assets/TH/381/8850718801381/ShotType1_540x540.jpg" width="60"  height=“60”>
    <p1> x{{ dataproduct1.amount }} </p1>
    <p1> รวม{{ dataproduct1.amount*dataproduct1.price }} บาท </p1>
  </div><br>
  <div v-if="dataproduct2.amount >= 1" block>
    <p1>{{dataproduct2.name}}</p1>
    <img src="https://secure.ap-tescoassets.com/assets/TH/056/8851727003056/ShotType1_540x540.jpg" width="60"  height=“60”>
    <p1> x{{ dataproduct2.amount }}</p1>
     <p1> รวม{{ dataproduct2.amount*dataproduct2.price }} บาท </p1>
  </div><br>
  <div v-if="dataproduct3.amount >= 1">
    <p1>{{dataproduct3.name}}</p1>
    <img src="https://secure.ap-tescoassets.com/assets/TH/060/8850425000060/ShotType1_540x540.jpg" width="60"  height=“60”>
    <p1> x{{ dataproduct3.amount }}</p1>
     <p1> รวม{{ dataproduct3.amount*dataproduct3.price }} บาท </p1>
  </div><br>
  <div v-if="dataproduct4.amount >= 1">
    <p1>{{dataproduct4.name}}</p1>
    <img src="https://secure.ap-tescoassets.com/assets/TH/059/8851727002059/ShotType1_540x540.jpg" width="60"  height=“60”>
    <p1> x{{ dataproduct4.amount }}</p1>
     <p1> รวม{{ dataproduct4.amount*dataproduct4.price }} บาท </p1>
  </div><br>
  <div v-if="dataproduct5.amount >= 1">
    <p1>{{dataproduct5.name}}</p1>
    <img src="https://secure.ap-tescoassets.com/assets/TH/007/8851019010007/ShotType1_540x540.jpg" width="60"  height=“60”>
    <p1> x{{ dataproduct5.amount }}</p1>
     <p1> รวม{{ dataproduct5.amount*dataproduct5.price }} บาท </p1>
  </div><br>
  <div v-if="dataproduct6.amount >= 1">
    <p1>{{dataproduct6.name}}</p1>
    <img src="https://secure.ap-tescoassets.com/assets/TH/107/8850157400107/ShotType1_540x540.jpg" width="60"  height=“60”>
    <p1> x{{ dataproduct6.amount }}</p1>
     <p1> รวม{{ dataproduct6.amount*dataproduct6.price }}  บาท</p1>
  </div><br>
  <div v-if="dataproduct7.amount >= 1">
    <p1>{{dataproduct7.name}}</p1>
    <img src="https://secure.ap-tescoassets.com/assets/TH/501/8852052110501/ShotType1_540x540.jpg" width="60"  height=“60”>
    <p1> x{{ dataproduct7.amount }}</p1>
     <p1> รวม{{ dataproduct7.amount*dataproduct7.price }}  บาท</p1>
  </div><br>
<div v-if="dataproduct8.amount >= 1">
  <p1>{{dataproduct8.name}}</p1>
    <img src="https://secure.ap-tescoassets.com/assets/TH/408/8852052220408/ShotType1_540x540.jpg" width="60"  height=“60”>
    <p1> x{{ dataproduct8.amount }}</p1>
     <p1> รวม{{ dataproduct8.amount*dataproduct8.price }}  บาท</p1>
  </div><br>
  <div v-if="dataproduct9.amount >= 1">
    <p1>{{dataproduct9.name}}</p1>
    <img src="https://secure.ap-tescoassets.com/assets/TH/927/8850425002927/ShotType1_540x540.jpg" width="60"  height=“60”>
    <p1> x{{ dataproduct9.amount }}</p1>
     <p1> รวม{{ dataproduct9.amount*dataproduct9.price }} บาท </p1>
  </div></b-row>
  </header></h3><div class="my-4"><h4>ราคารวม{{ sum+dataproduct1.amount*dataproduct1.price+dataproduct2.amount*dataproduct2.price+
    dataproduct3.amount*dataproduct3.price+dataproduct4.amount*dataproduct4.price+dataproduct5.amount*dataproduct5.price+dataproduct6.amount*dataproduct6.price+dataproduct7.amount*dataproduct7.price+dataproduct8.amount*dataproduct8.price+dataproduct9.amount*dataproduct9.price }} บาท</h4>
 </div>
    </div>
    <b-button variant="light" block @click="$bvModal.hide"> <button type="button" class="w-50 btn btn-lg btn-outline-primary" v-on:click="say('สั่งซื้อเสร็จสิ้น')" >สั่งซื้อ</button></b-button>
  </b-modal>
   <b-button variant="danger" block value="Reset" onClick="javascript:location.reload();">Resset</b-button>
 
</div>

  
  </div>
  </div>
</template> 

<script>
export default {
  name: 'App',
  data(){
    return{
      dataproduct1:{
        name:"สินค้าที่ 1",
        price:50,
        amount:0

      },
      dataproduct2:{
        name:"สินค้าที่ 2",
        price:40,
        amount:0
      },
      dataproduct3:{
        name:"สินค้าที่ 3",
        price:55,
        amount:0
      },
      dataproduct4:{
        name:"สินค้าที่ 4",
        price:75,
        amount:0
      },
      dataproduct5:{
        name:"สินค้าที่ 5",
        price:45,
        amount:0
      },
      dataproduct6:{
        name:"สินค้าที่ 6",
        price:80,
        amount:0
      },
      dataproduct7:{
        name:"สินค้าที่ 7",
        price:65,
        amount:0
      },
      dataproduct8:{
        name:"สินค้าที่ 8",
        price:35,
        amount:0
      },
      dataproduct9:{
        name:"สินค้าที่ 9",
        price:20,
        amount:0
      },
      sum: 0,
      say: function (message) {
      alert(message)
    }
    }
  }
}
</script>
