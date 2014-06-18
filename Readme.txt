Cocos2dxHtmlParse
Cocos2dHtmlParse是基于Cocos2dx中的Cocos2dxStudio扩展UI的Html文本解析和显示库
.

程序库依赖:
1.Cocos2dx v.23版本
2.Cocos2dx扩展UI库
3.Cocos2dx Lua支持

使用说明：
1.将Html代码库拷贝至 %Cocos2dx%/extensions/CocoStudio/GUI目录下
2.将UIHtmlView.pkg拷贝到%Cocos2dx%/tools/tolua++中
3.在CocoStudio.pkg最后加入$pfile "UIHtmlView.pkg"
4.最后运行build_studio.bat
5.再编译Cocos2dx,就可以在Lua中使用了

Lua中使用示例：
假定pWidget是你在Lua创建的Html容器窗口
local pHtmlView = UIHtmlView:create();
if pHtmlView ~= nil then
	pWidget:addChild( pHtmlView );
		
	pHtmlView:setSize( pWidget:getContentSize() );
	pHtmlView:setText( "<a href='lsf'>点这里</a>" );
end

官方主页: http://www.cocos2dres.com