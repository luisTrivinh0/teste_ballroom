### Teste de desenvolvimento Ballroom 2023
### Respostas de Luís Henrique Felix Trivinho

- __Situação 1__ - Receber o comprovante do pagamento feito por parte do cliente, que foi gerado na hora do pagamento, para resolução do problema

- __Situação 2__ - O e-mail raphaella9@gmail.com está registrado na tabela history_emails_blacklist, que, consultada pela função check_blacklist(), evita que o e-mail receba os envios

- __Situação 3__ - Dadas as circunstâncias, a forma correta de realocá-la seria direto pelo sistema, alterando o cadastro. Todavia, é possível copiar a linha do seu cadastro na tabela clientes da Company 1 e passá-la para a Company 2, verificando também as foreign keys existentes e realocando igualmente direto pelo MySQL para resolução do problema.

- __Situação 4__- SELECT concat_ws(' - ', l.user_id, l.username) as 'Usuário'
                  	   , l.action as 'Action'
                       , l.json_old -> Tratado no front-end
                       , l.json_new -> Tratado no front-end
                       , l.json_changed -> Tratado no front-end
                    FROM logs l
                   WHERE l.main_table = '$select_main_tables'
                     AND (l.user_id like '%$input_text_usuario%'
                  	     OR l.user_name like '%$input_text_usuario%')
                     AND l.action = '$select_actions';

- __Situação 5__ - A princípio, não foi encontrado nenhum erro para verificar o login, todavia, usario sistema de reCaptcha (https://www.google.com/recaptcha/about/) para autenticar e previnir fraudes e abusos

- __Situação 6__ - É de conhecimento geral que features que envolvem SMS tem custo adicional que pode ou não estar planejado pelo cliente. Esse custo adicional é cobrado por terceiros, que por maioria, disponibilizam APIs pagas para fazê-lo. Comunicando isso ao cliente e dando prosseguimento, uma pesquisa dos melhore serviços e dos melhores preços seria passa ao cliente, que provavelmente arcaria com os custos (dependendo do contrato que fora feito). Caso os custos sejam da Ballroom, recomendaria um terceiro que preze por facilitadores para uso futuro, como por exemplo, acompanhar boa performance com alta de uso.

- __Bônus__ - Os projetos 1-1 são projetos em que não há outros clientes com registro em clientes.projeto_id, diferente dos 1-n, que há mais clientes com clientes.projeto_id com o ID vinculado