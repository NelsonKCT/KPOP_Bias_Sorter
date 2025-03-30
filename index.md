---
layout: default
---

<script type="text/javascript">
  var idolData = [
    // IVE
    { name: "Wonyoung", image: "{{ site.baseurl }}/assets/members/wonyoung.jpg", group: "IVE" },
    { name: "Yujin", image: "{{ site.baseurl }}/assets/members/yujin.jpg", group: "IVE" },
    { name: "Liz", image: "{{ site.baseurl }}/assets/members/liz.jpg", group: "IVE" },
    { name: "Rei", image: "{{ site.baseurl }}/assets/members/rei.jpg", group: "IVE" },
    { name: "Leeseo", image: "{{ site.baseurl }}/assets/members/leeseo.jpg", group: "IVE" },
    { name: "Gaeul", image: "{{ site.baseurl }}/assets/members/gaeul.jpg", group: "IVE" },
    
    // aespa
    { name: "Karina", image: "{{ site.baseurl }}/assets/members/karina.jpg", group: "aespa" },
    { name: "Giselle", image: "{{ site.baseurl }}/assets/members/giselle.jpg", group: "aespa" },
    { name: "Ningning", image: "{{ site.baseurl }}/assets/members/ningning.jpg", group: "aespa" },
    { name: "Winter", image: "{{ site.baseurl }}/assets/members/winter.jpg", group: "aespa" },
    
    // (G)I-DLE
    { name: "Miyeon", image: "{{ site.baseurl }}/assets/members/miyeon.jpg", group: "(G)I-DLE" },
    { name: "Minnie", image: "{{ site.baseurl }}/assets/members/minnie.jpg", group: "(G)I-DLE" },
    { name: "Soyeon", image: "{{ site.baseurl }}/assets/members/soyeon.jpg", group: "(G)I-DLE" },
    { name: "Yuqi", image: "{{ site.baseurl }}/assets/members/yuqi.jpg", group: "(G)I-DLE" },
    { name: "Shuhua", image: "{{ site.baseurl }}/assets/members/shuhua.jpg", group: "(G)I-DLE" },
    
    // Red Velvet
    { name: "Irene", image: "{{ site.baseurl }}/assets/members/irene.jpg", group: "Red Velvet" },
    { name: "Seulgi", image: "{{ site.baseurl }}/assets/members/seulgi.jpg", group: "Red Velvet" },
    { name: "Wendy", image: "{{ site.baseurl }}/assets/members/wendy.jpg", group: "Red Velvet" },
    { name: "Joy", image: "{{ site.baseurl }}/assets/members/joy.jpg", group: "Red Velvet" },
    { name: "Yeri", image: "{{ site.baseurl }}/assets/members/yeri.jpg", group: "Red Velvet" },
    
    // ITZY
    { name: "Yeji", image: "{{ site.baseurl }}/assets/members/yeji.jpg", group: "ITZY" },
    { name: "Lia", image: "{{ site.baseurl }}/assets/members/lia.jpg", group: "ITZY" },
    { name: "Ryujin", image: "{{ site.baseurl }}/assets/members/ryujin.jpg", group: "ITZY" },
    { name: "Chaeryeong", image: "{{ site.baseurl }}/assets/members/chaeryeong.jpg", group: "ITZY" },
    { name: "Yuna", image: "{{ site.baseurl }}/assets/members/yuna.jpg", group: "ITZY" }
  ];
  
  // 为了兼容原有代码，创建namMember和memberImages数组
  var namMember = idolData.map(idol => idol.name);
  var memberImages = idolData.map(idol => idol.image);
  
  // 添加一个函数，可以通过文件名查找偶像
  function findIdolByImageFilename(filename) {
    return idolData.find(idol => {
      // 从图片路径中提取文件名
      var imagePath = idol.image;
      var imageFilename = imagePath.split('/').pop();
      return imageFilename === filename;
    });
  }
  
  // 示例：如何使用文件名查找偶像
  // 例如，如果你有一个文件名 "winter.jpg"，你可以这样查找对应的偶像：
  // var idol = findIdolByImageFilename("winter.jpg");
  // console.log(idol.name); // 输出: "Winter"
  // console.log(idol.group); // 输出: "aespa"
  
  // 你也可以通过这种方式添加新的偶像：
  // idolData.push({
  //   name: "新偶像名称",
  //   image: "{{ site.baseurl }}/assets/members/新文件名.jpg",
  //   group: "组合名称"
  // });
  // 
  // 然后更新兼容数组：
  // namMember = idolData.map(idol => idol.name);
  // memberImages = idolData.map(idol => idol.image);
</script>