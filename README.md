# festival

## Alterações/Correções feitas

Analisei o projeto e encontrei vários erros e partes incompletas que corrigi.

No ficheiro views.py, o import só tinha o modelo Palco, por isso adicionei Dia e Concerto que também eram necessários. A função concerto_view estava incompleta pois a variável concerto não tinha valor, corrigi para Concerto.objects.get(id=id). Também adicionei a palcos_view que estava completamente em falta apesar de existir uma rota para ela.

No ficheiro urls.py, faltava a rota para a página dos dias, por isso adicionei o path dias/ ligado à dias_view.

No template palcos.html, os links de cada concerto tinham o href vazio, corrigi para usar o url do concerto com o seu id.

Por fim, criei o ficheiro dias.html que não existia, apesar de ser necessário para a página dos dias funcionar.