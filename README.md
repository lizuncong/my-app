## app router
- 在app目录下的就是app router工作区
- app router基于react server components，支持共享布局，嵌套路由，loading状态，错误处理等。
- app router 比 page router优先级高，应该避免使用同名的url
- 包含page.tsx文件的，都将成为一个路由
- Passing data between a parent layout and its children is not possible. 
- 可以通过在layout.js或者page.js文件中导出metadata对象来修改html标签中的seo标签
- 路由导航
    + `<Link>` 组件。提供了prefetching和客户端导航的能力。是主要也是比较推荐的方式。可以通过这个保持页面跳转后的滚动距离
    + useRouter hook。（客户端组件）
    + redirect 函数(服务端组件)
    + 原生history api