<template>
  <el-checkbox-group v-model="checkList">
    <el-checkbox label="Option A"/>
    <el-checkbox label="Option B"/>
    <el-checkbox label="Option C"/>
    <el-checkbox label="disabled" disabled/>
    <el-checkbox label="selected and disabled" disabled/>
  </el-checkbox-group>

  <div>
    <el-checkbox-group v-model="checkboxGroup1">
      <el-checkbox-button v-for="city in cities" :key="city" :label="city">{{
          city
        }}
      </el-checkbox-button>
    </el-checkbox-group>
  </div>
  <div class="demo-button-style">
    <el-checkbox-group v-model="checkboxGroup2" size="medium">
      <el-checkbox-button v-for="city in cities" :key="city" :label="city">{{
          city
        }}
      </el-checkbox-button>
    </el-checkbox-group>
  </div>
  <div class="demo-button-style">
    <el-checkbox-group v-model="checkboxGroup3" size="small">
      <el-checkbox-button
          v-for="city in cities"
          :key="city"
          :label="city"
          :disabled="city === 'Beijing'"
      >{{ city }}
      </el-checkbox-button
      >
    </el-checkbox-group>
  </div>
  <div class="demo-button-style">
    <el-checkbox-group v-model="checkboxGroup4" size="mini" disabled>
      <el-checkbox-button v-for="city in cities" :key="city" :label="city">{{
          city
        }}
      </el-checkbox-button>
    </el-checkbox-group>
  </div>
  <div class="demo-button-style">
    <el-checkbox-group v-model="checkboxGroup5" size="mini">
      <el-checkbox label="Option1" border></el-checkbox>
      <el-checkbox label="Option2" border disabled></el-checkbox>
    </el-checkbox-group>
  </div>
</template>

<script lang="ts">
import {defineComponent, reactive, ref, toRefs} from 'vue'

const cityOptions = ['Shanghai', 'Beijing', 'Guangzhou', 'Shenzhen']

export default defineComponent({
  setup() {
    const checkList = ref(['selected and disabled', 'Option A'])
    const state = reactive({
      checkboxGroup1: ['Shanghai'],
      checkboxGroup2: ['Shanghai'],
      checkboxGroup3: ['Shanghai'],
      checkboxGroup4: ['Shanghai'],
      checkboxGroup5: [],
      cities: cityOptions,
    })
    return {
      checkList,
      ...toRefs(state),
    }
  },
})
</script>

<style scoped>
.demo-button-style {
  margin-top: 24px;
}
</style>
