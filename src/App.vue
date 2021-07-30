<template>

<body>

  

  <div style="text-align:center;color:white">
    <!-- <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css" integrity="sha384-HSMxcRTRxnN+Bdg0JdbxYKrThecOKuH5zCYotlSAcp1+c8xmyTe9GYg1l9a69psu" crossorigin="anonymous"> -->
    <link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
    
    <div>

      <div >
        <small>Hello</small>
        <br>
        <small>{{user.name}}</small>
      </div>

      <img src="https://cultivatedculture.com/wp-content/uploads/2019/12/LinkedIn-Profile-Picture-Example-Justin-Welsh.jpeg" alt="" class="image--cover" style="float: right;">
       
    </div>


    <div>
      <!-- <a href="#" class="btn btn-primary btn-lg active" role="button" aria-pressed="true">+</a> -->

      <button class="w3-button w3-circle w3-teal" style="position: absolute;right:10%;bottom:10%;">+</button>
    </div>

  </div>

  
</body>

</template>

<script>

// export default {
//   name: 'App',
//   components: {
//     HelloWorld
//   }
// }

export default {
  // setup(){
  //   onMounted(() => {
  //     // const messagesRef = db.database().ref("messages");
  //     // let docRef = db.collection('database').doc('practice')
  //     // let docRef = db.collection('database').doc('mainData')
  //     // let val = await docRef.get()
  //     // console.log(val)
  //     // const messagesRef = db.collection('database').doc('practice')
      
  //     // messagesRef.on('value', snapshot => {
  //     //   const data = snapshot.val();
  //     //   console.log(data)
  //     //   // let messages = [];
  //     //   // Object.keys(data).forEach(key => {
  //     //   //   messages.push({
  //     //   //     id: key,
  //     //   //     username: data[key].username,
  //     //   //     content: data[key].content
  //     //   //   });
  //     //   // });
  //     //   // state.messages = messages;
  //     // });


  //   });
  // },
  name: 'App',
  data(){
    return {

      user: {
        name: 'Nozomu',
        email: '',
        password: ''
      },

    }
  },

  computed: {
   
  },

  watch: {
    currentPlayer: {
      handler(val) {
        if (val === 'computer') {
          // CPUにプレイさせる
          this.playAsComputer()
        }
      },
      immediate: true
    }
  },


  methods: {
   

  },
  mounted(){


  },
  
}
</script>


<style>

.image--cover {
  width: 70px;
  height: 70px;
  border-radius: 50%;

  object-fit: cover;
  object-position: center right;
  /* right:0; */
}

body{
  background-color:#00008b;
}

</style>
