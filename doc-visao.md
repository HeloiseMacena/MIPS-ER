

# Documento de Visão

### Histórico de Revisões

| Data                |  Versão             |          Descrição  |  Autores            |
| :-----------------: | :-----------------: | :-----------------: | :-----------------: |
| 07/12/2022 | 1.0 | Versão inicial |  Hilquias Abias |
| 11/04/2023 | 1.1 | Visão atualizada do projeto |  Hilquias Abias e Rafael Pessoa |
| 17/04/2023 | 1.2 | Visão atualizada do projeto |  Hilquias Abias, Rafael Pessoa, Daniela Faria |
| 03/07/2023 | 1.2 | Visão atualizada do projeto |  Rafael Pessoa |
| 31/01/2025 | 1.3 | Visão atualizada do projeto |  Heloise Macena |

<br>

## 1. Objetivo do Projeto:

O projeto **MipsCode** tem como objetivo desenvolver um website que ajude usuários a aprender a linguagem de programação MIPS Assembly, fornecendo um ambiente de desenvolvimento integrado (IDE) e simulador, sistema de arquivos para guardar os códigos, tutoriais e documentação da linguagem.

<br>

## 2. Descrição do problema:
| **Problema**            | Encontrar um site em português que ajude a aprendizagem da linguagem de baixo nível assembly, e que possua uma comunidade disposta e ativa para tirar eventuais dúvidas e compartilhar experiências.|
| --- | :---: |
| **Afeta**               | Os interessados em aprender e praticar código assembly da arquitetura MIPS. |  
| **Impacto**             | A falta de interesse em desenvolver em assembly, consequentemente uma falta de profissionais qualificados. |
| **Solução**             | O desenvolvimento de um site que estimule a aprendizagem e  aumente a produtividade de desenvolvedores de aplicações em Assembly para MIPS, já que eles terão acesso a uma ferramenta de desenvolvimento de fácil manuseio. Além disso, o projeto também beneficiará a comunidade de desenvolvedores, já que haverá uma interação maior entre a comunidade.|

<br>

## 3. Descrição dos usuários:

| **Nome** | **Descrição** | **Responsabilidade** |
| :---: | --- | --- |
| Estudante | Usuário logado que faz uso das funcionalidades do site. | - Acessar IDE. <br> - Acessar documentação. <br> - Acessar tutoriais.  <br> - Gerenciar projetos.  <br> - Exportar código. <br> - Importar código. |
| Professor | Usuário logado que faz uso das funcionalidades do site. | - Acessar IDE. <br> - Acessar documentação. <br> - Acessar tutoriais. <br> - Gerenciar projetos. <br> - Exportar código. <br> - Importar código. <br> - Gerenciar tutoriais. |
| Visitante | Usuário não logado que faz uso limitado do site. | - Acessar IDE. <br> - Acessar documentação. <br> - Fazer login. <br> - Cadastrar-se. |
| Administrador | Gerencia os usuários, tutoriais e faz uso das funcionalidades do site. | - Acessar IDE. <br>  - Acessar documentação. <br> - Acessar tutoriais. <br>  - Gerenciar projetos. <br>  - Exportar código. <br>  - Importar código. <br>  - Gerenciar tutoriais. <br>  - Gerenciar os usuários cadastrados. |

<br>

## 4. Descrição do ambiente dos usuários:
A aplicação será em forma de aplicação web, e será utilizada através de qualquer computador com acesso a internet. Contendo:
- IDE para codificação de mips assembly;
- Sistema de arquivos;
- Perfil do usuário;
- Área para tutoriais e guia de aprendizagem inicial de mips assembly;
- Link para comunidade externa;
- Área para entrar em contato com os desenvolvedores;
- Configurações da página (modo claro, modo escuro, tema personalizado...).

<br>

## 5. Principais necessidades dos usuários:
- Não encontra ambiente intuitivo para codificação de assembly mips;
- As IDEs e interpretadores disponíveis são pouco intuitivas ou estão em outro idioma;
- Possui dificuldade em achar uma comunidade envolvida e tão próxima ao ambiente de desenvolvimento.

<br>

## 6. Alternativas concorrentes:
Interpretadores e simuladores de assembly mips armazenados na internet.

<br>

## 7. Visão geral do produto:
- Possui IDE construída com linguagem de script vinculada ao próprio browser(javascript), no servidor do usuário mantendo agilidade e desempenho, e utiliza sistema de tratamento de erros bem adaptado;
- Mantém conexão com comunidade externa para interação dos usuários;
- A documentação vinculada torna desnecessário a busca por conteúdos de aprendizagem externos, pois ela conduz o usuário ao entendimento.

<br>

## 8. Fonte de requisitos:

MARS (MIPS Assembler and Runtime Simulator) como uma fonte de requisitos para o projeto. O MARS foi analisado para entender como ele oferece suporte à programação em MIPS Assembly, seu ambiente de desenvolvimento integrado (IDE), as funcionalidades de simulação e depuração.
<br>

## 9. Requisitos FUNCIONAIS:

