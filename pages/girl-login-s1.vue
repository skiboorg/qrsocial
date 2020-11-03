<template>
  <div>
    <section class="girl-register-page">

      <el-steps class="mb-40" :active="active" finish-status="success">
        <el-step title="Шаг 1"></el-step>
        <el-step title="Шаг 2"></el-step>
        <el-step title="Шаг 3"></el-step>
      </el-steps>

      <div v-if="active===0">
        <p class="section-subheader  mb-40">о нашем сервисе</p>
        <p class="mb-60">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem </p>

        <p class="section-subheader  mb-40">Как вы зарабатываете</p>
        <p class="mb-60">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem </p>

        <p class="section-subheader  mb-40">правила нашего сервиса</p>
        <p class="mb-60">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem </p>
        <vs-button @click="active+=1" style="width: 400px" color="danger" type="gradient">ДАЛЕЕ</vs-button>
      </div>
      <div v-if="active===1">
        <p class="section-subheader  mb-40">ВВЕДИТЕ ВАШИ ДАННЫЕ</p>

        <div class="girl-register-page-form__row">
          <vs-input  style="width: 400px;margin-right: 20px"  label-placeholder="ВАШЕ ФИО" v-model="value1"/>
          <vs-input   style="width: 400px"  label-placeholder="контактный телефон" v-model="value1"/>
        </div>
        <div class="girl-register-page-form__row">
          <vs-input  style="width: 400px;margin-right: 20px"  label-placeholder="придумайте никнейм" v-model="value1"/>
          <vs-input   style="width: 400px"  label-placeholder="пароль" v-model="value1"/>
        </div>
        <div class="girl-register-page-form__row mb-20">
          <vs-input  style="width: 400px;margin-right: 20px"  label-placeholder="ваша почта" v-model="value1"/>
          <vs-input   style="width: 400px"  label-placeholder="еще раз пароль" v-model="value1"/>
        </div>
        <p class="mb-20">ПРИКРЕПИТЕ ВАШИ ФОТО</p>
        <el-upload
          class="mb-40"
          action="#"
          :multiple="true"
          list-type="picture-card"
          :auto-upload="false">
          <i slot="default" class="el-icon-plus"></i>
          <div slot="file" slot-scope="{file}">
            <img
              class="el-upload-list__item-thumbnail"
              :src="file.url" alt=""
            >
            <span class="el-upload-list__item-actions">
        <span
          class="el-upload-list__item-preview"
          @click="handlePictureCardPreview(file)"
        >
          <i class="el-icon-zoom-in"></i>
        </span>
        <span
          v-if="!disabled"
          class="el-upload-list__item-delete"
          @click="handleDownload(file)"
        >
          <i class="el-icon-download"></i>
        </span>
        <span
          v-if="!disabled"
          class="el-upload-list__item-delete"
          @click="handleRemove(file)"
        >
          <i class="el-icon-delete"></i>
        </span>
      </span>
          </div>
        </el-upload>
        <el-dialog :visible.sync="dialogVisible">
          <img width="100%" :src="dialogImageUrl" alt="">
        </el-dialog>

        <vs-button @click="active+=1" style="width: 400px" color="danger" type="gradient">ДАЛЕЕ</vs-button>
      </div>





    </section>

  </div>
</template>

<script>

  export default {
    layout: 'login',
    data(){
      return {
        value1:'',
        input:'',
        active: 0,
      }
    },

  }
</script>


<style>

</style>
