<template>
  <div id="myWrapper">
    <p id="title">A Quick Tour of Spiky</p>
    <p id="explanation">
      Drop us a line, our experts will be back within a day <br />to talk about
      your educational needs
    </p>
    <div id="myForm" data-aos="fade-up">
      <b-form @submit="onSubmit" @reset="onReset" v-if="show" id="boostrapform">
        <b-form-group id="input-group-2" label="Your Name:" label-for="input-2">
          <b-form inline id="lineform">
            <label class="sr-only" for="inline-form-input-name">Name</label>
            <b-input
              id="firstname"
              class="mb-2 mr-sm-2 mb-sm-0"
              placeholder="First Name"
            ></b-input>
            <label class="sr-only" for="inline-form-input-lastname"
              >Lastname</label
            >
            <b-input
              id="lastname"
              class="mb-2 mr-sm-2 mb-sm-0"
              placeholder="Last Name"
            ></b-input>
          </b-form>
        </b-form-group>
        <b-form-group
          id="input-group-1"
          label="Email address:"
          label-for="input-1"
          description="We'll never share your email with anyone else."
        >
          <b-form-input
            id="input-1"
            v-model="form.email"
            type="email"
            required
            placeholder="Enter email"
          ></b-form-input>
        </b-form-group>
        <b-form-group id="input-group-3" label="Message:" label-for="input-3">
          <b-form-textarea
            id="input-3"
            v-model="form.text"
            required
          ></b-form-textarea>
        </b-form-group>
        <button type="button" class="btn btn-outline-danger">
          Schedule a Meeting
        </button>
      </b-form>
    </div>
  </div>
</template>

<script>
export default {
  name: "DropALine",
  data() {
    return {
      form: {
        email: "",
        name: "",
        lastname: "",
      },
      show: true,
    };
  },
  methods: {
    onSubmit(evt) {
      evt.preventDefault();
      alert(JSON.stringify(this.form));
    },
  },
};
</script>

<style scoped lang="scss">
@import "../assets/colors.scss";

button {
  font-family: "Brown Regular";
  float: right;
}

#myForm {
  width: 100%;
  display: flex;
  justify-content: center;
  text-align: center;
  zoom: 1.15;
  -moz-transform: scale(1.15);
  padding-bottom: 5%;
}

#boostrapform {
  width: 70%;
}

#firstname {
  width: 45%;
}

#lastname {
  width: 45%;
}

#title {
  font-family: "Brown Regular";
  font-size: 35px;
  color: $textcolor;
  text-align: center;
  padding-top: 3%;
}

#explanation {
  font-family: "Brown Regular";
  font-size: 25px;
  color: $expcolor;
  padding-bottom: 3%;
  text-align: center;
}
</style>
