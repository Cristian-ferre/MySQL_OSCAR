<h1>E o Oscar vai para... ?</h1>

<ul> 
  <li>
  <h2>Quem tem mais Oscars: a categoria "Melhor Ator" ou "Melhor Filme"?</h2>
  <p> R:  SELECT * FROM `oscar` WHERE category like "%best pictures%"</p>
  </li>
  
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
