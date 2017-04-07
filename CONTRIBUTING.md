# <a name="contribute-to-microsoft-graph-documentation"></a>Contribua para a documentação do Microsoft Graph

Agradecemos seu interesse na documentação do Microsoft Graph!

* [Maneiras de contribuir](#ways-to-contribute)
* [Antes de podermos aceitar sua solicitação pull](#before-we-can-accept-your-pull-request)
* [Use o GitHub, o Git e este repositório](#use-github-git-and-this-repository)
* [Como usar o Markdown para formatar seu tópico](#how-to-use-markdown-to-format-your-topic)
* [Markdown-padrão](#standard-markdown)
* [Mais recursos](#more-resources)

## <a name="ways-to-contribute"></a>Maneiras de contribuir

Contribua para a [documentação do Microsoft Graph](http://graph.microsoft.io) dessas maneiras:

* Contribua com artigos por meio do [repositório de documentos do desenvolvedor do Microsoft Graph](https://github.com/microsoftgraph/microsoft-graph-docs)
    * Envie solicitações de pull separadas em ramificações /beta e/ou /v1.0. Essa etapa é necessária para garantir que as ramificações estão atualizadas até a data com as alterações mais recentes. 
    * Além disso, envie solicitações de recepção separada para/dominar ramificação. Esta etapa se presta a garantir que o site de documentação do site do Microsoft Graph faça as atualizações de acordo com as alterações mais recentes. 
* Relatar bugs na documentação via [Problemas no GitHub](https://github.com/microsoftgraph/microsoft-graph-docs/issues)
* Adicionar solicitações de documentação para o [UserVoice da Plataforma Office Developer](http://officespdev.uservoice.com)

##<a name="before-we-can-accept-your-pull-request"></a>Antes de podermos aceitar sua solicitação pull

###<a name="minor-corrections"></a>Correções secundárias

As correções ou os esclarecimentos secundários enviados para fins de documentação e exemplos de código neste repositório não exigem um Contrato de Licença de Contribuição (CLA). Os envios são recebidos na forma de solicitações pull. Faremos todo o possível para examinar as solicitações pull no período de dez dias úteis.


###<a name="larger-submissions"></a>Envios maiores

Se você enviar alterações novas ou significativas para a documentação e os exemplos de código, será necessário enviar-nos um Contrato de Licença de Contribuição (CLA) assinado antes que possamos aceitar sua solicitação pull caso você esteja em um desses grupos:

* Membros do grupo Microsoft Open Technologies
* Colaboradores que não trabalham na Microsoft

Como membro da comunidade, **você deve assinar o CLA (Contrato de Licença do Colaborador) antes de poder contribuir com envios volumosos para esse projeto**, mas é necessário completar e enviar a documentação uma única vez. Faça uma revisão cuidadosa do documento; talvez a assinatura de seu empregador também precise constar no documento.

A assinatura do Contrato de Licença de Contribuição (CLA) não lhe concede direitos para confirmar no repositório principal, mas isso significa que as equipes do Office Developer e do Office Developer Content Publishing serão capazes de analisar e considerar suas contribuições, e você receberá o crédito caso elas sejam aceitas.

Você pode baixar o Contrato de Licença de Contribuição (CLA) [aqui](https://github.com/microsoftgraph/microsoft-graph-docs/raw/master/Contribution%20License%20Agreement.pdf). Preencha o formulário e envie-o por email para [officedev@microsoft.com](mailto:officedev@microsoft.com).

Após recebermos e processarmos seu CLA, faremos todo o possível para analisar suas solicitações pull no prazo de dez dias úteis.

## <a name="use-github-git-and-this-repository"></a>Use o GitHub, o Git e este repositório

**Observação:** a maior parte das informações desta seção pode ser encontrada nos artigos da [Ajuda do GitHub] [].  Se você estiver familiarizado com Git e o GitHub, pule para a seção **Contribuir e editar conteúdo** para ver as informações específicas do fluxo de código/conteúdo deste repositório.

### <a name="setting-up-your-fork-of-the-repository"></a>Configurando sua bifurcação do repositório

1.    Configure uma conta GitHub para que você pode contribuir para esse projeto. Caso você ainda não tenha feito isso, acesse a [Página Inicial do GitHub] [] e faça isso agora.
2.    Configure seu computador com o Git. Siga as instruções no [Tutorial Configurando o Git] [Set Up Git].
3.    Crie sua própria bifurcação para este repositório. Para fazer isso, clique no botão **Bifurcação** localizado na parte superior da página.
4.    Copie sua bifurcação em sua máquina local. Para fazer isso, abra o GitBash. No prompt de comando, digite:

        git clone https://github.com/{seu nome de usuário}/microsoft-graph-docs.git

    Em seguida, crie uma referência para o repositório raiz inserindo esses comandos:

        cd microsoft-graph-docs   git remote add upstream https://github.com/microsoftgraph/microsoft-graph-docs.git   git fetch upstream

Parabéns! Agora seu repositório está configurado. Você não precisará repetir essas etapas novamente.

### <a name="contribute-and-edit-content"></a>Contribuir e editar o conteúdo

Para fazer com que o processo de contribuição se torne contínuo, siga este procedimento.

1. Crie uma nova ramificação.
2. Adicione novo conteúdo ou edite o conteúdo existente.
3. Envie uma solicitação pull para o repositório principal.
4. Exclua a ramificação.

Limite cada ramificação a um único conceito/artigo para simplificar o fluxo de trabalho e reduzir a chance de conflitos de mesclagem. Os seguintes tipos de contribuição são apropriados para uma nova ramificação:

* Um novo artigo (e imagens associadas)
* Edições de ortografia e gramática em um artigo
* Aplicar uma única alteração na formatação em um grande conjunto de artigos (por exemplo, aplicando um novo rodapé de direito autoral).

#### <a name="create-a-new-branch"></a>Criar uma nova ramificação

1.    Abra o GitBash.
2.    Digite `git pull upstream master:<new branch name>` no prompt. Isso cria uma nova ramificação local copiada da última ramificação-mestra do *microsoftgraph*. **Observação:** Para colaboradores internos, substitua o `master` no comando com a ramificação pela data de publicação que você estiver reproduzindo.
3.    Digite `git push origin <new branch name>` no prompt. Isso alertará GitHub para a nova ramificação. Agora você deverá surgir a nova ramificação na sua bifurcação do repositório no GitHub.
4.    Digite `git checkout <new branch name>` para alternar para sua nova ramificação.

#### <a name="add-new-content-or-edit-existing-content"></a>Adicionar novo conteúdo ou editar o conteúdo existente

Navegue até o repositório em sua máquina local usando o Explorador de Arquivos. Os arquivos do repositório estão no `C:\Users\<yourusername>\microsoft-graph-docs`.

Para editar arquivos, abra-os em um editor de sua escolha e modifique-os. Para criar um novo arquivo, use o editor de sua escolha e salve o novo arquivo no local apropriado em sua cópia local do repositório. Enquanto estiver trabalhando, certifique-se de salvar seu trabalho com frequência.

Os arquivos localizados no `C:\Users\<yourusername>\microsoft-graph-docs` são uma cópia de trabalho da ramificação nova que você criou em seu repositório local. Qualquer que seja a alteração você faça nessa pasta, ela só afetará o repositório local quando você confirmar uma alteração. Para confirmar uma alteração no repositório local, digite os seguintes comandos no GitBash:

    git add .
    git commit -v -a -m "<Describe the changes made in this commit>"

O comando `add` adiciona suas alterações para uma área de preparo em preparação para confirmá-las no repositório. O período posterior ao comando `add` especifica que você deseja preparar todos os arquivos adicionados ou modificados, verificando repetidamente as subpastas. (Caso você não queira confirmar todas as alterações, é possível adicionar arquivos específicos. Você também pode desfazer uma confirmação. Para ajuda, digite `git add -help` ou `git status`.)

O comando `commit` aplica as alterações em etapas no repositório. `-m` significa que você fornece o comentário de confirmação na linha de comando. Se você não estiver direcionando uma data específica para publicação, diga "para publicação o mais rápido possível".  As opções -v e -a podem ser omitidas. A opção -v corresponde à saída detalhada do comando, e a opção -a faz o que você já fez com o comando Adicionar.) 

Você pode confirmar várias vezes enquanto estiver fazendo seu trabalho, ou esperar e confirmar apenas uma vez quando terminar.

#### <a name="submit-a-pull-request-to-the-main-repository"></a>Enviar uma solicitação pull para o repositório principal.

Quando você terminar o trabalho e estiver pronto para mesclá-lo em um repositório central, siga estas etapas.

1.    No GitBash, digite `git push origin <new branch name>` no prompt de comando. Em seu repositório local, `origin` refere-se ao repositório do GitHub a partir do qual você clonou o repositório local. Esse comando coloca o estado atual do sua nova ramificação, incluindo todas as confirmações feitas nas etapas anteriores, na ramificação do GitHub.
2.    No site do GitHub, navegue em sua bifurcação para a nova ramificação.
3.    Clique no botão **Solicitação Pull** na parte superior da página.
4.    Certifique-se de que a Ramificação-base é `microsoftgraph/microsoft-graph-docs@master` e a Ramificação do cabeçalho da é `<your username>/microsoft-graph-docs@<branch name>`.
5.    Clique no botão **Atualizar o Intervalo de Confirmação**.
6.    Dê um título à sua solicitação pull e descreva todas as alterações que você estiver fazendo. Se seu bug corrigir um item do UserVoice ou um problema no GitHub, certifique-se de fazer referência a esse problema na descrição.
7.    Envie a solicitação pull.

Um dos administradores do site agora processará sua solicitação pull. Sua solicitação pull surgirá no site do microsoftgraph/microsoft-graph-docs em Problemas. Quando a solicitação pull for aceita, o problema será resolvido.

#### <a name="create-a-new-branch-after-merge"></a>Criar uma nova ramificação após a mesclagem

Depois que uma ramificação tiver sido mesclada com sucesso (por exemplo, sua solicitação for aceita), não continue a trabalhar na ramificação local que tiver sido mesclada a montante com êxito. Isso poderá gerar conflitos de mesclagem caso você envie outra solicitação pull. Em vez disso, se você quiser fazer outra atualização, crie uma nova ramificação upstream mesclada com êxito.

Por exemplo, suponha que sua ramificação local X tenha sido mesclada com êxito com o microsoftgraph/microsoft-graph-docs e você quiser fazer atualizações adicionais no conteúdo mesclado. Crie uma nova ramificação local, X2, da ramificação-mestra do microsoftgraph/microsoft-graph-docs. Para fazer isso, abra o GitBash e execute os seguintes comandos:

    cd microsoft-graph-docs
    git pull upstream master:X2
    git push origin X2

Agora você tem cópias locais (em uma nova ramificação local) do trabalho que você enviou na ramificação X. A ramificação X2 também contém todo o trabalho que outros autores mesclaram; portanto, se seu trabalho depende do trabalho de outras pessoas (por exemplo, imagens compartilhadas), ele estará disponível em nova ramificação. Você pode confirmar se seu trabalho anterior (e o trabalho de outras pessoas) está na ramificação verificando a nova ramificação...

    git checkout X2

... e verificando o conteúdo. (O comando `checkout` atualiza os arquivos no `C:\Users\<yourusername>\microsoft-graph-docs` para o estado atual da ramificação do X2.) Assim que você verificar a nova ramificação, será possível fazer atualizações no conteúdo e confirmá-las como de costume. No entanto, para evitar trabalhar na ramificação mesclada (X) por engano, o melhor a fazer será excluí-la (confira a seguinte seção: **Excluir uma ramificação**).

#### <a name="delete-a-branch"></a>Excluir uma ramificação

Depois que as alterações são mescladas com êxito no repositório central, você pode excluir a ramificação utilizada porque você não precisa mais dela.  Qualquer trabalho adicional exige uma nova ramificação.  

Para excluir sua ramificação, siga estas etapas:

1.    No GitBash, digite `git checkout master` no prompt de comando.  Isso garante que você não fique na ramificação a ser excluída (o que não é permitido).
2.    Em seguida, digite `git branch -d <branch name>` no prompt de comando.  Isso exclui a ramificação em sua máquina local somente se ela tiver sido mesclada com êxito no repositório upstream. (Você pode superar esse comportamento com o sinalizador `–D`, mas primeiro certifique-se de que você deseja fazer isso.)
3.    Por fim, digite `git push origin :<branch name>` no comando prompt (um espaço antes dos dois pontos e nenhum espaço depois deles).   Essa ação excluirá a ramificação em uma bifurcação do github.  

Parabéns, você tem contribuiu com êxito para o projeto.

## <a name="how-to-use-markdown-to-format-your-topic"></a>Como usar o Markdown para formatar seu tópico

### <a name="standard-markdown"></a>Markdown-padrão

Todos os artigos neste repositório usam Markdown.  Embora uma introdução completa (e a listagem de toda a sintaxe) podem ser encontradas em [Página Inicial de Markdown] [], falaremos sobre os conceitos básicos que você precisa conhecer.

Se você estiver procurando um editor bom editor, tente [Markdown Pad][].


### <a name="markdown-basics"></a>Noções básicas de markdown

Esta é uma lista com as ocorrências mais comuns para a sintaxe de markdown:

*     **Quebras de linha vs. parágrafos:** No markdown não há nenhum elemento de HTML `<br />`. Em vez disso, um novo parágrafo é indicado por uma linha vazia entre dois blocos de texto.
*    **Itálico:** O HTML `<i>some text</i>` é gravado em `*some text*`
*     **Negrito:** O elemento HTML `<strong>some text</strong>` é gravado em `**some text**`
*     **Cabeçalhos:** Os cabeçalhos HTML são designados por um número de caracteres `#` no início da linha.  A quantidade de caracteres `#` corresponde ao nível hierárquico do cabeçalho (por exemplo, `#` = h1, `##` = h2, e `###` = h3).
*     **Listas numeradas:** Para criar uma lista numerada (ordenada), inicie a linha com `1. `. Se você quiser vários elementos dentro de um elemento única da lista, formate sua lista da seguinte maneira:
        
        1.    Notice that this line is tabbed over after the '.'
        
            Now notice that there is a line break between the two paragraphs in the list element, and that the indentation here matches the indentation of the line above.

*    **Listas com marcadores:** Listas com marcadores (desordenadas) são praticamente idênticas às listas ordenadas em que `1. ` é substituído por `* `, `- ` ou `+ `.  As listas de elementos múltiplos funcionam da mesma maneira que as listas com ordenadas.
*    **Links:** A sintaxe básica para um link é `[visible link text](link url)`.

    Os links também podem ter referências, conforme se discute na seção **Link e referências de imagem** abaixo.

*    **Imagens:** A sintaxe básica de uma imagem é `![alt text for the image](image url)`.

    As imagens também podem ter referências, conforme se discute na seção **Link e referências de imagem** abaixo.

*    **HTML em linha:** O markdown permite que você inclua o HTML em linha: `<i>italic</i>` é renderizado corretamente por markdown como <i>itálico</i>.

### <a name="link-and-image-references"></a>Referências de link e de imagem

O markdown tem um recurso muito bonito que permite a um usuário inserir uma referência em vez de uma URL para imagens e links. Aqui está a sintaxe para usar este recurso:

    The image below is from [Google][googleweb]
    
    ![Google's logo][logo]
    
    [googleweb]: http://www.google.com
    [logo]: https://www.google.com/images/srpr/logo3w.png

Usando as referências agrupadas na parte inferior de seu arquivo, você encontrará com facilidade as URLs de link e de imagem, poderá editá-las e reutilizá-las. 


## <a name="more-resources"></a>Mais recursos

* Para saber mais sobre Markdown, acesse [seus sites][Página Inicial de Markdown].
* Para saber mais sobre como usar o Git e o GitHub, primeiro verifique a [seção Ajuda do GitHub] [Ajuda do GitHub] e, se for necessário, entre em contato com os administradores do site.

[Página inicial do GitHub]: http://github.com
[Ajuda do GitHub]: http://help.github.com/
[Set Up Git]: http://help.github.com/win-set-up-git/
[Página Inicial de Markdown]: http://daringfireball.net/projects/markdown/
[Teclado de markdown]: http://markdownpad.com/
[microsoftgraph/microsoft-graph-docs issues]: https://github.com/microsoftgraph/microsoft-graph-docs/issues
