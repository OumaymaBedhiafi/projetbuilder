<template>
  <a-card 
    class="card"
  >
    <div class="container">
      <img
        class="thumbnail"
        src="data:image/jpeg;base64,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"
      >
      <div class="headings">
        <span class="title">{{ component.items.title }}</span>
        <div class="sub-title">
          <span class="value">{{ component.items.value }}</span>
          <span class="key">{{ component.items.key }}</span>
        </div>
        <hr>
        <div class="sub-title">
          <span class="value"> {{ component.items.value }}</span>
          <span class="key">{{ component.items.key }}</span>
        </div>
      </div>
    </div>
  </a-card>
</template>
<script>
export default {
  name: 'Card',
  
  props: {
  component: {
  type: Object,
  required: true
  }
  },

}
</script>
  <style lang="scss" scoped>
  .card {
    width: 120px;
    height: 175px;
    max-width: 50%;
    margin: auto;
    border: 1px solid lightgray;
    border-radius: 8%;
    .container {
     
      padding: 1vw;
      .thumbnail {
        position: absolute; /* Pour que l'image de couverture se positionne par-dessus les autres éléments */
            left: 9.9%;
             right: 0%;
             bottom:0%;
             top: 8%;
        width: 30px;
        
      }
      .headings{
        margin-top: 0.2vw;
        padding: 0.1PX;
        position: absolute; /* Pour que l'image de couverture se positionne par-dessus les autres éléments */
            left: 9.9%;
             right: 0%;
             bottom:0%;
             top: 30%;
        .title {
          color: rgb(67, 67, 67);
          font-size: 15px;
          margin-top: 5px;
        }
        .sub-title{
          margin-top: 0.1VW;
          .value{
            font-weight: bold;
            font-size: 19px;
            margin-right: 3px;
          }
          .key{
            font-size: 13px;
          }
        }
      }
      
    }
  }
  
  </style>