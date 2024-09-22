# Cadastro-de-alunos
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Projeto Carômetro

Carômetro é um aplicativo para desktop (Windows, Linux ou MAC) de repositório de informações de pessoas com uma foto associada. Neste exemplo um carômetro de alunos, porém você pode reutilizar este projeto e criar um repositório de imagens de uma equipe, candidatos, jogadores de futebol etc.

 <img width=60% src="https://github.com/Lucasbarbosa332/Cadastro-de-alunos-/blob/main/Cronometo/java%20and%20Mysql/assets/caraometro1.png?raw=true"></img>

# Pré requisitos
1.Ter o Java versão 17 ou superior instalado. Testado com a versão openJDK 21 LTS que pode ser obtida no link indicado. Na instalação, selecione todos os recursos conforme indicado na imagem.

 <img width=60% src="https://github.com/Lucasbarbosa332/Cadastro-de-alunos-/blob/main/Cronometo/java%20and%20Mysql/assets/openjdk.png?raw=true"></img>

2.Ter um banco de dados local baseado no MySQL 8 ou MariaDB compatível, no exemplo usei o XAMPP que pode ser obtido no link indicado.

#Instalação do banco

1.Iniciar os serviços Apache e MySQL no XAMPP, conforme indicado na imagem.
 
 <img width=60% src=""></img>

2.No navegador de internet digite: localhost/dashboard e selecione no menu: phpMyAdmin conforme indicado na imagem.

 <img width=60% src=""></img>

3.Crie um novo banco de dados de nome dbcarometro (sem usar acentuação) conforme indicado na imagem.

 <img width=60% src=""></img>

4.Na aba SQL, copie e cole o código abaixo e execute. (Passos 1,2 e 3 indicados na imagem)
      
       CREATE TABLE alunos (ra int PRIMARY KEY AUTO_INCREMENT,nome varchar(30) NOT NULL,foto LONGBLOB NOT NULL);

 <img width=60% src=""></img>

# Instalação do aplicativo

1.Em Releases faça o download do arquivo carometro.jar

2.Execute e verifique no rodapé o ícone que representa o banco de dados conectado. Se estiver com erro (conforme indicado na figura), verifique o XAMPP e revise novamente os passos 1 a 4 da instalação do banco.

 <img width=60% src=""></img>

3.Se tudo estiver OK ( 1 ) você pode iniciar gerando uma listagem dos alunos cadastrados ( 2 ) ou pesquisar um aluno pelo RA ou Nome ( 3 ), neste caso o aplicativo libera os botões e recursos de acordo com o resultado da pesquisa, por exemplo, se não tiver um aluno cadastrado, ele libera os botões para carregar foto e adicionar e se existir um aluno cadastrado, ele traz todas as informações e libera os botões para editar e excluir.

 <img width=60% src=""></img>


# Tecnologias que são abordadas neste Projeto :

* Criação de banco de dados e tabelas no MySQL
* CRUD (Criar, Ler, Atualizar e Excluir)
* IDE Eclipse
* Java SE
* Construtor de janelas
* JDBC (conectividade de banco de dados Java)
* Validação de dados
* Uso da biblioteca iTextpdf para gerar listagem de alunos com foto
