# ChingMuSimulink
ChingMu Vrpn for matlab simulink<br>
操作说明：<br>
注：simulink中需要给变量设置上限，过大上限会影响速度，默认输出尺寸上限为10刚体，如需支持更多刚体，在model explorer中修改trackerlist尺寸上限<br>
1.将.dll、.h、.m文件放到同一路径下，并在matlab中将当前文件夹改为该路径。<br>
2.在Matlab中执行：mex -setup， 安装VS编译器。<br>
3.修改getVrpnArray.m中的VrpnServer地址。<br>
4.打开Simulink_Multi_NoDisplay.slx，修改Body ID input。<br>
5.使用Simulation下的运行开始接收数据。<br>
6.退出matlab前，调用以下两行命令卸载dll:<br>
&emsp;&emsp;calllib('CMVrpn', 'CMUnityQuitExtern');<br>
&emsp;&emsp;unloadlibrary('CMVrpn');<br>
[CMVrpn_Simulink.zip](https://github.com/ChingMuVisionTech/ChingMuSimulink/files/14771795/CMVrpn_Simulink.zip)
