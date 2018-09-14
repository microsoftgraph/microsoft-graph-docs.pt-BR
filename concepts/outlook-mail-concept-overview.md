# <a name="outlook-mail-api-overview"></a>Visão geral da API de email do Outlook

O Outlook é um hub de comunicação de mensagens do Office 365. Além disso, ele permite gerenciar contatos, agendar reuniões, saber mais sobre os usuários de uma organização, iniciar conversas online, compartilhar arquivos e colaborar em grupos.

## <a name="why-integrate-with-outlook-mail"></a>Por que integrar-se ao email do Outlook?

### <a name="integrate-with-rich-features-and-reach-hundreds-of-millions-of-customers"></a>Integrar recursos avançados e alcançar centenas de milhões de clientes

Integrar-se ao Outlook significa embarcar na experiência avançada que os clientes adoram, uma experiência consistente e intuitiva com emails, [contatos](outlook-contacts-concept-overview.md) e [calendário](outlook-calendar-concept-overview.md) que está disponível em todos os dispositivos: celular, web e desktop.

Ao usar o [Microsoft Graph](overview.md), você pode integrar-se ao Outlook escrevendo um aplicativo apenas uma vez e assim alcançar centenas de milhões de consumidores e dezenas de milhões de clientes empresariais que escolhem o Outlook como o cliente de email deles. Você pode escrever aplicativos que se concentrem em cenários de email ou que se conectem a uma grande variedade de outras inteligências, recursos e relações do Outlook ou fora dele, e criar cenários que têm suporte da nuvem da Microsoft.

### <a name="automate-message-organization-and-processing"></a>Automatizar o processamento e a organização de mensagens

Os clientes gostam da forma como o Outlook ajuda na organização. O Microsoft Graph leva esses recursos aos desenvolvedores de aplicativo, permitindo que eles criem fluxos de trabalho que otimizam a descoberta e melhoram a eficiência e a produtividade do cliente. 

- Os clientes costumam organizar suas mensagens de várias maneiras: alguns deixam todas as mensagens na Caixa de Entrada e simplesmente buscam por elas; outros arquivam suas mensagens em pastas. Essas pessoas gostam da abordagem flexível e intuitiva do Outlook que oferece suporte a essas duas organizações: simples e com pastas. Os aplicativos podem, de forma conveniente, [filtrar, buscar ou classificar](query_parameters.md) as mensagem em pastas específicas ou em toda a caixa de correio do usuário.

- As categorias do Outlook são diferenciadas por nome e cor. As categorias permitem aos clientes classificarem as mensagens para aumentar a organização e a descoberta. Os aplicativos podem acessar e [definir a lista de categorias mestra do usuário](../api-reference/v1.0/api/outlookuser_post_mastercategories.md). Além disso, essa lista é compartilhada entre mensagens do Outlook, assim como entre eventos, contatos, tarefas e postagens em grupo e ainda permitem cenários criativos para os desenvolvedores de aplicativo. Por exemplo, um provedor de treinamento online pode codificar por cor os emails, os eventos do curso e as atribuições de acompanhamento de cada curso que o usuário esteja inscrito.

- Além disso, os usuários do aplicativo podem alterar a prioridade de uma mensagem (evento ou tarefas) ou sinalizar uma mensagem para acompanhamento. (No momento, a sinalização está [no modo de visualização](versioning_and_support.md#beta-version) no Microsoft Graph).

- A API de regras transporta a organização de mensagens para um nível superior. Os aplicativos podem definir as [regras de Caixa de Entrada](../api-reference/v1.0/resources/messagerule.md) para tratar imediatamente as mensagens que chegam e reduzir emails secundários. Por exemplo, um aplicativo pode mover automaticamente as mensagens para outra pasta se as linhas do assunto contiverem determinadas palavras-chave e atribuir categorias e prioridades para facilitar o acompanhamento posterior.

### <a name="write-smarter-apps-that-leverage-intelligence"></a>Escrever aplicativos mais inteligentes que potencializam a inteligência 

Use o Microsoft Graph para sugerir dados contextuais aos usuários de seu aplicativo:

- Integrar-se a [Caixa de Entrada Destaques](../api-reference/v1.0/resources/manage_focused_inbox.md) e [menções @ (prévia)](../api-reference/beta/api/message_get.md#request-2) e permitir que os usuários de seu aplicativo leiam e respondam primeiro ao que é relevante para eles. 

- Verificar as [dicas de emails](../api-reference/v1.0/resources/mailtips.md) ao redigir uma mensagem para obter informações de status úteis sobre um destinatário (por exemplo, se o destinatário enviou uma resposta automática ou se a caixa de correio está cheia). As dicas de email podem alertar os aplicativos a respeito de determinadas condições para permitir que se tomem ações de acompanhamento mais eficientes. 

- Utilizar a [API de pessoas](people_example.md) para fornecer controles interativos, como o seletor de pessoas em seu aplicativo. A API de pessoas pode sugerir as pessoas mais relevantes para um usuário, tendo como base as comunicações, os padrões de colaboração e as relações comerciais desse usuário. 

- Oferecer aos usuários do aplicativo um seletor de arquivos inteligente e sugerir arquivos com os quais eles tenham interagido recentemente para serem adicionados como anexos quando estiverem escrevendo uma mensagem. Os [Insights (versão prévia)](../api-reference/beta/resources/insights.md) usam análise avançada para sugerir arquivos mais populares para um usuário, que tenham sido editados ou vistos pelo usuário, ou compartilhados recentemente com ele.


### <a name="store-app-data-in-a-resource-or-resource-instance"></a>Armazenar os dados do aplicativo em um recurso ou em uma instância do recurso

Muitas vezes os aplicativos precisam armazenar os dados em um repositório de dados externo e acarretam sobrecarga no gerenciamento e no acesso aos dados. O Microsoft Graph permite que você inclua dados de aplicativo como cabeçalhos de mensagem da internet ao [Criar](../api-reference/v1.0/api/user_post_messages.md#request-2) ou [enviar](../api-reference/v1.0/api/user_sendmail.md#request-2) uma nova mensagem ou uma resposta a uma mensagem. 

Se você precisar adicionar e subsequentemente atualizar dados personalizados, você pode [armazenar os dados em instâncias de recursos individuais](extensibility_overview.md#open-extensions). Se apropriado, como alternativa, você pode estender o esquema, adicionar propriedades personalizadas e armazenar dados digitados em recursos do Microsoft Graph. Você pode fazer com que essas [extensões de esquema](extensibility_overview.md#schema-extensions) sejam passíveis de ser descobertas e compartilhadas. 


## <a name="next-steps"></a>Próximas etapas

- Selecione e experimente as consultas de exemplos de email do Outlook no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages&version=v1.0). Escolha **Mostrar mais exemplos** na coluna à esquerda. Use o menu para habilitar o **Email do Outlook**.
- Saiba mais:

  - [Criar e enviar mensagens](outlook-create-send-messages.md)
  - Formas de [organizar mensagens](outlook-organize-messages.md)
  - Como [compartilhar pastas de mensagens](outlook-share-messages-folders.md)

- Saiba mais sobre como [usar a API de email](../api-reference/v1.0/resources/mail_api_overview.md) e seus [casos de uso](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) no Microsoft Graph v1.0.


