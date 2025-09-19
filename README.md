🖥️ Comandos Úteis do Windows para Manutenção de Hardware 

Este guia reúne 20 comandos úteis do Windows que ajudam na manutenção, diagnóstico e reparo de hardware. Cada comando inclui um exemplo de uso, descrição da função e no final há um fluxo sugerido de diagnóstico. 

🔹 Comandos Principais 

chkdsk 

Exemplo: chkdsk C: /f /r 

Verifica erros no disco, corrige problemas e tenta recuperar setores defeituosos. 

sfc 

Exemplo: sfc /scannow 

Verifica e repara arquivos corrompidos do sistema. 

DISM 

Exemplo: DISM /Online /Cleanup-Image /RestoreHealth 

Repara a imagem do sistema quando o sfc não resolve. 

wmic diskdrive 

Exemplo: wmic diskdrive get status 

Mostra o estado (S.M.A.R.T.) dos discos instalados. 

driverquery 

Exemplo: driverquery /v /fo table 

Lista todos os drivers instalados, versão e status. 

powercfg 

Exemplo: powercfg /batteryreport 

Gera relatório detalhado sobre a bateria (para notebooks). 

tasklist 

Exemplo: tasklist 

Lista todos os processos em execução. 

taskkill 

Exemplo: taskkill /F /PID 1234 

Encerra um processo específico pelo PID. 

msinfo32 

Exemplo: msinfo32 

Abre informações detalhadas do sistema (hardware e software). 

dxdiag 

Exemplo: dxdiag 

Abre o diagnóstico do DirectX (placa de vídeo, áudio, drivers). 

perfmon 

Exemplo: perfmon /report 

Gera relatório de desempenho e saúde do sistema. 

systeminfo 

Exemplo: systeminfo 

Exibe informações completas do sistema, incluindo BIOS, memória e rede. 

ipconfig 

Exemplo: ipconfig /all 

Mostra configurações detalhadas de rede. 

ping 

Exemplo: ping 8.8.8.8 

Testa a conectividade com outro host ou servidor. 

tracert 

Exemplo: tracert www.google.com 

Mostra a rota que os pacotes fazem até o destino. 

netstat 

Exemplo: netstat -ano 

Exibe conexões de rede ativas e portas em uso. 

sc query 

Exemplo: sc query type= service 

Lista todos os serviços ativos no Windows. 

fsutil 

Exemplo: fsutil fsinfo drives 

Mostra informações sobre os volumes e sistemas de arquivos. 

diskpart 

Exemplo: diskpart → list disk 

Gerencia partições e discos (avançado, usar com cuidado). 

eventvwr 

Exemplo: eventvwr 

Abre o Visualizador de Eventos, útil para diagnosticar falhas de hardware e drivers. 

⚡ Extras Úteis 

resmon 

Exemplo: resmon 

Abre o Monitor de Recursos (CPU, RAM, Disco, Rede). 

getmac 

Exemplo: getmac 

Mostra o endereço MAC das interfaces de rede. 

bcdedit 

Exemplo: bcdedit /enum 

Mostra informações sobre o Boot Manager. 

shutdown 

Exemplo: shutdown /r /t 0 

Reinicia imediatamente o sistema. 

devmgmt.msc 

Exemplo: devmgmt.msc 

Abre o Gerenciador de Dispositivos. 

cleanmgr 

Exemplo: cleanmgr 

Abre a Limpeza de Disco. 

🛠️ Fluxo Sugerido de Diagnóstico 

1. Verificar disco e integridade do sistema 

chkdsk C: /f /r 

sfc /scannow 

DISM /Online /Cleanup-Image /RestoreHealth 

2. Checar drivers e hardware 

driverquery /v /fo table 

msinfo32 

devmgmt.msc 

3. Analisar desempenho e gargalos 

tasklist 

taskkill 

resmon 

perfmon /report 

4. Diagnóstico de rede 

ipconfig /all 

ping 8.8.8.8 

tracert www.google.com 

netstat -ano 

5. Conferir logs e eventos do sistema 

eventvwr 

bcdedit /enum 

6. Ações corretivas 

shutdown /r /t 0 

cleanmgr # Criando-seu-Primeiro-Projeto-111
