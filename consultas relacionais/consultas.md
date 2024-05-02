desafio concluido


select nome, ano from filmes

select nome, ano from filmes
order by ano

select * from filmes
where nome = 'de volta para o futuro'
order by ano,duracao

select * from filmes
where ano = 1997


select * from filmes
where ano  > 2000
 

 select * from filmes
 where duracao > 100 and duracao < 150
 order by duracao

 select ano,count(ano)quantidade from filmes
 group by ano
 order by quantidade desc

 select PrimeiroNome,UltimoNome, genero from atores
 where genero = 'M'


select PrimeiroNome,UltimoNome, genero from atores
 where genero = 'F'
 ORDER BY PrimeiroNome


select Filmes.nome , Generos.genero from filmesgenero
join Filmes on filmesgenero.idfilme = filmes.id
join generos on filmesgenero.idgenero = generos.id



select Filmes.nome , Generos.genero from filmesgenero
join Filmes on filmesgenero.idfilme = filmes.id
join generos on filmesgenero.idgenero = generos.id
where Generos.genero = 'mistério'


 

 
 
select Filmes.nome , atores.PrimeiroNome, atores.UltimoNome , ElencoFilme.Papel from filmes
join ElencoFilme on filmes.Id = ElencoFilme.IdFilme
join atores on atores.Id = ElencoFilme.IdAtor