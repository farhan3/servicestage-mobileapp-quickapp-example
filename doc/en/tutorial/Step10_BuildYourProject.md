## Step 10:  (Optional) Start your own Mobile App Project

This step provides instructions for developer who want to know more about creating a Mobile Application from scratch.  
To create a quick app project requires Node JS and hap toolkit.  Node JS and hap toolkit installation are explained in Step 2. Running quick app requires Android device, such as a physical android device. Detailed steps for handset setup is described in Step 7.

Below are the instructions to create the mobile application using Quick App.

1.	To create new quick app project you need to install the toolkit tool and debugger.

Run the following command from the command line.

```
   npm install -g hap-toolkit
```

Executing the command line hap –V will output the version information indicating that the hap-toolkit installation is successful, as shown in the following command.

```
   hap –V
```

2.	After installing the toolkit tool, you can hap create a project template with global commands as follows:

```	
   hap init <project name>
   e.g: hap init QuickEats	
```

3.	After the command is executed, a <ProjectName>folder will be created in the current directory as the project root directory. This project already contains the initial code of the project configuration and sample page. The main structure of the project root directory is as follows.

```
	├── sign                      rpk包签名模块
	│   └── debug                 调试环境
	│       ├── certificate.pem   证书文件
	│       └── private.pem       私钥文件
	├── src
	│   ├── Common                公用的资源和组件文件
	│   │   └── logo.png          应用图标
	│   ├── Demo                  页面目录
	│   |   └── index.ux          页面文件，可自定义页面名称
	│   ├── app.ux                APP文件，可引入公共脚本，暴露公共数据和方法等
	│   └── manifest.json         项目配置文件，配置应用图标、页面路由等
	└── package.json              定义项目需要的各种模块及配置信息
```

  A brief description of the directory is as follows.

* **src** : project source folder
* **sign** : signature module, the signature generation methods are detailed in the document [https://doc.quickapp.cn/tools/compiling-tools.html](https://doc.quickapp.cn/tools/compiling-tools.html)   


4. Please refer to [https://doc.quickapp.cn/tutorial/](https://doc.quickapp.cn/tutorial/) for more information. 
