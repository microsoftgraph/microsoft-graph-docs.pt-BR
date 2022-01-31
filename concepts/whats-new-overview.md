---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 96d68f14255178ad94bd9fdcc88c8358df018cff
ms.sourcegitcommit: a60e5e81cfa04b666a1df1111a1d91f6c11989e9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2022
ms.locfileid: "62282062"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Recursos, incluindo APIs e ferramentas, no status de _visualização_ podem mudar sem aviso prévio e alguns podem nunca ser promovidos ao status de disponibilidade geral (GA). Não utilize recursos de visualização em aplicativos de produção.


## <a name="january-2022-new-and-generally-available"></a>Janeiro de 2022: Novo e disponível ao público em geral

### <a name="devices-and-apps--service-health-and-communications"></a>Dispositivos e aplicativos | Integridade do serviço e comunicações
Obtenha um [anexo de anúncio de serviço](/graph/api/resources/serviceAnnouncementAttachment) a uma [mensagem de atualização de serviço](/graph/api/resources/serviceupdatemessage).

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
- Obtenha uma coleção de recursos de [revisão de acesso](/graph/api/resources/accessreviewreviewer) que é usada para definir revisores contatados para uma [instância de revisores de acesso](/graph/api/resources/accessReviewInstance).
- Diferencie 3 tipos de recursos cujo acesso é representado por meio de uma [decisão de revisão de acesso](/graph/api/resources/accessreviewinstancedecisionitem):
  - Uma [política de atribuição de pacote de acesso](/graph/api/resources/accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource) para a qual o acesso é determinado por uma decisão de revisão de acesso.
  - Uma [função de recurso do Azure](/graph/api/resources/accessReviewInstanceDecisionItemAzureRoleResource) para a qual o acesso é determinado por uma decisão de revisão de acesso.
  - Uma [entidade de serviço](/graph/api/resources/accessReviewInstanceDecisionItemServicePrincipalResource) cujo acesso a um recurso é determinado por uma decisão de revisão de acesso.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
Imponha um [controle de sessão](/graph/api/resources/conditionalAccessSessionControls) (definindo a propriedade **disableResilienceDefaults**) para determinar se o Microsoft Azure AD deve estender as sessões existentes com base nas informações coletadas antes de uma interrupção.

### <a name="teamwork"></a>Trabalho em equipe
[Criar um chat](/graph/api/chat-post) usando as permissões do aplicativo.

## <a name="january-2022-new-in-preview-only"></a>Janeiro de 2022: Novo somente na pré-visualização

### <a name="compliance--ediscovery"></a>Conformidade | Descoberta eletrônica
Obtenha a URL do site OneDrive for Business de um custodiante (propriedade **siteWebUrl** de [userSource](/graph/api/resources/ediscovery-userSource?view=graph-rest-beta&preserve-view=true)).

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
- Obtenha ou atualize as [configurações de uma organização](/graph/api/resources/cloudpcorganizationsettings?view=graph-rest-beta&preserve-view=true), que incluem a versão do sistema operacional Windows para provisionar em PCs na nuvem e o tipo de conta de usuário nos PCs na nuvem provisionados.
- [Altere o tipo de conta de usuário](/graph/api/cloudPC-changeUserAccountType?view=graph-rest-beta&preserve-view=true) em um PC na nuvem especificado.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
- Os revisores de uma revisão de acesso podem [registrar](/graph/api/accessreviewinstancedecisionitem-recordalldecisions?view=graph-rest-beta&preserve-view=true) as decisões para as quais o usuário atual é o revisor.
- Configure [a data e hora do último login de um usuário como um insight](/graph/api/resources/userLastSignInRecommendationInsightSetting?view=graph-rest-beta&preserve-view=true) para ajudar os revisores na tomada de decisões para uma [definição de cronograma de revisão de acesso](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true).
- Configure [a data e hora da última entrada de um usuário como um insight](/graph/api/resources/userSignInInsight?view=graph-rest-beta&preserve-view=true) para uma [decisão sobre o acesso de um usuário ou entidade de segurança em uma instância de uma revisão de acesso](/graph/api/resources/accessreviewinstancedecisionitem?view=graph-rest-beta&preserve-view=true).
- O solicitante de um pacote de acesso pode fornecer informações personalizadas como parte de um [recurso de pacote de acesso](/graph/api/resources/accesspackageresource?view=graph-rest-beta&preserve-view=true) que pode ser usado para tomar decisões de aprovação do pacote de acesso.
- Um solicitante pode editar a resposta para a uma [pergunta](/graph/api/resources/accessPackageQuestion?view=graph-rest-beta&preserve-view=true) em uma [política de atribuição de pacote de acesso](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true).