| **Código** | **Nome** | **Descrição** | **Prioridade** |
| :---: | :---: | --- | --- |
| RF001 | Login | O usuário e visitante terão a opção de login disponibilizada de acordo com o nível de permissão do usuário. | Alta
| RF002 | Cadastro | O visitante terá acesso ao cadastro para o uso de mais funcionalidades do site. | Alta
| RF003 | Acessar documentação | O usuário/visitante deverá ter a disponibilização da IDE para uso. | Alta
| RF004 | Acessar IDE | O usuário/visitante irá acessar a área do site que possui a documentação do MIPS Assembly. | Alta
| RF005 | Contatar | Usuário e visitante poderão contatar a equipe desenvolvedora. | Média
| RF006 | Console decimal | Todos os usuários terão exibidos os valores dos registradores e do console. | Alta
| RF007 | Montar código | O usuário/visitante poderá realizar a compilação do código assembly | Alta
| RF008 | Voltar uma etapa | Todos os usuários podem retroceder uma linha da execução do código, manualmente. | Alta
| RF009 | Avançar uma etapa | Todos os usuários podem executar o código linha por linha manualmente. | Alta
| RF010 | Executar código | O usuário e visitante poderá executar o código completo após compilado. | Alta
| RF011 | Desmontar código | Usuário e Visitante poderão cancelar o processo de compilação do código assembly. | Alta
| RF012 | Visualizar registradores | Será disponibilizado para todos a visualização de registradores na versão mobile. | Média
| RF013 | Abrir console |Usuário e Visitante poderão abrir um console que mostra o resultado do código que já foi rodado na versão mobile. | Alta
| RF014 | Acessar dashboard | O usuário poderá entrar na área de apresentação das funcionalidades do sistema. | Alta
| RF015 | Filtrar projetos | O usuário poderá filtrar entre as opções dada pelo sistema os projetos solicitados. | Alta
| RF016 | Acessar tutoriais | O usuário poderá entrar na área de guia de aprendizagem. | Alta
| RF017 | Favoritar projetos | O usuário poderá favoritar um ou mais projetos para melhor identificação. | Baixa
| RF018 | Gerenciar perfil | O usuário poderá: Inserir, editar, excluir dados(bio, foto, e-mail, nome, github…) e mudar tema do site. | Média
| RF019 | Filtrar tutoriais | O usuário poderá: Filtrar entre as opções dada pelo sistema os tutoriais solicitados. | Alta
| RF020 | Acessar fórum externo | Acessar fórum da comunidade externa ao site. | Baixa
| RF021 | Exportar arquivo | Usuário e visitante poderão fazer download de arquivo de texto referente ao código. | Alta
| RF022 | Importar arquivo | Usuário e visitante poderão fazer o download do arquivo de texto referente ao código. | Alta
| RF023 | Manter Projeto | Apenas o usuário poderá Criar, editar, salvar e excluir projetos que sejam visíveis para os usuários. | Alta
| RF024 | Manter tutoriais | Apenas o usuário poderá Criar, editar, salvar e excluir tutoriais que sejam visíveis para os usuários. | Alta
| RF025 | Manter os usuários cadastrados | A administração deverá poder: Criar, editar, excluir, salvar e alterar permissão de acesso. | Alta

<br>

## 10. Requisitos NÃO FUNCIONAIS:

| **Código** | **Nome** | **Objetivo** | **Escala** | **Métrica** | **Mínimo** | **Intervalo OK** | **Ótimo** |
| :---: | :---: | --- | :---: | :---: | :---: | :---: | :---: |
| RNF001 | Tempo de Resposta | Garantir uma comunicação rápida entre o servidor e o cliente para otimizar a experiência do usuário. | Tempo decorrido em segundos | Medir o tempo entre a solicitação do usuário e a resposta do sistema na exportação | Menos de 5 segundos para pelo menos 95% dos casos | Entre 0,5 e 3 segundos para mais de 98% dos casos | Menos de 0,5 segundos para 100% dos usuários |
| RNF002 | Facilidade de uso | Fornecer uma interface amigável e intuitiva para melhorar a experiência do usuário | Avaliação qualitativa da usabilidade | Aplicar testes de usabilidade com os usuários e medir a facilidade de interação com o sistema | Pelo menos 80% dos usuários devem considerar a interface intuitiva | Entre 85% e 95% de aprovação pelos usuários | Mais de 95% dos usuários consideram a interface intuitiva |
| RNF003 | Manutenção e suporte da IDE | Garantir o funcionamento correto da IDE com um alto grau de impacto | Disponibilidade da IDE em porcentagem | Monitorar a disponibilidade e falhas da IDE por meio de logs e feedback dos usuários | 95% de disponibilidade mensal | Entre 97% e 99% de disponibilidade | 99,9% de disponibilidade |
| RNF004 | Monitorar os tutoriais | Assegurar que os tutoriais estejam atualizados, precisos e acessíveis aos usuários | Frequência de revisões e feedback dos usuários | Monitorar revisões de tutoriais e analisar feedback dos usuários | Revisão de tutoriais pelo menos a cada 6 meses | Revisão entre 3 e 6 meses | Revisão trimestral com mais de 90% de aprovação dos usuários |
| RNF005 | Requisitos legais | Adequar a plataforma às normas legais (LGPD), garantindo a segurança dos dados sensíveis | Conformidade com auditorias legais | Realização de auditorias de segurança e testes de conformidade com a LGPD | Atendimento de 90% dos requisitos legais em auditorias anuais | Atendimento entre 95% e 99% dos requisitos | Conformidade total com 100% dos requisitos legais |
| RNF006 | Disponibilidade de armazenamento de arquivos | Gerenciar o cache para armazenamento de arquivos locais com espelhamento interno | Tempo de resposta para recuperação de arquivos | Medir o tempo necessário para acessar arquivos armazenados em cache | Recuperação em menos de 10 segundos para 95% dos casos | Entre 3 e 7 segundos para mais de 98% dos casos | Menos de 3 segundos para 100% dos casos |
| RNF007 | Exportação de Arquivo | Disponibilizar o arquivo exportado em extensões ASM e XML | Disponibilidade das opções de exportação | Verificar se os formatos ASM e XML estão disponíveis na exportação | Disponibilidade de ambas as opções para 95% das exportações | Opções de exportação corretas em 98% dos casos | 100% de compatibilidade e disponibilidade nos dois formatos |
