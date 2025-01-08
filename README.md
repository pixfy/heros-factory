# Desafio Fullstack - Kinebot

Antes de tudo, obrigado pelo o interesse em querer trabalhar conosco. O projeto visa avaliar habilidades técnicas  e desafios enfrentados no dia-a-dia. Logo abaixo você encontrará mais informações necessárias para o seu teste.


## Avisos importantes

-   Dê uma olhada com calma em tudo o que está escrito aqui e tente seguir as instruções o mais fielmente possível.
-   Crie um repositório no seu GitHub **sem mencionar o Kinebot em nenhum momento**.
-   Vá fazendo seus commits no repositório enquanto for avançando.
-   Depois, envie o link do seu repositório por e-mail para o recrutador responsável.
-   Fique à vontade para dar uma pesquisada no Google, Stack Overflow ou até no que você já tem de projeto na sua máquina.
-   Se pintar alguma dúvida, é só perguntar para os recrutadores. Estamos aqui para ajudar!
-   E lembre-se: sem pressa, respira tranquilo. Já passamos por essa etapa também. Boa sorte!

_Corpo do Email com o link do repositório do desafio_

> Seu Nome
> 
> Nome do recrutador
> 
> Link do repositório


### Sobre o ambiente da aplicação:

 - A aplicação deverá ser composta de uma API, Front-end e banco de dados.

#### Front-end
- Deve ser feito em ReactJS em qualquer framework.
- Usar Typescript é essencial.
- Sinta-se a vontade em usar qualquer biblioteca de componentes

 #### Back-end
 - Deve ser feito com NodeJS.
 - Pode ser feito em JS puro.
 - Pode utitlizar ORM ou raw queries.
 
 #### Banco de dados
 - Usar o MySQL em qualquer versão.
 
 **Observação**: O banco de dados deverá rodar em uma imagem Docker localmente.
 
### Apresentação do seu projeto
No dia da apresentação do seu projeto, tenha a aplicação rodando em sua máquina local para a execução de testes e possíveis questionamentos de como foi pensado e desenvolvido. Vamos fazer o code review juntos para você explicar como foi processo de criação e possíveis evoluções do projeto.

### Aplicação
A "**Hero Factory**" é uma plataforma de gestão de heróis. Nela podemos informar principais características e poderes do nosso herói. Nela é possível realizar a criação, listagem, updates e exclusão dos mesmos. 

#### Requisitos
A seguir estão algumas regras de negócio importantes para o funcionamento:

- A resposta da API para criação de herói deve seguir o seguinte padrão:
```json
{
	id: "e314636e-1ca6-4925-a0e7-da5eb5ae2403",
	name: "Robert Bruce Banner",
	nickname: "Hulk",
	date_of_birth: "1962-04-10 00:00:00",
	universe: "Marvel"
	main_power: "Force"
	avatar_url: "https://cdn.pixabay.com/photo/2024/05/07/00/59/hulk-8744607_1280.jpg",
	is_active: true,
	created_at: "2024-09-18 21:41:43",
	updated_at: "2024-09-18 21:41:43"
}
```
- As demais respostas da API devem seguir o modelo apresentado acima
- A listagem dos heróis já criados devem ser ordenados pela data de criação `created_at` (Os mais recentes primeiro).
- Registos inativos devem ter uma coloração "cinza" para diferenciar dos registros ativos
- Na lista cada registro deverá conter um botão de ações. Ao clicar deverá aparecer as seguintes opções: "Excluir", "Editar" ou "Ativar"
	- Ao clicar em "Editar" o usuário será redirecionado para a tela de edição
	- Ao clicar em "Excluir" deverá aparecer um modal de confirmação ao usuário
	- Caso o herói esteja desativado a opção ''Ativar" deve substituir a opção "Excluir", ao clicar deverá aparecer um modal de confirmação ao usuário
	- Qualquer interação de confirmação deverá atualizar a lista de heróis.
- Não é possível editar um herói desativado
- A tela inicial é a listagem dos heróis
- Todas as interações assíncronas deverão ter algum "Loading" na tela
- Todas as ações deveram ter mensagens de "erros" ou "sucesso" para o usuário
- Na tela de listagem deverá existir um campo de texto, que busque registros a partir do `name` ou `nickname`
- A lista de heróis deve ter paginação e retornar 10 registros por vez
- Na tela de edição deverá mostrar todos os dados do herói, porém, apenas os campos "Nome completo", "Nome de guerra", "Data de nascimento", "Universo", "Habilidade" e "Avatar" poderão ser editados
- Todos os serviços deveram ser RESTFul
- Não é necessário qualquer tipo de autenticação

## Avaliação
Apresente sua solução utilizando o framework que você desejar, justificando a escolha. Atente-se a cumprir a maioria dos requisitos, pois você pode cumprir-los parcialmente e durante a avaliação vamos bater um papo a respeito do que faltou.

## O que será avaliado e valorizamos

Habilidades básicas de criação de projetos backend:
-   Conhecimentos sobre REST
-   Uso do Git
-   Capacidade analítica
-   Apresentação de código limpo e organizado

Conhecimentos intermediários de construção de projetos manuteníveis:
-	Aplicação e conhecimentos de SOLID
-	Identificação e aplicação de Design Patterns
-	Conhecimentos sobre conceitos de containers (Docker)
-	Documentação e descrição de funcionalidades e manuseio do projeto
-	Implementação e conhecimentos sobre testes de unidade e integração
-	Identificar e propor melhorias

Aptidões para criar e manter aplicações de alta qualidade:
-	Aplicação de testes unitários
-	Boas noções de bancos de dados relacionais
-	Estrutura de pastas e nomes de arquivos

## O que será um Diferencial
-   Uma cobertura de testes consistente
-   Uso de Design Patterns
-   Documentação
-   Proposta de melhoria na arquitetura
-   Ser consistente e saber argumentar suas escolhas
-   Apresentar soluções que domina
-   Modelagem de Dados
-   Manutenibilidade do Código
