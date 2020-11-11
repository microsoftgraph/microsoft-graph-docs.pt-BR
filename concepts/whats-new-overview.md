---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: c0399ce4b171224225c570e88b9fbd094e9d2c8d
ms.sourcegitcommit: 4e7830a22b440bbbcfa795937af85d8542e5525b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982692"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](changelog.md). 

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_ , podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use os recursos de visualização em aplicativos de produção.

## <a name="november-2020-new-and-generally-available"></a>Novembro de 2020: novo e geralmente disponível

### <a name="teamwork"></a>Trabalho em equipe
- GA de permissões de consentimento específicas de recurso (RSC). As permissões RSC permitem que os proprietários da equipe concedam consentimento granular a um aplicativo de produção para acessar e/ou modificar dados específicos de uma equipe, como por exemplo, ler as configurações da equipe ou modificar nomes de canal, descrições e outras configurações.
- GA de APIs que se aplicam a um [canal](/graph/api/resources/channel) ou mensagens dentro de um canal. As APIs incluem:
  - [Criar](/graph/api/conversationmember-add) ou [excluir](/graph/api/conversationmember-delete) um membro de conversa de um canal.
  - [Atualizar a função de um membro](/graph/api/conversationmember-update) em um canal.
  - Receber uma mensagem específica ou todas as mensagens em um canal.
  - Receber uma resposta específica ou todas as respostas em um canal.
  - [Acompanhar mensagens novas ou atualizadas em um canal](/graph/api/chatmessage-delta).

## <a name="november-2020-new-in-preview-only"></a>Novembro de 2020: novidades somente na pré-visualização

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
[Inscreva-se para alterar as notificações](webhooks.md) em uma [definição de tarefa de impressão](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true).

### <a name="search"></a>Pesquisar
Você pode agregar resultados de pesquisa de tipo numérico ou cadeia de caracteres que são importados por [conectores do Microsoft Graph](/microsoftsearch/connectors-overview) e que são configurados para serem refináveis no [esquema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true). Veja mais informações sobre [refinar resultados de pesquisa usando agregações](search-concept-aggregation.md).

## <a name="october-2020-new-and-generally-available"></a>Outubro de 2020: novo e geralmente disponível

