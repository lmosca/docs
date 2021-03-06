{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:download: .download}
{:pre: .pre}
{:app_name: data-hd-keyref="app_name"}
{:app_key: data-hd-keyref="app_key"}
{:app_secret: data-hd-keyref="app_secret"}
{:app_url: data-hd-keyref="app_url"}
{:host: data-hd-keyref="host"}
{:org_name: data-hd-keyref="org_name"}
{:route: data-hd-keyref="route"}
{:space_name: data-hd-keyref="space_name"}
{:service_name: data-hd-keyref="service_name"}
{:service_instance_name: data-hd-keyref="service_instance_name"}
{:user_ID: data-hd-keyref="user_ID"}

# Cloud Foundry 명령행 인터페이스로 앱 배치
*마지막 업데이트 날짜: 2015년 11월 11일*

Cloud Foundry 명령행 인터페이스를 사용하여 애플리케이션 및 서비스 인스턴스를 배치하고 수정할 수 있습니다.{:shortdesc}

시작하기 전에 cf 명령행 인터페이스를 설치하십시오.

<p>
<a class="xref" href="https://github.com/cloudfoundry/cli/releases" target="_blank" title="(새 탭 또는 창에서 열림)"><img class="image" src="images/btn_cf_commandline.svg" alt="Cloud Foundry 명령행 인터페이스 다운로드" /> </a>
</p>

**제한사항:** Cloud Foundry 명령행 인터페이스는
Cygwin에서는 지원되지 않습니다. Cygwin 명령행 창 외의
명령행 창에서 Cloud Foundry 명령행 인터페이스를 사용하십시오.

cf 명령행 인터페이스가 설치된 후 시작할 수 있습니다.

  1. 스타터 코드를 다운로드하십시오.
  
    <p>
    <a class="xref" href="http://bluemix.net" target="_blank" title="(새 탭 또는 창에서 열림)"><img class="image" src="images/btn_starter-code.svg" alt="스타터 코드 다운로드" /> </a>
    </p>
  
  {:download}
  2. 패키지를 새 디렉토리로 추출하여 개발 환경을 설정하십시오.
  3. 새 디렉토리로 변경하십시오.
  
  <pre class="pre">cd <var class="keyword varname">your_new_directory</var></pre>
  
  4. {{site.data.keyword.Bluemix}}에 연결하십시오.
  
  <pre class="pre">cf api https://api.<span class="keyword" data-hd-keyref="DomainName">DomainName</span></pre>
  
  5. {{site.data.keyword.Bluemix_notm}}에 로그인하십시오.
 
  <pre class="pre">cf login -u <var class="keyword varname" data-hd-keyref="user_ID">username</var> -o <var class="keyword varname" data-hd-keyref="org_name">org_name</var> -s <var class="keyword varname" data-hd-keyref="space_name">space_name</var></pre>
  
  6. 앱을 {{site.data.keyword.Bluemix_notm}}에 배치하십시오. cf push 명령에 대한 자세한 정보는
[애플리케이션 업로드](upload_app.html#upload_app__push)를 참조하십시오.
  
  <pre class="pre">cf push <var class="keyword varname" data-hd-keyref="app_name">app_name</var></pre>
  
  7. 브라우저에 다음 URL을 입력하여 앱에 액세스하십시오. 
  
  <pre class="codeblock"><code><var class="keyword varname" data-hd-keyref="host">host</var>.<span class="keyword" data-hd-keyref="APPDomain">AppDomainName</span></code></pre>
