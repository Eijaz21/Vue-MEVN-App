<template>

    <div class="row justify-content-center">

        <div class="col-md-6">
            <!-- Content goes here -->
            <h3 class="text-center">Create Students</h3>

            <form @submit.prevent="handleSubmitForm">

                <div class="form-group">
                    <label for="name">Name</label>
                    <input type="text" name="" id="" class="form-control" v-model="student.name" required>
                </div>

                <div class="form-group">
                    <label for="email">Email</label>
                    <input type="email" name="" id="" class="form-control" v-model="student.email" required>
                </div>

                <div class="form-group">
                    <label for="phone">Phone</label>
                    <input type="text" name="" id="" class="form-control" v-model="student.phone" required>
                </div>

                <div class="form-group">
                   <button class="btn btn-danger btn-block">Create</button>
                </div>
            </form>
        </div>

    </div>

</template>

<script>
    export default {
      data() {
          return {
            student: {
                name: '',
                email: '',
                phone: ''
            }
          }
      },
      methods: {
        handleSubmitForm() {
            
        }
      }  
    }
</script>