### <a name="application"></a>Aplicativo
- Permitir [email como uma ID de login alternativa para o Azure Active Directory](/azure/active-directory/authentication/howto-authentication-use-email-signin), usando uma política de [Descoberta de Realm Inicial](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#home-realm-discovery). Uma política de Descoberta de Realm Inicial determina, depois que um usuário fornece uma ID de entrada, se deve solicitar a autenticação do usuário. Nesse caso, definir a propriedade **AlternateIdLogin** de um recurso [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy) pode habilitar que um usuário conecte-se com um endereço de email.
- Obtenha as informações verificadas do fornecedor para um [aplicativo](/graph/api/resources/application) ou [servicePrincipal](/graph/api/resources/serviceprincipal) e [defina](/graph/api/application-setverifiedpublisher) ou [remova](/graph/api/application-unsetverifiedpublisher) as informações verificadas do fornecedor para um **aplicativo**.

### <a name="change-notifications"></a>Mudar notificações
Os aplicativos de produção agora podem assinar notificações de ciclo de vida do Outlook [mensagem](/graph/api/resources/message), [evento](/graph/api/resources/event) e [contato](/graph/api/resources/contact) e do Microsoft Teams [chatMessage](/graph/api/resources/chatmessage) em ordem a [reduzir a falta de assinaturas e alterar as notificações](webhooks-lifecycle.md).

### <a name="identity-and-access"></a>Identidade e acesso
- GA de opções avançadas de consulta do sistema OData (`$count`,`$search` e `$filter`) em objetos de diretório.
- Confira exemplos que mostram o elenco do OData em objetos de diretório.
- Confira a seção Identidade e acesso das atualizações de [outubro](changelog.md#october-2020) no log de mudanças para obter as listas de APIs aprimoradas.

### <a name="teamwork"></a>Trabalho em equipe
- O GA do conjunto completo de operações CRUD para [chatMember](/graph/api/resources/conversationmember) e [aadUserConversationMember](/graph/api/resources/aaduserconversationmember). Esses recursos representam um membro em um chat ou conversa de canal, que pode ou não ser um usuário no Microsoft Azure Active Directory.
- O GA de notificações de ciclo de vida para recursos do Teams de [chatMessage](/graph/api/resources/chatmessage), para [reduzir assinaturas ausentes e notificações de alteração](webhooks-lifecycle.md).

### <a name="to-do-tasks"></a>Tarefas pendentes
O GA da [API Microsoft To-Do](/graph/api/resources/todo-overview?view=graph-rest-1.0&preserve-view=true) - use a API de tarefas em um aplicativo de produção para criar e gerenciar tarefas que fazem parte do fluxo de trabalho de um usuário, como criar uma tarefa de um email.  

### <a name="users"></a>Comercial
Obtenha novas propriedades aplicáveis ​​a um [usuário](/graph/api/resources/user) que é funcionário corporativo: data de contratação, associação organizacional, como divisão e centro de custo, e tipo de funcionário, como consultor, contratado ou fornecedor. Essas propriedades requerem a especificação do `$select`parâmetro de consulta OData na operação GET.

## <a name="october-2020-new-in-preview-only"></a>Outubro de 2020: novo apenas na pré-visualização

### <a name="cloud-communications--online-meeting"></a>Comunicações em nuvem | Reunião online
- Diferencie a função de um participante em uma [reunião online](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) como um participante ou apresentador, usando a propriedade **função** do tipo [meetingParticipantInfo](/graph/api/resources/meetingParticipantInfo?view=graph-rest-beta&preserve-view=true).
- Obtenha uma [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) ao [filtrar na propriedade joinWebUrl da reunião](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-3-retrieve-an-online-meeting-by-joinweburl).

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem

- Descontinue a ação **uploadData** em favor de [criar uma sessão de upload](/graph/api/printdocument-createuploadsession?view=graph-rest-beta&preserve-view=true) para [fazer upload de um documento](upload-data-to-upload-session.md) para uma impressora ou compartilhamento de impressora.
- Cancele a propriedade **configuração** em [printDocument](/graph/api/resources/printdocument?view=graph-rest-beta&preserve-view=true) em favor de uma propriedade de **configuração** semelhante em [printJob](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true).
- Obtenha o URL do trabalho de origem ou de destino para um **printJob** que está sendo redirecionado, usando a propriedade **redirectedFrom** ou **redirectedTo**.
- Obtenha o status atual de um **printJob** usando a propriedade **estado** e a nova propriedade **detalhes**.
- Obtenha a coleção de compartilhamentos de impressora associados a uma [impressora](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true) usando a relação **compartilhamentos**. 
- Substitua a propriedade **processingStateReasons** da **impressora** em favor da propriedade **status**. A propriedade **status** é do tipo [status da impressora](/graph/api/resources/printerstatus?view=graph-rest-beta&preserve-view=true) e expõe uma propriedade **detalhes**. Use a propriedade **detalhes** para identificar o motivo de uma impressora estar no estado atual.
- Cancele a propriedade **feedDirections** em [printerCapabilities](/graph/api/resources/printercapabilities?view=graph-rest-beta&preserve-view=true) em favor da propriedade **feedOrientations** , para obter orientações de alimentação suportadas por uma impressora.
- Confira a seção de impressão na nuvem das atualizações de [outubro](changelog.md#october-2020) no log de mudanças para algumas renomeações de API, propriedades e algumas outras descontinuações.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gestão corporativa
Atualizações do Intune de [outubro](changelog.md#october-2020) para a versão beta.

### <a name="files"></a>Arquivos
[Revogar](/graph/api/permission-revokegrants?view=graph-rest-beta&preserve-view=true) o acesso à para um [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true) ou [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true) concedido por meio de um link de compartilhamento.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- Gerenciar [políticas de método de autenticação](/graph/api/resources/authenticationmethodspolicies-overview?view=graph-rest-beta&preserve-view=true) para identificar os usuários que podem usar métodos de autenticação multifator específicos para entrar no Azure Active Directory. Configure políticas para definir o seguinte:
  - Os tipos de chaves de segurança FIDO2 que podem ser usadas no locatário do Azure AD.
  - Os usuários ou grupos de usuários que têm permissão para usar chaves de segurança FIDO2 ou a Entrada por Telefone sem Senha para entrar no Azure AD.
- Configure um [método de autenticação de email](/graph/api/resources/emailauthenticationmethod?view=graph-rest-beta&preserve-view=true) para que os usuários possam redefinir a senha sozinhos.
- Use o [Azure AD B2C](/azure/active-directory-b2c/overview) e [escolha um mecanismo para configurar e permitir que os usuários finais se autentiquem por contas locais](/graph/api/resources/b2cauthenticationmethodspolicy?view=graph-rest-beta&preserve-view=true).
- Use o `Policy.ReadWrite.AuthenticationMethod` para ler ou gravar as políticas do método de autenticação de uma organização, como uma permissão delegada em nome de um usuário conectado ou como uma permissão de aplicativo sem ter um usuário conectado.
- Especifique em uma [política de autorização](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true) se e quem pode convidar usuários externos para uma organização.

### <a name="people-and-workplace-intelligence--insights"></a>Inteligência de pessoas e local de trabalho | Intuições 
Os administradores podem ver os [exemplos de uso de cmdlets do Windows PowerShell](insights-customize-item-insights-privacy.md#how-to-configure-item-insights-setting-via-powershell) para personalizar as configurações de percepção do item para uma organização.

### <a name="teamwork"></a>Trabalho em equipe
- Use o atributo de instância **channelCreationMode** para indicar que um [canal](https://docs.microsoft.com/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true#instance-attributes) está sendo criado para servir à migração de dados. Use o [completeMigration](/graph/api/channel-completemigration?view=graph-rest-beta&preserve-view=true) para indicar que a migração terminou, de forma que os membros possam postar e ler mensagens.
- Use o atributo de instância **teamCreationMode** para indicar que uma [equipe](https://docs.microsoft.com/graph/api/resources/team?view=graph-rest-beta&preserve-view=true#instance-attributes) está sendo criada para atender à migração. Use o [completeMigration](/graph/api/team-completemigration?view=graph-rest-beta&preserve-view=true) para indicar que a migração terminou, de forma que as operações dos membros podem acontecer e os membros podem postar mensagens.


## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote em novos recursos no [Microsoft Graph User Voice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
    Alguns novos recursos são originados como solicitações populares da comunidade de desenvolvedores. A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

    1. Estreia no status de visualização **_prévia_**. As atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

    2. Promovido para o status de **_disponibilidade geral_ (GA)** , se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/microsoftgraphcall) da chamada mensal à comunidade do Microsoft Graph.
- Inscreva-se no [programa para desenvolvedores do Microsoft 365](https://developer.microsoft.com/office/dev-program), ganhe uma assinatura gratuita do Microsoft 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](changelog.md).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).
