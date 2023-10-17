# Teste de mudança
Sistema de Biblioteca Avançado: 

Descrição do Projeto:  

As bibliotecas da universidade precisam de um sistema que controle o estoque de livros, permita consulta de títulos, gerencie multas, atrasos de devolução e envie notificações sobre devoluções. É necessário que o sistema seja de fácil implementação, eficiente, tenha interface intuitiva e que incorpore os princípios de programação orientada a objetos. 

Requisitos de Projeto: 

Sistema para Bibliotecários: 

O sistema precisa ser capaz de procurar títulos de livro no estoque, editar o acervo, editar cadastros de alunos (adicionar, remover e alterar dados), registrar empréstimos e devoluções. 

Sistema para Alunos: 

A implementação terá que realizar a busca de títulos no acervo, consultar a situação de empréstimos do usuário (calcular multa e acessar o histórico de livros emprestados) e acessar seus dados. 

Levantamento de requisitos: 

Requisitos funcionais: 

O sistema deve atender alunos e bibliotecários, cada um com sua devida finalidade e funcionalidade. 

Controle do acervo (consulta, possibilidade de adicionar ou remover livros). 

Calcular multas. 

Registrar empréstimos e devoluções. 

Enviar notificações sobre atrasos de devoluções. 

Consultar dados de usuários. 

Requisitos não funcionais: 

Interface intuitiva. 

Código bem documentado e organizado. 

Modelagem básica do sistema: 

Terão duas classes principais: Alunos e Bibliotecário. 

Classe Alunos: 

Atributos: 

Pessoa (): Struct que identifica o usuário (nome, telefone, login, senha, email, matrícula).

Situação (): Situação do empréstimo, acusa qualquer pendência e/ou multa. 

Métodos: 

ConsultarDados: Permite que o aluno veja seus dados cadastrados (nome, telefone, login, senha, email, matrícula).

ProcurarLivros (PorNome, PorAutor, PorEditora, DetalhesLivro) 

ConsultarSituacao (CalcularMulta, LivrosEmprestados, HistoricoEmprestimos)  

 

Classe Bibliotecário: 

Atributos: 

Pessoa (): Struct que identifica o usuário (nome, telefone, login, senha, email, matrícula).

Métodos: 
ProcurarLivro (PorTitulo, PorAutor, PorEditora, DetalhesLivro) 

EditarAcervo (AdicionarLivro, RemoverLivro, EditarLivro (EditarTitulo, EditarAutor, EditarEditora, EditarDetalhes)) 

EditarCadastros (AdicionarPessoa, RemoverPessoa, EditarPessoa (EditarNome, EditarSenha, EditarEmail, EditarMatricula)) 

Emprestar (ConsultarSituacao, ProcurarLivro (PorNome, PorAutor, PorEditora, DetalhesLivro), EmprestarLivro) 

Devolver (ConsultarSituacao, ProcurarLivro (PorNome, PorAutor, PorEditora, DetalhesLivro), CalcularMulta, ReceberLivro) 
