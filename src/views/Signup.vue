<template>
    <div>
        <v-container>
            <v-row>
                <v-col>
                    <v-form>
                        <v-text-field label="Email" type="email"></v-text-field>
                        <v-autocomplete label="Which browser do you use?" :items="browsers"></v-autocomplete>
                        <v-file-input label="Attach Profile Picture"></v-file-input>
                        <v-text-field label="Birthday" v-model="birthday" readonly></v-text-field>
                        <v-date-picker v-model="birthday" ></v-date-picker>
                        <v-checkbox label="Agree to Terms and Conditions"></v-checkbox>
                        <v-btn type="submit" color="primary">Submit</v-btn>
                    </v-form>
                </v-col>
            </v-row>
        </v-container>
    </div>
</template>

<script>
    export default {
        data: () => ({
            browsers: ['Chrome', 'Firefox', 'Safari', 'Edge', 'Brave'],
            birthday: ''
        })
    }
</script>

<style scoped>

</style>