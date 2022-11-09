# bot_googleforms
Script para 'automatizar' uma tarefa de responder a formulários do google de forma randomica


Usando a Biblioteca Selenium que permite com que eu abra o navegador atráves do python, de forma simples consegui reaizar em poucos segundos uma tarefa que levaria horas para ficar pronta se tivesse de fazê-la manualmente.

Na linha 1 faço a importação do WebDriver da lib Selenium, para que eu consiga abrir o navegador
Na linha 2 faço a importação da lib random que utilizo para gerar respostas aleatórias dentro do formulário
Na linha 3 defino o meu webdriver, que no meu caso é o Chrome

Nas linhas 4, 5, 6 e 7 vou definir o xpath de cada resposta possível em cada pergunta do meu formulário de exemplo

Então inicio o meu loop for e difinio quantas vezes eu quero que meu formulário seja respondido

Nas linhas 9, 10, 11 e 12 utilizo o random.choice() para que ele selecione de forma aleatória um xpath pra cada pergunto e atribua na respectiva variavel

Na linha 13 uso o .get para abrir o link do meu formulário

Nas linhas 14, 15, 16 e 17 encontro o elemento na página que selecionará minha resposta utilizando o xpath e finalizanod com o .click() para ele executar a ação de clicar na resposta

Na linha 18 utilizo a função .click() para estar enviando o meu formulário
