<template>
  <div>
    <h2>Contact</h2>

    <p>{{errors}}</p>

    <form @submit.prevent="contactForm">
        <p>Email: <input type="text" placeholder="Email" v-model="form.email"></p>
        <p>First Name: <input type="text" placeholder="First" v-model="form.first"></p>
        <p>Last Name: <input type="text" placeholder="Last" v-model="form.last"></p>
        <p>Message: <textarea placeholder="Message" v-model="form.message"></textarea></p>

        <button>Submit</button>
    </form>
        
        
  </div>
</template>

<script>
export default {
  name: 'Contact',
  data(){
    return {
        form: {
            email: '',
            first: '',
            last: '',
            message: ''
        },
        errors: []
    }
  },
  methods: {
    contactForm() {
        if (this.form.name && this.form.email) {
        return true;
      }

      this.errors = [];

      if (!this.form.name) {
        this.errors.push('Name required.');
      }
      if (!this.form.email) {
        this.errors.push('Email required.');
      }
    }
  }
}
</script>