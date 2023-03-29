 - pnpm install
 - pnpm start


 ### 此demo操作步骤
  - 访问 localhost:5555
  - 点击 '去app1'
  - 然后点击 '去我的login' 按钮

 ### 现象
  - dynamicImport: true, 每次都是 master app 的layouts/index文件的 main layout -> render 先执行， 然后qiankun-app1的 app1 -> login render 执行
  - dynamicImport: false, 每次都是 qiankun-app1的 app1 -> login render 先执行， 然后master app 的layouts/index文件的 main layout -> render 执行
