---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 156f15534b102d5a3e17acd7b04c32e30f34a3f7
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61803501"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Recursos, incluindo APIs e ferramentas, no status de _visualização_ podem mudar sem aviso prévio e alguns podem nunca ser promovidos ao status de disponibilidade geral (GA). Não utilize recursos de visualização em aplicativos de produção.


## <a name="december-2021-new-and-generally-available"></a>Dezembro de 2021: novo e disponível ao público geral

### <a name="cloud-communications--presence"></a>Comunicações na nuvem | Presença
[Inscreva-se nas notificações de alterações](/graph/api/subscription-post-subscriptions?view=graph-rest-beta&preserve-view=true) no status de [presença](/graph/api/resources/presence) de um usuário especificado. Sempre especifique um certificado de criptografia na solicitação de assinatura, pois são [notificações avançadas que incluem dados de recursos criptografados](webhooks-with-resource-data.md).


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


## <a name="november-2021-new-and-generally-available"></a>Novembro de 2021: Novo e geralmente disponível ao público

### <a name="files"></a>Arquivos
Obtenha o estado de uma unidade a partir de um horário específico especificando o carimbo de data/hora codificado no URL correspondente. Veja um [exemplo](/graph/api/driveitem-delta#example-4-retrieving-delta-results-using-a-timestamp).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
- Execute [campanhas](/graph/api/resources/authenticationMethodsRegistrationCampaign) e [imponha os usuários a se registrarem](/graph/api/resources/registrationEnforcement) no momento da entrada para configurar os métodos de autenticação direcionados.
-  Configurar um [provedor de identidade Apple](/graph/api/resources/applemanagedidentityprovider) em um locatário do Azure AD B2C.

## <a name="november-2021-new-in-preview-only"></a>Novembro de 2021: Novo somente na pré-visualização

### <a name="cloud-communications--online-meeting"></a>Comunicações na nuvem | Reunião online
Admita automaticamente novos tipos de participantes em uma reunião online e ignore o lobby da reunião:
- Somente pessoas convidadas pelo organizador.
- Somente os participantes da mesma empresa.

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
- Defina uma [configuração](/graph/api/resources/cloudPcDomainJoinConfiguration?view=graph-rest-beta&preserve-view=true) de como um dispositivo de PC na nuvem provisionado pode ingressar no Azure Active Directory (Microsoft Azure AD): somente nuvem e ingressar somente no Microsoft Azure AD, ou híbrido e ingressar no Active Directory local e no Microsoft Azure AD.
- Obtenha o [recurso de imagem da galeria](/graph/api/resources/cloudPcGalleryImage?view=graph-rest-beta&preserve-view=true) da organização atual que pode ser usado para provisionar um PC na nuvem.

### <a name="devices-and-apps--device-updates"></a>Dispositivos e aplicativos | Atualizações do dispositivo
- Use as [configurações de salvaguarda](/graph/api/resources/windowsupdates-safeguardSettings?view=graph-rest-beta&preserve-view=true) para recusar as proteções contra prováveis problemas em uma implantação.
- Suporte para um [estado de implantação](/graph/api/resources/windowsupdates-deploymentState?view=graph-rest-beta&preserve-view=true) em que uma implantação está com defeito devido ao conteúdo não ser mais implantável, por exemplo, no fim do serviço.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
- Defina e atribua [atributos de segurança personalizado ](/graph/api/resources/custom-security-attributes-overview?view=graph-rest-beta&preserve-view=true) aos objetos do Microsoft Azure AD. Use esses atributos para armazenar informações, categorizar objetos ou impor um controle de acesso refinado sobre recursos específicos do Azure. Use esses atributos com o [Controle de acesso baseado em atributo do Azure](/azure/role-based-access-control/conditions-overview) (Azure ABAC).
- [Crie um grupo dentro de uma unidade administrativa](/graph/api/administrativeunit-post-members?view=graph-rest-beta&preserve-view=true).

### <a name="reports--microsoft-365-usage-reports"></a>Relatórios | Relatórios de uso do Microsoft 365
[Os relatórios de uso do Microsoft 365](/graph/api/resources/report?view=graph-rest-beta&preserve-view=true) no tipo de saída JSON não são mais fortemente tipados e são do tipo `Edm.Stream`. Para obter mais informações, consulte [Alterações da propriedade OData na API de relatórios de uso do Microsoft 365 no Microsoft Graph](https://devblogs.microsoft.com/microsoft365dev/odata-property-changes-to-microsoft-365-usage-reports-api-in-microsoft-graph/).

### <a name="teamwork"></a>Trabalho em equipe
Marque um chat como [lido](/graph/api/chat-markChatReadForUser?view=graph-rest-beta&preserve-view=true) ou [não lido](/graph/api/chat-markchatunreadforuser?view=graph-rest-beta&preserve-view=true) para um usuário.



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
