
https://docker-py.readthedocs.io/en/stable/
https://desktop.docker.com/win/main/amd64/Docker%20Desktop%20Installer.exe?utm_source=docker&utm_medium=webreferral&utm_campaign=dd-smartbutton&utm_location=header

https://www.zhihu.com/question/68766084

https://www.cnblogs.com/Alier/p/8125524.html

https://m.yisu.com/zixun/165800.html

https://www.pythonheidong.com/blog/article/900860/4a50ac62cdfe9dcb5d4d/

https://www.pugetsystems.com/labs/articles/Unreal-Engine-12th-Gen-Intel-Core-vs-AMD-Ryzen-5000-Series-2249/



 if __name__ == "__main__":
  v_compare = QVersionNumber(5,6,0)
  v_current,_ = QVersionNumber.fromString(QT_VERSION_STR) #获取当前Qt版本
  if QVersionNumber.compare(v_current,v_compare) >=0 :
    QApplication.setAttribute(Qt.AA_EnableHighDpiScaling)  #Qt从5.6.0开始，支持High-DPI
    app = QApplication(sys.argv)  #
  else:
    app = QApplication(sys.argv)
    font = QFont("宋体")
    pointsize = font.pointSize()
    font.setPixelSize(pointsize*90/72)
    app.setFont(font)
  mymainwin = Mymainwindow()
  mymainwin.show()
  sys.exit(app.exec())
