<template>
    <div>
        <h2>Form validation</h2>
        <div>
            <pre>{{ JSON.stringify(formValues, null, 2 )}}</pre>
        </div>
        <form @submit="submitForm">
            <div>
                <label for="name">Name</label>
                <input type="text" id="name" v-model.trim="formValues.name">
            </div>
            <div>
                <label for="profile">Profile Summary</label>
                <input type="text" id="profile" v-model="formValues.profile">
            </div>
            <div>
                <label for="country">Country</label>
                <select name="" id="country" v-model="formValues.country">
                    <option value="">Select a country</option>
                    <option value="india">India</option>
                    <option value="vietnam">VietNam</option>
                    <option value="singapore">Singapore</option>
                </select>
            </div>
            <div>
                <label for="job-location">Job Location</label>
                <select name="" id="job-location" multiple v-model="formValues.jobLocation">
                    <option value="india">India</option>
                    <option value="vietnam">VietNam</option>
                    <option value="singapore">Singapore</option>
                </select>
            </div>
            <div style="display:inline">
                <input type="checkbox" id="remoteWork" v-model="formValues.remoteWork" true-value="yes" false-value="no">
                <label for="remoteWork">Open to remote work?</label>
            </div>
            <div>
                <label>Skill set</label>
                <input type="checkbox" id="html" value="html" v-model="formValues.skillSet">
                <label for="html">HTML</label>
                <input type="checkbox" id="css" value="css"  v-model="formValues.skillSet">
                <label for="css">CSS</label>
                <input type="checkbox" id="javascript" value="javascript" v-model="formValues.skillSet">
                <label for="javascript">Javascript</label>
            </div>
            <div>
                <label for="">Years of Experience</label>
                <input type="radio" id="0-2" value="0-2" v-model="formValues.yearsOfExperience">
                <label for="0-2">0-2</label>
                <input type="radio" id="3-5" value="3-5" v-model="formValues.yearsOfExperience">
                <label for="3-5">3-5</label>
                <input type="radio" id="5-10" value="5-10" v-model="formValues.yearsOfExperience">
                <label for="5-10">5-10</label>
            </div>
            <button>Submit</button>
        </form>
    </div>
</template>
<script>
export default {
    name: 'NewComponent',
    data() {
        return {
            formValues: {
                name: '',
                profile: '',
                country: '',
                jobLocation:[],
                remoteWork: "no",
                skillSet:[],
                yearsOfExperience: ''
            }
        }
    },
    methods: {
        submitForm(event) {
           event.preventDefault();
           console.log("Event", this.formValues);
        }
    }
}
</script>
<style scoped>
    label {
        font-weight: bold;
        display: flex;
        margin-bottom: 5px;
    }
    input + label {
        font-weight: bold;
        display: inline-flex;
        margin-right: 20px;
    }
    input[type='text'],
    textarea,
    select {
        display: block;
        width: 400px;
        padding: 6px 12px;
        font-size: 14px;
        line-height: 1.42857143;
        color: #555;
        background-color: #fff;
        background-image: none;
    }
</style>