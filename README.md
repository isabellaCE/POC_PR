🎯 Objetivo da POC
Esta Prova de Conceito (POC) foi criada para demonstrar os benefícios e a viabilidade da implementação de templates de Pull Request (PR) em nossos projetos. Nosso objetivo é padronizar a criação de PRs, garantindo que todas as informações essenciais estejam presentes, o que pode levar a:

-Melhoria na Qualidade dos PRs: Menos informações faltantes, resultando em PRs mais completos e fáceis de entender.

-Agilidade nas Revisões de Código: Revisores terão um contexto claro e todos os dados necessários, reduzindo o tempo gasto em perguntas e idas e vindas.

-Consistência e Padronização: Estabelecer um formato unificado para todos os PRs, facilitando a navegação e a leitura.

-Redução de Erros: Menos chances de esquecer pontos importantes, como testes ou atualização de documentação.

⚙️ Como a POC Foi Conduzida
Repositório de Teste
Esta POC foi executada neste próprio repositório (ou em um repositório dedicado de testes). Ele contém uma estrutura mínima de arquivos para simular um projeto real, permitindo a criação de PRs de exemplo.

Templates Desenvolvidos
Foram criados os seguintes templates de PR para esta POC:

feature.md: Um template específico para a adição de novas funcionalidades, com seções dedicadas a Visão Geral, Mudanças Propostas, Como Testar, etc.

bugfix.md: Um template específico para a correção de bugs, focando em Descrição do Bug, Solução Proposta e Causa Raiz.

Os templates estão localizados na pasta .github/PULL_REQUEST_TEMPLATE/ na raiz deste repositório, seguindo as convenções do GitHub.

▶️ Como Testar (Simular a Criação de um PR)
Para ver os templates em ação, siga os passos abaixo:

Clone este repositório:

Bash

git clone [URL_DO_SEU_REPOSITORIO]
cd [nome-do-repositorio]
Crie uma nova branch de trabalho:

Bash

git checkout -b minha-nova-feature-ou-bugfix
Faça uma alteração qualquer:

Crie um novo arquivo ou modifique um existente (ex: echo "Hello POC" >> test.txt).

Adicione e commite suas mudanças:

Bash

git add .
git commit -m "feat: Adicionando arquivo de teste para POC"
Envie sua branch para o repositório remoto:

Bash

git push origin minha-nova-feature-ou-bugfix
Abra um Pull Request:

Vá até a interface web do GitHub (ou sua plataforma).

Você verá um prompt para abrir um PR da branch minha-nova-feature-ou-bugfix para main (ou master).

Ao criar o PR, você deverá ver a opção de selecionar um dos templates que foram configurados. Escolha entre Nova Funcionalidade ou Correção de Bug, dependendo do cenário que você quer simular.

Observe como o corpo do PR é automaticamente preenchido com a estrutura do template escolhido.

✔️ Resultados da POC e Próximos Passos
Durante esta POC, observamos que:

A criação de PRs se tornou mais intuitiva e guiada, com campos específicos para cada tipo de mudança.

As informações cruciais (como "Como Testar" e "Issue Relacionada") são solicitadas explicitamente, garantindo que o desenvolvedor as inclua.

A padronização visual dos PRs melhora a experiência do revisor.

Templates específicos para features e bugs garantem que o contexto correto seja fornecido para cada cenário.

Conclusão e Recomendação
Esta POC demonstrou que a implementação de templates de PR é viável e altamente benéfica para o nosso fluxo de trabalho. Acreditamos que a adoção desses templates em nossos repositórios de produção trará melhorias significativas na qualidade do código, na eficiência das revisões e na comunicação da equipe.

Próximos Passos Sugeridos
Refinamento dos Templates: Com base no feedback da POC, ajustar e otimizar os templates existentes.

Documentação Interna: Criar uma breve documentação para a equipe sobre como usar e aproveitar ao máximo os templates de PR.

Implementação em Projetos Piloto: Adicionar os templates a um ou dois projetos-piloto para uma adoção controlada e coleta de feedback em um ambiente mais real.

Treinamento/Apresentação: Realizar uma breve sessão para a equipe para apresentar os templates e seus benefícios.