snova-gae  Read Me
Release 2011/12/18
http://snova.googlecode.com 

This file is part of snova-gae.                                   
                                                                  
snova is free software: you can redistribute it and/or modify 
it under the terms of the GNU General Public License as           
published by the Free Software Foundation, either version 3 of the
License, or (at your option) any later version.                   
                                                                  
snova is distributed in the hope that it will be useful,      
but WITHOUT ANY WARRANTY; without even the implied warranty of    
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the     
GNU General Public License for more details.                      
                                                                  
You should have received a copy of the GNU General Public License 
along with snova(client & server & plugin).  If not, see <http://www.gnu.org/licenses/>.

Dependencies
------------
1. You need to install JRE/JDK(1.6+).
2. You need to install Google App Engine SDK(Java/GO) (use the latest version)

INSTALL:
GAE server part����GAE server���֣�
 1. unzip snova-gae-[g|j]server-[version].zip
    ����Ŀ¼�½�ѹsnova-gae-[g|j]server-[version].zip
 2. cd snova-gae-[g|j]server-[version] 
    �����ѹ��Ŀ¼
  ע�⣬Go/Javaֻ��Ҫ����һ�����ɣ�Go���ֲ���server��Ҫ��linux��ִ��
 3.For Java(jserver)
   modify war/WEB-INF/appengine-web.xml, change the element '<application>hyk-proxy-demo</application>'
       �޸�war/WEB-INF/appengine-web.xml�� ��'<application>'ֵ��Ϊ�Լ�������appid
 4. execute appcfg.cmd/appcfg.sh update war & appcfg.cmd/appcfg.sh backends update war(make sure you are in the directory 'snova-gae-jserver-[version]')
       ִ��appcfg.cmd/appcfg.sh update war�� appcfg.cmd/appcfg.sh backends update war�ϴ�
 5.For Go(gserver in linux)
   modify app.yaml, change the element 'application:<appid>'
       �޸�app.yaml�� ��'application:<appid>'ֵ��Ϊ�Լ�������appid
 6. execute appcfg.py update <dir> & appcfg.py backends update <dir>(make sure you are in the directory 'snova-gae-jserver-[version]')
       ִ��appcfg.py update <dir>�� appcfg.py backends update <dir>�ϴ�
 
    
Client part: ��Client���֣�
  1. cd snova-[version]/plugins/gae 
           ����snova gae plugin��Ŀ¼
  3. modify conf/gae-client.xml, refer the comment for more information
           ����ע���޸�conf/gae-client.xml
  4. execute <SNOVA_HOME>/bin/start.bat(start.sh) to start the local server
             ִ��<SNOVA_HOME>/bin/start.bat(start.sh)����local server

 
