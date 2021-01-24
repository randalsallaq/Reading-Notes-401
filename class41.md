# Data Fetching - NEXT.js

#### When you navigate to a page that’s pre-rendered using getStaticProps, Next.js fetches this JSON file (pre-computed at build time) and uses it as the props for the page component. This means that client-side page transitions will not call getStaticProps as only the exported JSON is used.


![f](https://miro.medium.com/max/1000/1*ycqhUTo1LqydeC355iHRoA.jpeg)

Only allowed in a page
getStaticProps can only be exported from a page. You can’t export it from non-page files.

One of the reasons for this restriction is that React needs to have all the required data before the page is rendered.

Also, you must use export async function getStaticProps() {} — it will not work if you add getStaticProps as a property of the page component.

Runs on every request in development
In development (next dev), getStaticProps will be called on every request.


# Deployment

The easiest way to deploy Next.js to production is to use the Vercel platform from the creators of Next.js. Vercel is an all-in-one platform with Global CDN supporting static & Jamstack deployment and Serverless Functions.

![c](https://i2.wp.com/blog.logrocket.com/wp-content/uploads/2019/06/csr-explanation.png?resize=800%2C564&ssl=1)
