<h1>E o Oscar vai para... ?</h1>

Quantas vezes Natalie Portman foi indicada ao Oscar?

<strong>Comandos:</strong> <code>SELECT * from `oscar`WHERE `name` LIKE "Natalie Portman";</code>

<strong>Resultado:</strong> Natalie Portman, foi indicada 3 vezes ao Oscar

##

Quantos Oscars Natalie Portman ganhou?

<strong>Comandos:</strong> SELECT * FROM `oscar` WHERE `name` = "Natalie Portman"  AND `winner` = "true";</code>

<strong>Resultado:</strong>  Natalie Portman, foi premiada com apenas 1 Oscar

##

Amy Adams já ganhou algum Oscar?

<strong>Comandos:</strong> SELECT COUNT(*) FROM `oscar` WHERE name = "Amy Adams" AND winner = "true";</code>

<strong>Resultado:</strong> Amy Adams, foi premiada com 0 Oscar.

##

Alguém já ganhou um Oscar e tem o seu primeiro nome?

<strong>Comandos:</strong> <code>SELECT * FROM `oscar` WHERE name = "Cristian";</code>

<strong>Resultado:</strong> nome cristian, não foi encontrado como valor para a coluna "name".

##

Toy Story 3 ganhou um Oscar em quais anos?

<strong>Comandos:</strong> <code>SELECT (year_ceremony) FROM `oscar` WHERE film = "Toy Story 3" AND winner = "true";</code>

<strong>Resultado:</strong> Toy Story, foi contemplado com dois oscar em 2011, 1 ano ápos seu lançamemto. .




##


Quem tem mais Oscars: a categoria "Melhor Ator" ou "Melhor Filme"?

<strong>R:</strong> <code> SELECT COUNT(*) FROM `oscar` WHERE `name` AND winner ="true";</code>
  
<code> SELECT COUNT(*) FROM `oscar` WHERE `film` AND winner ="true";</code>
                    
 <strong>Resultado:</strong> melhor filme.
                    
 
  
##

Alguém já ganhou um Oscar e tem o seu primeiro nome?

  
  Na categoria Winner, altere todos os valores com "True" para 1 e todos os valores "False" para 0.
  UPDATE `oscar` SET `winner` = "1" WHERE winner like "%false%";
  UPDATE `oscar` SET `winner` = "0" WHERE winner like "%true%";
  
  Em qual edição do Oscar "Crash" ganhou o prêmio?
  SELECT * FROM `oscar` WHERE film like "%crash%" and winner like "%1%";
  2006
  
  Que filme merecia ganhar um Oscar e não ganhou?

R: Vingadores: Guerra Infinita! <code>(SELECT * FROM `oscar` WHERE film LIKE '%Avengers: Infinity War%')</code>
  
  Bom... dê um Oscar para esse filme, então.
  UPDATE `oscar` SET `winner`='1' WHERE film LIKE '%Avengers: Infinity War%';
  
  O filme Central do Brasil aparece no Oscar?
  SELECT * FROM `oscar` WHERE film like "%central do brasil%"
  não
  
  Inclua no banco 7 filmes que nunca nem foram nomeados ao Oscar, mas que na sua opinião, merecem.
  INSERT INTO `oscar`( `film`) VALUES (('O Grande Ditador '),('Cidadão Kane'),('Doze Homens e uma Sentença'),('Dr. Fantástico '),('A Primeira Noite de um Homem'),('Taxi Driver'),('Sociedade dos Poetas Mortos');
  
  Crie uma nova categoria de premiação. Qualquer prêmio que você queira dar. Agora vamos dar esses prêmios aos filmes que você cadastrou na questão acima.
  INSERT INTO `oscar`(`category`) VALUES ("choro noite")
 
 </ul>
