<template>
    <div>
      <div v-if="showImageA">
        <!-- Hiển thị hình ảnh A -->
        <img src="https://www.elle.vn/wp-content/uploads/2017/07/25/hinh-anh-dep-1.jpg" alt="Image A">
      </div>
      <div v-if="showImageB">
        <!-- Hiển thị hình ảnh B -->
        <img src="https://d1hjkbq40fs2x4.cloudfront.net/2016-01-31/files/1045-2.jpg" alt="Image B">
      </div>
      <div>
        <!-- Hiển thị đoạn văn -->
        <p>{{ paragraph }}</p>
      </div>
    </div>
  </template>
  
  <script>
export default {
  data() {
    return {
      showImageA: true,
      showImageB: false,
      paragraph: "Đây là đoạn văn"
    };
  },
  mounted() {
    window.addEventListener('scroll', this.handleScroll);
  },
  destroyed() {
    window.removeEventListener('scroll', this.handleScroll);
  },
  methods: {
    handleScroll() {
      // Kiểm tra nếu người dùng đã cuộn đến vị trí mong muốn, sau đó hiển thị hình ảnh B
      const scrollPosition = window.scrollY;
      const threshold = 500; // Vị trí ngưỡng cuộn đến để hiển thị hình ảnh B

      if (scrollPosition > threshold) {
        this.showImageA = false;
        this.showImageB = true;
        // Loại bỏ sự kiện cuộn sau khi đã hiển thị hình ảnh B
        window.removeEventListener('scroll', this.handleScroll);
      }
    }
  }
};
</script>
  