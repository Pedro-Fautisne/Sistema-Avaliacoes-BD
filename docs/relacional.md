- **Usuário** \= {E-mail, Nome, Idade, Gênero}  
- **Jogatina** \= {$\overline{\underline{Email\ do\ Usuário}}$, Jogo, Data}  \#Podemos fazer com que a data de uma instância apenas *atualize* a cada vez que o usuário joga o jogo novamente; serve para indicar quais usuários devem fazer quais avaliações  
- **Avaliação** \= {Código, Jogo Avaliado, Data de Avaliação, Descrição}  
- **Questão** \= {Enunciado, Tipo}  
- **Requisitado para Avaliar** \= {$\overline{\underline{Email\ do\ Avaliador}}$, $\overline{\underline{Código\ da\ Avaliação}}$, Anonimato}  \#As Avaliações que um Usuário recebe para responder são definidas pelas suas Jogatinas  
- **Questão em Avaliação** \= {$\overline{\underline{Enunciado\ da\ Questão}}$, $\overline{\underline{Código\ da\ Avaliação}}$}  
    
  \#Tipo da Questão Define em qual tabela a resposta vai  
- **Resposta Escala \=** {$\overline{\underline{Email\ do\ Avaliador}}$, $\overline{\underline{Código\ da\ Avaliação}}$, $\overline{\underline{Enunciado\ da\ Questão\ Respondida}}$, Resposta em Nota}  
- **Resposta Livre \=** {$\overline{\underline{Email\ do\ Avaliador}}$, $\overline{\underline{Código\ da\ Avaliação}}$,$\overline{\underline{Enunciado\ da\ Questão\ Respondida}}$, Resposta em Texto}

**O esquema está na 3FN,** pois não há tuplas espúrias (1FN), e também não há, em nenhuma das tabelas, atributos não primos que dependam de apenas parte da chave (2FN) ou de outros atributos primos (3FN).