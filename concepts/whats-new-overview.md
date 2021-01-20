---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 9d041944b65949564ade9f1fc4bfc12d5e69519f
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910756"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use os recursos de visualização em aplicativos de produção.


## <a name="january-2021-new-in-preview-only"></a>Janeiro de 2021: novo apenas em pré-visualização

### <a name="cloud-communications"></a>Comunicações na nuvem
- Organize um evento ao vivo como uma [reuniãoOnline ](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) - veja um [exemplo](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true#example-3-create-a-live-event-with-a-user-token). 
- Obtenha o fluxo de conteúdo de um [relatório de participante](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-4-retrieve-the-attendee-report-of-a-live-event), [gravação](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-5-retrieve-the-recording-of-a-live-event) ou gravação alternativa do evento ao vivo.
- Obtenha o status de [presença](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true) de um usuário que está [fora do escritório](/graph/api/resources/outofofficesettings?view=graph-rest-beta&preserve-view=true) e qualquer mensagem definida para esse status.

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Cloud PC
- [Atualize uma senha de domínio do Active Directory ](/graph/api/cloudpconpremisesconnection-updateaddomainpassword?view=graph-rest-beta&preserve-view=true) para uma [conexão de rede local bem-sucedida](/graph/api/resources/cloudPcOnPremisesConnection?view=graph-rest-beta&preserve-view=true).
- [Executar verificações de integridade em uma conexão de rede local](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) agora pode expor 5 tipos de erros adicionais no recurso de [verificação de integridade da conexão local](/graph/api/resources/cloudpconpremisesconnectionhealthcheck?view=graph-rest-beta&preserve-view=true). Para obter mais informações sobre os tipos de erro, confira o [log de mudanças](https://developer.microsoft.com/graph/changelog) de janeiro de 2021.

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
Use permissões delegadas em aplicativos em nome do usuário conectado:
- `PrinterShare.ReadBasic.All` para ler informações básicas sobre compartilhamentos de impressoras, excluindo informações de controle de acesso.
- `PrintConnector.Read.All` para ler conectores de impressão.
- `PrintConnector.ReadWrite.All` para ler ou gravar conectores de impressão.
- `PrintJob.Create` para criar trabalhos de impressão e fazer upload de conteúdo para trabalhos de impressão.
- `PrintSettings.Read.All` para ler as configurações de impressão de todo o locatário.
- `PrintSettings.ReadWrite.All` para ler ou gravar configurações de impressão para todo o locatário.
- `Reports.Read.All` para ler o resumo do uso de impressão por usuário especificado ou por impressora.

### <a name="groups"></a>Grupos
Obtenha o status de processamento de um grupo dinâmico baseado em regras usando a propriedade **membershipRuleProcessingStatus**. Isso é útil quando um atributo de um usuário é alterado, a associação do usuário em um [grupo Microsoft 365](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) baseado em regras é reavaliada com base nas regras de associação de grupo definidas para a organização. 

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
- Os aplicativos podem usar as permissões do aplicativo para permitir que os administradores gerenciem os [métodos de autenticação](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true) dos usuários.
- Suporte ao [Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethod?view=graph-rest-beta&preserve-view=true) como um método de autenticação de um usuário para entrar ou executar autenticação multifator no Azure Active Directory.
- Use a [política do Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true) para definir as configurações e usuários ou grupos que podem usar o Microsoft Authenticator como método de autenticação. Use a política do Microsoft Authenticator no lugar da [política de login por telefone sem senha do Microsoft Authenticator](/graph/api/resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true), que está obsoleta. 
- Ofereça suporte ao [Windows Hello para Empresas](/graph/api/resources/windowshelloforbusinessauthenticationmethod?view=graph-rest-beta&preserve-view=true) como um método de autenticação para um usuário entrar em dispositivos Windows sem usar uma senha.

## <a name="december-2020-new-and-generally-available"></a>Dezembro de 2020: Novo e disponível para o público geral

### <a name="calendar"></a>Calendário
- Os organizadores da reunião podem usar a propriedade **hideAttendees** de um [evento](/graph/api/resources/event) para controlar se os participantes podem ver uns aos outros na lista de **acompanhamento** da reunião.
- GA da propriedade **isDraft** e método de [cancelamento](/graph/api/event-cancel) que estão disponíveis para os organizadores e o método de [encaminhamento](/graph/api/event-forward) disponível para organizadores e participantes para gerenciar melhor os recursos do [evento](/graph/api/resources/event) em um calendário.
- GA das propriedades **hexColor** e **isDefault** de um [calendário](/graph/api/resources/calendar) para gerenciar melhor os calendários.

### <a name="cloud-communications"></a>Comunicações na nuvem
GA do recurso de [presença](/graph/api/resources/presence), permitindo obter a presença de um ou mais usuários, como disponibilidade e atividade do usuário.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
Experimente um novo [tutorial](tutorial-riskdetection-api.md) para aprender como usar a [API de proteção de identidade](/graph/api/resources/identityprotectionroot) para identificar o risco e configurar um fluxo de trabalho para confirmar o comprometimento ou habilitar a correção.

### <a name="teamwork"></a>Trabalho em equipe
- GA da [API para gerenciar a instalação do aplicativo Teams](/graph/api/resources/teamsappinstallation), incluindo a instalação de aplicativos ou a adição, a remoção ou a atualização do aplicativo em uma equipe ou no escopo pessoal de um usuário.
- [Obtenha um chat entre um usuário e um aplicativo do Teams](/graph/api/userscopeteamsappinstallation-get-chat).

### <a name="use-the-toolkit"></a>Usar o kit de ferramentas
GA do Kit de ferramentas do Microsoft Graph 2.0 - esta versão inclui um novo [componente para Tarefas Pendentes do Microsoft Graph](./toolkit/components/todo.md), diferente do [componente de tarefas do Planner](./toolkit/components/tasks.md), e um [componente de cartão pessoal aprimorado](./toolkit/components/person-card.md). Confira a [postagem do blog](https://developer.microsoft.com/graph/blogs/announcing-the-general-availability-of-microsoft-graph-toolkit-2-0/) relacionada para obter mais informações.


## <a name="december-2020-new-in-preview-only"></a>Dezembro de 2020: novo apenas em pré-visualização

### <a name="compliance--ediscovery"></a>Conformidade | Descoberta Eletrônica
Continuar a cumprir o pipeline das [APIs do Centro de conformidade do Microsoft 365](/graph/api/resources/ediscoveryapioverview?view=graph-rest-beta&preserve-view=true)é o recurso de [guardião](/graph/api/resources/custodian?view=graph-rest-beta&preserve-view=true) e suas operações e métodos relacionados para [liberar](/graph/api/custodian-release?view=graph-rest-beta&preserve-view=true) ou [ativar](/graph/api/custodian-activate?view=graph-rest-beta&preserve-view=true) um guardião. Use o recurso do **guardião** para acessar os dados do guardião ([userSource](/graph/api/resources/userSource?view=graph-rest-beta&preserve-view=true)) em uma caixa de correio do Exchange Online e OneDrive for Business, sites do Microsoft Office SharePoint Online ([siteSource](/graph/api/resources/siteSource?view=graph-rest-beta&preserve-view=true)) e grupos do Microsoft 365 ([unifiedGroupSource](/graph/api/resources/unifiedGroupSource?view=graph-rest-beta&preserve-view=true)).

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
Identifique o status de falha de um desktop virtual gerenciado em nuvem coletivamente como `failed`, na propriedade de **status** do recurso [cloudPC](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true).

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- [Atualize](/graph/api/printjob-update-configuration?view=graph-rest-beta&preserve-view=true) a [configuração](/graph/api/resources/printjobconfiguration?view=graph-rest-beta&preserve-view=true) de um [trabalho de impressão](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true).
- Para obter detalhes sobre a renomeação de algumas propriedades e redigitação de relacionamentos, confira a seção de dezembro de 2020 do [changelog da API](https://developer.microsoft.com/graph/changelog/) para obter detalhes.

### <a name="education"></a>Educação
- Se os alunos forem adicionados após a publicação da tarefa, os professores podem controlar o comportamento da tarefa usando a propriedade **addedStudentAction** do recurso [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true).
- Os professores podem postar notificação de publicação de tarefa por meio da propriedade **notificationChannelUrl** do recurso **educationAssignment**.

### <a name="identity-and-access"></a>Identidade e acesso
Obtenha ou defina a versão e os metadados de criação para um [contrato](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true) de [termos de uso](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true) do Azure Active Directory, [arquivo de contrato](/graph/api/resources/agreementfile?view=graph-rest-beta&preserve-view=true) e [localização de contrato](/graph/api/resources/agreementfilelocalization?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
Como parte do [gerenciamento de direitos](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta&preserve-view=true) do Azure Active Directory, quando os usuários que acessam grupos, aplicativos ou sites do SharePoint Online solicitam um período de acesso a um [pacote de acesso](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true), eles podem responder às [perguntas](/graph/api/resources/accesspackagequestion?view=graph-rest-beta&preserve-view=true) representadas no [conteúdo localizado](/graph/api/resources/accesspackagelocalizedcontent?view=graph-rest-beta&preserve-view=true) na [solicitação de permanência do pacote de acesso](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- Os administradores podem associar fluxos de usuários a aplicativos que são compartilhados com usuários externos e permitir a [inscrição de autoatendimento](/azure/active-directory/external-identities/self-service-sign-up-overview) nesses aplicativos. Eles podem personalizar um fluxo de usuário de inscrição de autoatendimento e criar uma experiência de inscrição personalizada. Especificamente, eles criam um [ouvinte para um evento de início de inscrição para chamar um fluxo de usuário customizado](/graph/api/resources/invokeuserflowlistener?view=graph-rest-beta&preserve-view=true). Depois que um aplicativo é associado ao fluxo do usuário, os usuários que acessam esse aplicativo poderão iniciar um fluxo de inscrição que provisiona uma conta de convidado.
- Em um [fluxo de usuário do Azure Active Directory](/graph/api/resources/b2xidentityuserflow?view=graph-rest-beta&preserve-view=true) ou no [fluxo de usuário do locatário do Azure Active Directory B2C](/graph/api/resources/b2cidentityuserflow?view=graph-rest-beta&preserve-view=true), você pode gerenciar os padrões de idioma e [personalizar o idioma e as cadeias de caracteres exibidas para os usuários no fluxo do usuário](/graph/api/resources/userflowlanguageconfiguration?view=graph-rest-beta&preserve-view=true).
- Use um [conector de API](/graph/api/resources/identityapiconnector?view=graph-rest-beta&preserve-view=true) em fluxos de usuário para inscrição de autoatendimento do Azure Active Directory e inscrição do Azure Active Directory B2C, para chamar uma API em uma etapa específica para afetar a execução do fluxo de usuário.
- Defina uma [política de métodos de autenticação OTP de email](/graph/api/resources/emailauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true) para um locatário.

### <a name="teamwork"></a>Trabalho em equipe
- Para um recurso de [membro](/graph/api/resources/conversationmember?view=graph-rest-beta&preserve-view=true) em uma [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true), [canal](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) ou contexto de [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true), agora você pode:
  - Diferencie um membro que é um [usuário do Azure Active Directory](/graph/api/resources/aaduserconversationmember?view=graph-rest-beta&preserve-view=true), observando a ID do usuário, o endereço de email e a ID do locatário do Azure Active Directory. 
  - [Adicione vários usuários como membros de uma equipe](/graph/api/conversationmembers-add?view=graph-rest-beta&preserve-view=true).
- Para um recurso de [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true):
  - [Obtenha todas as mensagens em chats dos quais o usuário especificado participou](/graph/api/chats-getallmessages?view=graph-rest-beta&preserve-view=true), incluindo chats individuais, chats em grupo e chats de reunião.
  - Use toda a gama de funcionalidades para listar, obter, adicionar, remover e atualizar um [aplicativo](/graph/api/resources/teamsappinstallation?view=graph-rest-beta&preserve-view=true) ou uma [guia](/graph/api/resources/teamstab?view=graph-rest-beta&preserve-view=true) em um chat.
  - Use a propriedade **chatType** para distinguir um chat individual de um chat em grupo ou de um chat associado a uma reunião online.
  - [Crie](/graph/api/chat-post?view=graph-rest-beta&preserve-view=true) ou [atualize](/graph/api/chat-patch?view=graph-rest-beta&preserve-view=true) um chat.
  - Para um membro em um contexto de chat, use a propriedade **visibleHistoryStartDateTime** para definir ou obter um carimbo de data/hora que representa quanto tempo atrás o histórico de uma conversa é compartilhado com esse membro.
  - [Crie](/graph/api/chat-post-members?view=graph-rest-beta&preserve-view=true) ou [exclua](/graph/api/chat-delete-members?view=graph-rest-beta&preserve-view=true) membro de um chat especificado. 
- Para o recurso de [canal](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true):
  - [Obtenha todas as mensagens em todos os canais em uma equipe](/graph/api/channels-getallmessages?view=graph-rest-beta&preserve-view=true).
  - Os proprietários da equipe podem ativar a [moderação de um canal](/graph/api/resources/channelmoderationsettings?view=graph-rest-beta&preserve-view=true) para controlar quem pode iniciar novas postagens ou responder às postagens nesse canal, usando a propriedade **moderationSettings** do canal.
- Como parte da [definição de um aplicativo Teams](/graph/api/resources/teamsappdefinition?view=graph-rest-beta&preserve-view=true), use o relacionamento de **bot** para se conectar a um bot de [trabalho em equipe](/graph/api/resources/teamworkbot?view=graph-rest-beta&preserve-view=true).

### <a name="to-do-tasks"></a>Tarefas pendentes
Assine para [receber notificações de alterações](webhooks.md) de [Tarefas Pendentes](/graph/api/resources/todoTask?view=graph-rest-beta&preserve-view=true).

## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote em novos recursos no [Microsoft Graph User Voice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
    Alguns novos recursos são originados como solicitações populares da comunidade de desenvolvedores. A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

    1. Estreia no status de visualização **_prévia_**. As atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

    2. Promovido para o status de **_disponibilidade geral_ (GA)**, se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/microsoftgraphcall) da chamada mensal à comunidade do Microsoft Graph.
- Inscreva-se no [programa para desenvolvedores do Microsoft 365](https://developer.microsoft.com/office/dev-program), ganhe uma assinatura gratuita do Microsoft 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](https://developer.microsoft.com/graph/changelog/).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).