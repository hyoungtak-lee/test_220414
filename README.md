=======================================
========반드시 읽고 실행해주세요========
=======================================

D:\workspace이름\.metadata\.plugins\org.eclipse.wst.server.core\tmp0\wtpwebapps\LifeBook2
위 경로에
book_imgs
boardUpload
폴더를 추가해주세요(웹에서 업로드한 파일과 이미지가 들어가는 폴더입니다.)

Server.xml 파일의 Host태그 안쪽 제일 아래에
<Context docBase="LifeBook2" path="/LifeBook2" reloadable="true" source="org.eclipse.jst.jee.server:LifeBook2">
	<Resource auth="Container" driverClassName="oracle.jdbc.OracleDriver" maxActive="100" maxIdle="30" maxWait="10000" name="jdbc/oracle" password="1234" type="javax.sql.DataSource" url="jdbc:oracle:thin:@localhost:1521:xe" username="lifebook"/>
</Context>
위 코드를 넣어주세요.

D:\java\pp\db
위 경로를 생성해주세요.(테이블 스페이스 생성 경로)

이후 SQL Developer를 실행한 후
System계정에서 CreateUserLifeBook.sql 스크립트,
생성된 lifebook 계정에서 CreateTableAndView.sql 스크립트를 각각 실행해주신 후

main/main.jsp에서 파일을 실행해 주세요.