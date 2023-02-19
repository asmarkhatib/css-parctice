<template>
  <div class="incoming-load-main">
    <div class="section-header">
      <img
        src="https://itl-cc-aws.s3.ap-south-1.amazonaws.com/my-alpha/theme1/assets/images/incoming-load.svg"
        alt="Header image"
      />
      <h3>Incoming Load</h3>
    </div>
    <div class="outer-row-cover">
      <div class="row" v-for="(item, index) in items" :key="index">
        <base-card>
          <div class="count-load-font">{{ item.kg }}</div>
          <div class="day-load-font">{{ item.day }}</div>
        </base-card>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      items: [
        { kg: "0 / 0 kg", day: "Pending Delivered" },
        { kg: "151 / 23.37 kg", day: "Inward Pending" },
        { kg: "19 / 5.82 kg", day: "Today" },
        { kg: "18 / 4.49 kg", day: "Tomorrow" },
        { kg: "4 / 0.66 kg", day: "2+ Days" },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.incoming-load-main {
  background-color: #f3f4f6;
  .section-header {
    display: flex;
    padding: 20px 40px;
    img {
      margin-right: 1rem;
    }
  }
  .outer-row-cover {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    padding: 0 40px 16px 40px;

    .row {
      .count-load-font {
        font-weight: 900;
        font-size: 20px;
      }
      .day-load-font {
        font-size: 12px;
       
      }
    }
  }
}
</style>
