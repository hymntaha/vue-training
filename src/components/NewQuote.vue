<template>
    <div class="row">
        <div class="col-md-8 col-sm-offset-2 col-xs-12 col-md-6 col-md-offset-3">
            <label for="quote">Quote</label>
            <textarea class=form-control" v-model="quote" name="" id="" cols="30" rows="10"></textarea>
        </div>
        <div class="col-md-8 col-sm-offset-2 col-xs-12 col-md-6 col-md-offset-3">
            <button class="btn btn-primary" @click.prevent="createNew">Add Quote</button>
        </div>
    </div>
</template>
<script>
    export default {
      data: function () {
        return {
          quote:''
        }
      },
      methods:{
        createNew(){
          this.$emit('quoteAdded', this.quote);
          this.quote = '';
        }
      }
    }
</script>
