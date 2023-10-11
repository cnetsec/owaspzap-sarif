Execução do Owasp Zap:
owasp-zap -daemon -port 8080 -host localhost -quickurl http://testphp.vulnweb.com -quickout $(pwd)/results.json
<img width="958" alt="image" src="https://github.com/cnetsec/owaspzap-sarif/assets/86935257/3e837b89-a343-47a7-9b05-796a4da8e40e">


Conversão para resultado Sarif:
python owaspzap-sarif.py -J results.json
![image](https://github.com/cnetsec/owaspzap-sarif/assets/86935257/2f7892f8-935e-4cc4-bf1f-54e42d48b3ac)