### <a name="reports--identity-and-access-reports"></a>Relatórios | Relatórios de identidade e acesso
- Obtenha detalhes dos [métodos de autenticação registrados para um usuário](/graph/api/resources/userRegistrationDetails?view=graph-rest-beta&preserve-view=true), como autenticação multifator, redefinição de senha de autoatendimento e autenticação sem senha.
- Obtenha as seguintes propriedades para um evento de [entrada](/graph/api/resources/signIn?view=graph-rest-beta&preserve-view=true) de um usuário ou aplicativo em uma organização: 
  - Qualquer contexto de autenticação de [acesso condicional](/graph/api/resources/authenticationContext?view=graph-rest-beta&preserve-view=true).
  - Qualquer [política de duração da sessão](/graph/api/resources/sessionLifetimePolicy?view=graph-rest-beta&preserve-view=true) de acesso condicional.
  - A ID de um recurso do Azure acessada durante a entrada.
  - O identificador da credencial de identidade federada de um aplicativo, caso tenha sido usado para entrar.
  - O identificador da entidade de serviço que representa o recurso de destino no evento de entrada.

### <a name="reports--microsoft-365-usage-reports"></a>Relatórios | Relatórios de uso do Microsoft 365
Obtenha relatórios de uso do Outlook, OneDrive e SharePoint para o Microsoft Cloud for US Government. Veja o resumo de [implantações na nuvem](/graph/api/resources/report?view=graph-rest-beta&preserve-view=true#cloud-deployments).

### <a name="sites-and-lists"></a>Sites e listas
- Adicione ou sincronize um tipo de conteúdo do hub de tipo de conteúdo para um [site](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true) ou [lista](/graph/api/resources/list?view=graph-rest-beta&preserve-view=true), usando a ação [addCopyFromContentTypeHub](/graph/api/contenttype-addcopyfromcontenttypehub?view=graph-rest-beta&preserve-view=true). Isso torna um tipo de conteúdo ou sua atualização disponível para um site ou lista específica onde é necessário. Essa é uma melhoria da infraestrutura de sincronização herdada que envia o tipo de conteúdo para todos os sites de uma organização, reduzindo os tempos de espera para a propagação da publicação. 
- Obtenha uma ou mais [operações avançadas e de longa duração](/graph/api/resources/richlongrunningoperation?view=graph-rest-beta&preserve-view=true) ocorrendo em um site ou lista, o que pode acontecer ao adicionar um tipo de conteúdo de forma síncrona.
- Obtenha uma coleção de recursos de [tipo de conteúdo](/graph/api/resources/contentType?view=graph-rest-beta&preserve-view=true) do hub de tipo de conteúdo que são compatíveis usando a ação [getCompatibleHubContentTypes](/graph/api/contenttype-getcompatiblehubcontenttypes?view=graph-rest-beta&preserve-view=true). 

### <a name="teamwork"></a>Trabalho em equipe
- Permita que os usuários escolham **LastModifiedDateTime** ou **CreatedDateTime** como a ordem de classificação ao [listar mensagens em um chat](/graph/api/chat-list-messages?view=graph-rest-beta&preserve-view=true).
- Especifique a atribuição do usuário (na propriedade **onBehalfOf**) quando um bot envia uma [mensagem de chat](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) em nome de um usuário.
- Adicione os seguintes tipos de membros a um [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true):
  - [Convidado anônimo](/graph/api/resources/anonymousGuestConversationMember?view=graph-rest-beta&preserve-view=true)
  - [Usuário da conta Microsoft](/graph/api/resources/microsoftAccountUserConversationMember?view=graph-rest-beta&preserve-view=true)
  - [Usuário do Skype for Business](/graph/api/resources/skypeForBusinessUserConversationMember?view=graph-rest-beta&preserve-view=true)
  - [Skype usuário](/graph/api/resources/skypeUserConversationMember?view=graph-rest-beta&preserve-view=true)

## <a name="december-2021-new-and-generally-available"></a>Dezembro de 2021: novo e disponível ao público geral

### <a name="cloud-communications--presence"></a>Comunicações na nuvem | Presença
[Inscreva-se nas notificações de alterações](/graph/api/subscription-post-subscriptions) no status de [presença](/graph/api/resources/presence) de um usuário especificado. Sempre especifique um certificado de criptografia na solicitação de assinatura, pois são [notificações avançadas que incluem dados de recursos criptografados](webhooks-with-resource-data.md).


### <a name="compliance--subject-rights-requests"></a>Conformidade | Solicitações de direitos de entidade
Como parte do [gerenciamento de privacidade no Microsoft 365](/privacy/solutions/privacymanagement/privacy-management?view=o365-worldwide&preserve-view=true), a [API de solicitações de direitos do sujeito](/graph/api/resources/subjectrightsrequest) estreia nos pontos de extremidade v1 e beta do Microsoft Graph. A API permite que os usuários façam solicitações para revisar ou gerenciar seus dados pessoais em suas organizações. Ele também permite que as organizações automatizem e dimensionem o gerenciamento dessas solicitações, ajudando-as a atender às regulamentações do setor com mais eficiência.

### <a name="customer-booking"></a>Reserva de clientes
Use a API do Microsoft Bookings em aplicativos de produção e aproveite os seguintes novos recursos e atualizações:
- Notifique seus clientes nos EUA ou Canadá por SMS para um [compromisso](/graph/api/resources/bookingappointment) ou serviço [ específico ](/graph/api/resources/bookingservice) associado a um compromisso.
- Habilite a reunião online para um serviço e gere automaticamente um link de reunião do Microsoft Teams para o compromisso.
- Permita um ou mais clientes em um compromisso de grupo, definindo uma contagem máxima de participantes para um serviço e para um compromisso e acompanhando a contagem real de participantes em um compromisso.
- Crie uma [pergunta personalizada](/graph/api/resources/bookingcustomquestion) para uma [empresa](/graph/api/resources/bookingbusiness), associe uma pergunta a uma opção para especificá-la como obrigatória para um serviço e acompanhe perguntas e respostas em um compromisso.
- Obter ou definir o fuso horário de um cliente em um compromisso ou [membro da equipe](/graph/api/resources/bookingstaffmember).
- Obtenha ou defina o local e o número de telefone de um [cliente](/graph/api/resources/bookingcustomer).
- Acesse a API v1 do novo ponto de extremidade `https://graph.microsoft.com/v1.0/solutions/`. Observe que a API beta permanece no `https://graph.microsoft.com/beta` ponto de extremidade.

### <a name="education"></a>Educação
- Especifique [tarefa](/graph/api/resources/educationassignment) ser adicionada somente aos calendários dos alunos usando a propriedade **addToCalendarAction**.
- [Reatribuir](/graph/api/educationsubmission-reassign) uma [tarefa enviada](/graph/api/resources/educationsubmission) a um aluno com feedback para revisão.
- [Listar atribuições](/graph/api/educationuser-list-assignments) para [um educationUser](/graph/api/resources/educationuser). 

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
[Atualizar](/graph/api/accessreviewinstance-update) revisores e revisores de fallback para uma instância [de uma análise de acesso](/graph/api/resources/accessreviewinstance).

### <a name="teamwork"></a>Trabalho em equipe
- Identifique um [chat](/graph/api/resources/chat) no Microsoft Teams por sua URL da Web (por meio da propriedade **webUrl** ).
- Obtenha detalhes de um evento que aconteceu em um chat, canal ou equipe, acessando [eventMessageDetail](/graph/api/resources/EventMessageDetail) de um [chatMessage](/graph/api/resources/chatmessage) ou [chat](/graph/api/resources/chat). Por exemplo, membros adicionados a um canal ou chat, e a descrição da equipe atualizada.

## <a name="december-2021-new-in-preview-only"></a>Dezembro de 2021: novo apenas na visualização

### <a name="cloud-communications--online-meetings"></a>Comunicações na nuvem | Reuniões online
Habilite o registro para uma [reunião online](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) usando um sistema de [registro externo](/graph/api/resources/externalmeetingregistration?view=graph-rest-beta&preserve-view=true). 

### <a name="cloud-communications--presence"></a>Comunicações na nuvem | Presença
- Use a ação [setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true) para definir o status de disponibilidade e atividade preferencial de um usuário. A presença do usuário se torna a presença preferencial.
- Use a ação [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true) para limpar os status de disponibilidade e atividade preferencial de um usuário.
- Use `Presence.ReadWrite` como permissão delegada com [setPresence](/graph/api/presence-setpresence?view=graph-rest-beta&preserve-view=true), [clearPresence](/graph/api/presence-clearpresence?view=graph-rest-beta&preserve-view=true), [setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true)ou [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true).
- Use `Presence.ReadWrite.All` como permissão de aplicativo com [setPresence](/graph/api/presence-setpresence?view=graph-rest-beta&preserve-view=true), [clearPresence](/graph/api/presence-clearpresence?view=graph-rest-beta&preserve-view=true), [setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true)ou [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true).

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
- Os administradores podem habilitar o [Microsoft Managed Desktop](/graph/api/resources/microsoftmanageddesktop?view=graph-rest-beta&preserve-view=true) especificando as configurações em uma [política de provisionamento de PC na nuvem](/graph/api/resources/cloudpcprovisioningpolicy?view=graph-rest-beta&preserve-view=true) e configurando uma experiência de dispositivo gerenciado para um PC na nuvem.
- [Reinicializar](/graph/api/cloudpc-reboot?view=graph-rest-beta&preserve-view=true) um [PC na nuvem](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true).
- [Renomear](/graph/api/cloudpc-rename?view=graph-rest-beta&preserve-view=true) para atualizar o nome de exibição de um PC na nuvem.
- [Solução](/graph/api/cloudpc-troubleshoot?view=graph-rest-beta&preserve-view=true) para verificar o status de integridade de um PC na nuvem e do host da sessão.
- Acompanhe o último resultado da ação remota em um PC na nuvem, incluindo reinicialização, renomeação, reprovisionamento, solução de problemas, pela propriedade **lastRemoteActionResult**.
- Acompanhe o último carimbo de data/hora de logon de um PC na nuvem pela propriedade **lastLoginResult**.
- Rastreie a data em que uma [imagem de dispositivo PC na nuvem](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true) se torna indisponível pela propriedade **expireDate**.
- Acompanhe o status do sistema operacional em uma [imagem de dispositivo de PC na nuvem](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true) pela propriedade **osStatus**.
- [Crie](/graph/api/rbacapplication-post-roledefinitions?view=graph-rest-beta&preserve-view=true), [atualize](/graph/api/unifiedroledefinition-update?view=graph-rest-beta&preserve-view=true) e [exclua](/graph/api/unifiedroledefinition-delete?view=graph-rest-beta&preserve-view=true)um objeto[unifiedRoleDefinition](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true) para um provedor RBAC do PC na nuvem.

### <a name="education"></a>Educação
- [Acompanhe as alterações](delta-query-overview.md) nos recursos [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true) e [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta&preserve-view=true).
- Especifique [tarefa](/graph/api/resources/educationassignment) ser adicionada somente aos calendários dos alunos usando a propriedade **addToCalendarAction**.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
- [Obter](/graph/api/application-get?view=graph-rest-beta&preserve-view=true) os detalhes de certificação de um [aplicativo](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) pela propriedade de **certificação**. A propriedade é definida apenas quando o aplicativo é certificado pelo [Programa de Conformidade do Aplicativo do Microsoft 365](/microsoft-365-app-certification/docs/enterprise-app-certification-guide).  
- [Inclua](/graph/api/permissiongrantpolicy-post-includes?view=graph-rest-beta&preserve-view=true) ou [exclua](/graph/api/permissiongrantpolicy-post-excludes?view=graph-rest-beta&preserve-view=true) a certificação como uma [condição](/graph/api/resources/permissionGrantConditionSet?view=graph-rest-beta&preserve-view=true) em uma [política de concessão de permissão](/graph/api/resources/permissiongrantpolicy?view=graph-rest-beta&preserve-view=true) pela propriedade **certifiedClientApplicationsOnly** de [permissionGrantConditionSet](/graph/api/resources/permissionGrantConditionSet?view=graph-rest-beta&preserve-view=true).

### <a name="search--index"></a>Pesquisa | Índice
Use a operação [atualizar](/graph/api/externalconnectors-schema-update?view=graph-rest-beta&preserve-view=true) para atualizar as propriedades dos itens em um esquema de [conexão](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true), incluindo seus aliases e rótulos.

### <a name="teamwork"></a>Trabalho em equipe
- [Liste](/graph/api/teams-list?view=graph-rest-beta&preserve-view=true) todas as equipes em uma organização.

### <a name="to-do-tasks"></a>Tarefas pendentes
- Para prever a capacidade de gerenciar em um único lugar todas as tarefas de várias fontes (como mensagens do Outlook, chats do Teams, documentos do OneDrive):
  - Use a [Api de Tarefas Pendentes](/graph/api/resources/tasks-overview?view=graph-rest-beta&preserve-view=true) e acesse-o no novo ponto de extremidade `https://graph.microsoft.com/beta/me/tasks/`.
  - Use o segmento `allTasks` para obter todas as tarefas de um usuário: `https://graph.microsoft.com/beta/me/tasks/alltasks`.
  - Diferencie entre uma lista de tarefas interna (como **Email sinalizado** ou **Tarefas**) e uma lista de tarefas definida pelo usuário. Uma lista de tarefas integrada é representada pelo recurso [wellKnownTaskList](/graph/api/resources/wellknowntasklist?view=graph-rest-beta&preserve-view=true) e uma lista de tarefas definida pelo usuário é representada pelo recurso [taskList](/graph/api/resources/tasklist?view=graph-rest-beta&preserve-view=true).
  - Diferencie entre o tipo de tarefas atualmente definido, [tarefa](/graph/api/resources/task?view=graph-rest-beta&preserve-view=true), de um tipo base [baseTask](/graph/api/resources/basetask?view=graph-rest-beta&preserve-view=true).
- Divida uma tarefa mais [tarefa](/graph/api/resources/task?view=graph-rest-beta&preserve-view=true) em subtarefas menores e mais acionáveis. Cada subtarefa é representada por um [checklistItem](/graph/api/resources/checklistitem?view=graph-rest-beta&preserve-view=true) recurso.
- [Mover](/graph/api/basetask-move?view=graph-rest-beta&preserve-view=true) uma tarefa entre listas.
- Consulte esta [ postagem do blog ](https://devblogs.microsoft.com/microsoft365dev/announcing-the-public-preview-of-to-do-tasks-api/) para obter mais detalhes e migre todos os aplicativos existentes que usam a [API To Do anterior](/graph/api/resources/todo-overview?view=graph-rest-beta&preserve-view=true) para a [API To Do mais recente](/graph/api/resources/tasks-overview?view=graph-rest-beta&preserve-view=true).


## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote nos novos recursos na [Comunidade Microsoft Tech](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).
    Alguns novos recursos são originados como solicitações populares da comunidade de desenvolvedores. A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

    1. Estreia no status de **_visualização_**. Todas as atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

    2. Promovido para o status de **_disponibilidade geral_ (GA)**, se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/microsoftgraphcall) da chamada mensal à comunidade do Microsoft Graph.
- Inscreva-se no [programa para desenvolvedores do Microsoft 365](https://developer.microsoft.com/office/dev-program), ganhe uma assinatura gratuita do Microsoft 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](https://developer.microsoft.com/graph/changelog/).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).
