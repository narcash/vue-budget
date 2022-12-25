<template>
  <ElCard>
    <ElForm :model="formData">
        <ElFormItem lable="Type" prop="type">
            <Elselect v-model="formData.type" placeholder="Choose type ...">
                <ElOption lable="Income" value="INCOME"></ElOption>
                <ElOption lable="Outcome" value="OUTCOME"></ElOption>
            </Elselect>
        </ElFormItem>
        <ElFormItem lable="Comments" prop="comment">
            <ElInput v-model="formData.comment" />
        </ElFormItem>
        <ElFormItem lable="Value" prop="value">
            <ElInput v-model.number="formData.value" />
        </ElFormItem>
        <ElButton @click="" type="primary">Submit</ElButton>
    </ElForm>
  </ElCard>
</template>

<script>
export default {
    name: "Form",
    data: () => ({
        formData: {
            type: "INCOME",
            comment: "",
            value: 0
        }
    }),
    methods: {
        onSubmit() {
            
        }
    }

}
</script>

<style scoped>

</style>