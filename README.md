# ngrinder

ngrinder 컨트롤러를 먼저 실행시키고, agent를 실행

> #### ngrinder 실행  
> java -XX:MaxPermSize=200m -jar ngrinder-controller-3.5.3.war  
> java -XX:MaxPermSize=200m -jar ngrinder-controller-3.5.3.war -p 7777  // 이건 특정 포트 설정하고 싶을때....


> #### agent 실행 
> ./run_agent.sh



## 참고
> #### tar 분할 압축법  
> tar zcvf - ngrinder-controller-3.5.3.war | split -b 64m - ngrinder-controller-3.5.3.war.tar.gz   
> #### tar 분할 압축 해제  
> cat ngrinder-controller-3.5.3.war.tar.gz* | tar zxvf -  

