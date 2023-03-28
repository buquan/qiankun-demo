 - pnpm install
 - pnpm start


 ### 此demo操作步骤
  - 访问 localhost:5555
  - 点击 '去app1'
  - 然后点击 '去我的login' 按钮

 ### 现象
  - 每次都是 master app 的layouts/index文件的 main layout -> render 先执行，复合预期
  - 但是项目中，第二次操作就是子组件的根组件先监听到理由变化， 然后才是根组件
  - demo的打印顺序：
   1. main layout -> render
   2. app1 -> login render

