## [中文](./README_SC.md)

# Iris Mysteria Helper

built on [Selenium WebDriver](https://github.com/SeleniumHQ/) for browser conrol and [OpenCV](https://github.com/opencv) for image recognition.

## 用途

解放双手 自动登录爱丽丝秘迹并自动执行操作

#### 功能包括但不限于
   - 学园训练
   - 每日苍粒子关卡
   - 每周素材关卡
   - 当期活动关卡
   - 领取礼物和任务奖励等等



## 使用之前

#### 因为种种原因......只能养老而不适用于新号
   - 点击功能时不会弹出教程挡住点击和图形识别
   - 苍粒子和所有的每周素材关卡已经通关过
   - 活动关卡的战斗不能出现战败的情况
   - 有充足的skip券
   
   
### 必要的配置
  #### 在爱丽丝秘迹
   1. 关闭event(イベント)开始的opening(オープニング)播放 在设置的game(ゲーム)里面 选择从不播放
   2. 用来执行活动关卡的队伍 从默认名"パーティーxx"改名为"event_clear" 或者在助手关闭event
  #### 在助手config.json
   1. 在"account"和"password"填入DMM账号和密码
   2. 设置"event"的"enable"为false关闭event功能 或者在在爱丽丝秘迹里配置活动队伍名称

## 注意事项
  ### 避免不当操作
   - scroll操作使用绝对坐标执行 若要改变浏览器大小或缩放比例 请先关闭weekly功能
   - 非无头模式下 注意浏览器窗口不能被最小化或者切换浏览器的tab 鼠标不能位于浏览器界面上 也不要点击cmd
   - (建议首次使用后切换成无头模式 在配置文件里设置"headless"为true)
  ### 可能问题
   - 可以手动打开程式使用的同一chrome进行操作 如果手动操作DMM登陆选择了保存用户名和密码 登陆时可能不会清理原来填入的值而是在后面继续添加用户名和密码 导致无法登录
   - 如果程式使用的chrome没有维持在最新版本的话 程式自动更新的driver版本可能会无法使用
  ## License
  ### MIT
  
欢迎自由修改和编辑