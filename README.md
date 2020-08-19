### Use Demo
``` 将源码下载到自己的项目目录下，比如下载到loader文件夹，修改webpack.config查找loader路径
resolveLoader: {
  modules: ['node_modules','loaders']
},

``` 在webpack.config配置文件中loader配置加上以下代码
{
  test: /\.html$/,
  use: [
         {
          loader: 'replace-img-url-loader',
          options: {
            replaceUrl: '',
            outputPath: ''
          }
        }
      ]
}
