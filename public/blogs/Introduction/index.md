> 阅读此文章请确保你已完成部署2025-blog-public 项目
# 效果展示
![](https://cdn.jsdelivr.net/gh/yingshen-hk/cdn@master/%E8%87%AA%E5%AE%9A%E4%B9%89%E4%B8%AA%E4%BA%BA%E7%AE%80%E4%BB%8B/%E6%95%88%E6%9E%9C%E5%B1%95%E7%A4%BA1.png)![](https://cdn.jsdelivr.net/gh/yingshen-hk/cdn@master/%E8%87%AA%E5%AE%9A%E4%B9%89%E4%B8%AA%E4%BA%BA%E7%AE%80%E4%BB%8B/%E6%95%88%E6%9E%9C%E5%B1%95%E7%A4%BA2.png)

## 代码获取
### 1.1 自定义简介的设置代码
```ts
			<div>
				<label className='mb-2 block text-sm font-medium'>简介</label>
				<textarea
					value={formData.meta.Introduction}
					onChange={e => setFormData({ ...formData, meta: { ...formData.meta, Introduction: e.target.value } })}
					rows={3}
					className='bg-secondary/10 w-full rounded-lg border px-4 py-2 text-sm'
				/>
			</div>
```
### 1.2 定义Introduction 
```ts
const Introduction = siteContent.meta.Introduction || ''
```
### 1.3 替换原本简介内容
```ts
				<h1 className='font-averia mt-3 text-2xl'>
                    <span className='text-linear text-[32px]'>{username}</span>
					<br />
					<span className='text-linear text-[30px]'>{Introduction}</span>
                </h1>
```
# 修改代码

## 2.1 配置设置内容

### 2.1.1 找到需要的文件
代码更改在 `src/app/(home)` 目录这个目录代表首页所有文件。<br/>
我们需要的具体文件为 `src/app/(home)/config-dialog/site-settings/site-meta-form.tsx` 
找到后右上角铅笔图标开始修改
![](https://cdn.jsdelivr.net/gh/yingshen-hk/cdn@master/%E8%87%AA%E5%AE%9A%E4%B9%89%E4%B8%AA%E4%BA%BA%E7%AE%80%E4%BB%8B/%E8%AE%BE%E7%BD%AE%E4%BF%AE%E6%94%B91.png)
### 2.1.2 添加自定义简介的设置代码
复制1.1的代码并在第44行添加
![](https://cdn.jsdelivr.net/gh/yingshen-hk/cdn@master/%E8%87%AA%E5%AE%9A%E4%B9%89%E4%B8%AA%E4%BA%BA%E7%AE%80%E4%BB%8B/%E8%AE%BE%E7%BD%AE%E4%BF%AE%E6%94%B92.png)
### 2.1.3 保存并发布
点击右上角绿色Commit changes按钮完成发布
![](https://cdn.jsdelivr.net/gh/yingshen-hk/cdn@master/%E8%87%AA%E5%AE%9A%E4%B9%89%E4%B8%AA%E4%BA%BA%E7%AE%80%E4%BB%8B/%E8%AE%BE%E7%BD%AE%E4%BF%AE%E6%94%B93.png)

## 2.2 配置卡片内容

### 2.2.1 找到需要的文件
代码更改在 `src/app/(home)` 目录这个目录代表首页所有文件。<br/>
我们需要的具体文件为 `src/app/(home)/hi-card.tsx` 
找到后右上角铅笔图标开始修改
![](https://cdn.jsdelivr.net/gh/yingshen-hk/cdn@master/%E8%87%AA%E5%AE%9A%E4%B9%89%E4%B8%AA%E4%BA%BA%E7%AE%80%E4%BB%8B/%E4%BF%AE%E6%94%B9%E5%86%85%E5%AE%B94.png)
### 2.2.2 定义Introduction
复制1.2的代码并在第26行添加
![](https://cdn.jsdelivr.net/gh/yingshen-hk/cdn@master/%E8%87%AA%E5%AE%9A%E4%B9%89%E4%B8%AA%E4%BA%BA%E7%AE%80%E4%BB%8B/%E4%BF%AE%E6%94%B9%E8%AE%BE%E7%BD%AE5.png)
### 2.2.3 替换原本简介内容
复制1.3的代码并在第51行替换
替换前
![](https://cdn.jsdelivr.net/gh/yingshen-hk/cdn@master/%E8%87%AA%E5%AE%9A%E4%B9%89%E4%B8%AA%E4%BA%BA%E7%AE%80%E4%BB%8B/%E4%BF%AE%E6%94%B9%E5%89%8D.png)
替换后
![](https://cdn.jsdelivr.net/gh/yingshen-hk/cdn@master/%E8%87%AA%E5%AE%9A%E4%B9%89%E4%B8%AA%E4%BA%BA%E7%AE%80%E4%BB%8B/%E4%BF%AE%E6%94%B9%E5%90%8E.png)
### 2.2.4 保存并发布
与2.1.3一样点击右上角绿色Commit changes按钮完成发布

# 注意事项 重要事情说三次
## **请确保你提交的修改已经完成部署后再进行下一次修改**
## **请确保你提交的修改已经完成部署后再进行下一次修改**
## **请确保你提交的修改已经完成部署后再进行下一次修改**
