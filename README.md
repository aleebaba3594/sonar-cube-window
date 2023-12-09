# sonar-cube-window
sonar cube with windows locally configuration setup (all the steps)

1) install jdk java latest version 
2) set system env path to bin folder of java jdk (C:\Program Files\Java\jdk-17\bin)
3) download comunity editon sonar cube and sonar scanner and paste them into C folder.
4) goto sonarcube->conf->sonar and un-comment the sonar.web.port=9099 and set port whatever suits you.
5) goto sonarcube->bin->windows-> and StartSonar.bat , run that file.
6) now open cmd and goto the sonar-scanner->bin folder and then paste the code copied from Execute the Scaner tab i,e (sonar-scanner.bat -D"sonar.projectKey=ovasave" -D"sonar.sources=." -D"sonar.host.url=http://localhost:9099" -D"sonar.token=sqp_345066c27e5062e6ff3033e19c723f89e6ae16fe" -D"sonar.projectBaseDir=.\path-of-your-proj")
7) at the end of that url change the path to your project directory eg (-D"sonar.projectBaseDir=C:\Projects\ovasave\httpdocs).
8) to downlaod the report of project , downlaod the CNES extension and paste it into sonar-cube->extensions->plugins and restart the sonar web-server than at web-server find the more section , there you'll find the option called CNES to download the report.


`reference : https://www.youtube.com/watch?v=bnIvlnu_YL0`
