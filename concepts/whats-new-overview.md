---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 0ddbd63e7c5ced08f7737ad8bb01ea15efead715a9912117e215216da3cdcce3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54167230"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Recursos, incluindo APIs e ferramentas, no status de _visualização_ podem mudar sem aviso prévio e alguns podem nunca ser promovidos ao status de disponibilidade geral (GA). Não utilize recursos de visualização em aplicativos de produção.

## <a name="july-2021-new-and-generally-available"></a>Julho de 2021: Novo e disponível para o público em geral

### <a name="cloud-communications--calls"></a>Comunicações na nuvem | Chamadas
Suporte para um limite de capacidade para o número de participantes que um aplicativo pode controlar ao [atender](/graph/api/call-answer) uma [chamada](/graph/api/resources/call), em organizações que adotam [gravação baseada em políticas do Teams](/microsoftteams/teams-recording-policy).

### <a name="users"></a>Usuários
Permitir que um usuário [altere sua própria senha](/graph/api/user-changepassword) sem exigir uma função de administrador.


## <a name="july-2021-new-in-preview-only"></a>Julho de 2021: Novo somente para visualização

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | PC na nuvem
Uma [verificação de integridade](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) de conexão local pode identificar mais alguns tipos de erros de verificação de integridade:
- A conta do computador do PC na Nuvem não foi encontrada na unidade organizacional (`adJoinCheckComputerObjectAlreadyExists`).
- O objeto do PC na Nuvem não foi encontrado no Microsoft Azure Active Directory (`azureAdDeviceSyncCheckDeviceNotFound`).
- Tempo limite para verificar se um objeto do PC na nuvem foi sincronizado com o Microsoft Azure Active Directory (`azureAdDeviceSyncCheckLongSyncCircle`). 

Consulte a [referência](/graph/api/resources/cloudpconpremisesconnectionhealthcheck?view=graph-rest-beta&preserve-view=true#cloudpconpremisesconnectionhealthcheckerrortype-values) para obter detalhes e as ações corretivas recomendadas.

### <a name="devices-and-apps--multi-tenant-management"></a>Dispositivos e aplicativos | Gerenciamento de vários locatários
Lançamento da [API do Microsoft 365 Lighthouse](managedtenants-concept-overview.md) que permite que os Provedores de Serviços Gerenciados (MSPs) gerenciem remotamente vários locatários de clientes em escala para conformidade e detecção de ameaças, e ajudam a manter os dispositivos dos locatários em um estado íntegro e seguro.

### <a name="search"></a>Pesquisa
Use a [API de Pesquisa da Microsoft para recuperar informações sobre as pessoas](search-concept-person.md) que são mais relevantes para um usuário. A relevância é determinada pelos padrões de comunicação, colaboração e pelas relações comerciais do usuário. 

### <a name="teamwork"></a>Trabalho em equipe
- [Inscreva-se para alterar notificações no recurso de chat](teams-changenotifications-chat.md).
- [Inscreva-se para alterar notificações de usuários em um chat](teams-changenotifications-chatmembership.md), em um [canal](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) ou em uma [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) (ou seja, recursos de [conversationMember](/graph/api/resources/conversationmember?view=graph-rest-beta&preserve-view=true)).

## <a name="june-2021-new-and-generally-available"></a>Junho de 2021: novos e disponíveis para o público em geral

### <a name="applications"></a>Aplicativos
Obter ou definir o status de uma [aplicação](/graph/api/resources/application) ou [serviçoPrincipal](/graph/api/resources/serviceprincipal) para identificar se a Microsoft desativou a aplicação através da propriedade **disabledByMicrosoftStatus**. Os motivos de desabilitação incluem atividades suspeitas, abusivas ou mal-intencionadas ou uma violação do Contrato de Serviços Microsoft.

### <a name="change-notifications"></a>Alterar notificações
Estendeu o comprimento máximo de uma assinatura antes de expirar para os seguintes recursos:
- OneDrive [driveItem](/graph/api/resources/driveitem) e Microsoft Office SharePoint Online[lista](/graph/api/resources/list) de 3 a 30 dias.
- [grupo](/graph/api/resources/group), [usuário](/graph/api/resources/user), ou outros recursos de diretório de 3 a 29 dias.

### <a name="change-tracking"></a>Controle de alterações
Removida a limitação para rastrear mudanças em pastas não-root em OneDrive for Business e Microsoft Office SharePoint Online.

### <a name="education"></a>Educação
As APIs para a educação [serviços de atribuições](/graph/api/resources/educationassignment) agora estão disponíveis. 

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
GA da [revisão de acesso](/graph/api/resources/accessreviewsv2-root) API. Confira a [visão geral](accessreviews-overview.md) e tutoriais para [rever o acesso a grupos de segurança](tutorial-accessreviews-securitygroup.md) e [acesso a grupos Microsoft 365](tutorial-accessreviews-m365group.md). Observe que o [API de revisão de acesso ao legado](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true) está sendo depreciado e deixará de retornar dados em maio de 2023.


## <a name="june-2021-new-in-preview-only"></a>Junho de 2021: Novo somente para visualização

### <a name="cloud-communications--online-meetings"></a>Comunicações na nuvem | Reuniões online
Personalizar o controle de áudio e vídeo em [uma Reunião on-line](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true), habilitando ou desabilitando os participantes de ligar suas câmeras e microfones, através da **Permitindo aCâmera de Atendimento** e **Permitindo o Atendimento à Câmera de Habilitação**, respectivamente.

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
- [Atribuir](/graph/api/cloudpcusersetting-assign?view=graph-rest-beta&preserve-view=true) e gerenciar [cloudPcUserSetting](/graph/api/resources/cloudpcusersetting?view=graph-rest-beta&preserve-view=true) para permitir a administração local ou opção de auto-serviço para um usuário em um PC na nuvem. Atualmente, as atribuições podem ser feitas em nível de grupo (usuários pertencentes a um grupo Microsoft 365 ou grupo de segurança).
- [Obter](/graph/api/cloudpc-get?view=graph-rest-beta&preserve-view=true) algumas novas propriedades de um [cloudPC](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true): os nomes da política de provisionamento e da conexão local usada durante o provisionamento e a data/hora de término do período de cortesia pelo qual ocorre o reprovisionamento ou desprovisionamento.
- Suporte para mais status e tipos de erros em um [exame de saúde](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) em uma [conexão no local](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true).

### <a name="education"></a>Educação
- Os professores já podem selecionar o comportamento padrão de um calendário ao publicarem tarefas. Os professores podem controlar o comportamento do calendário da atribuição usando a propriedade **addToCalendarAction** do recurso [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true).
- Os professores já também podem definir um comportamento padrão para um calendário ao publicarem tarefas. Os professores podem controlar o comportamento do calendário padrão da atribuição usando a propriedade **addToCalendarAction** do recurso [educationAssignment](/graph/api/resources/educationAssignmentDefaults?view=graph-rest-beta&preserve-view=true).

### <a name="groups"></a>Grupos
Permitir que um [grupo](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) seja atribuído a uma função do Azure Active Directory na criação definindo a propriedade **isAssignableToRole**. Se definida, essa propriedade torna conveniente gerenciar funções para indivíduos – em vez de ter que atribuir uma função a cada pessoa individual, as pessoas qualificadas podem ingressar em um grupo e, atribuindo a função ao grupo, por padrão, atribuiria a função a cada nova pessoa que ingressasse no grupo. 

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
Definir usuários ou membros do grupo a serem notificados sobre o progresso de uma [análise de acesso](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true), usando a propriedade **additionalNotificationRecipients** da [definição de agendamento](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
Definir um filtro para incluir ou excluir dinamicamente dispositivos, usando o **deviceFilter** propriedade de [conditionalAccessDevices](/graph/api/resources/conditionalAccessDevices?view=graph-rest-beta&preserve-view=true).

### <a name="sites-and-lists"></a>Sites e listas
Criar ou obter um [sharingLink](/graph/api/resources/sharinglink?view=graph-rest-beta&preserve-view=true) existente para uma [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true) chamando [createLink](/graph/api/listitem-createlink?view=graph-rest-beta&preserve-view=true).

### <a name="teamwork"></a>Trabalho em equipe
- [Obter](/graph/api/chat-get?view=graph-rest-beta&preserve-view=true) uma URL opaca para um [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true) através da **webUrl** propriedade.
- [Assinar notificações de mudança](/graph/webhooks?view=graph-rest-beta&preserve-view=true) de um [canal](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true), [membro de conversação](/graph/api/resources/conversationmember?view=graph-rest-beta&preserve-view=true), ou [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) recurso.
- Usar [consentimento específico de recursos](/microsoftteams/platform/graph-api/rsc/resource-specific-consent) permissões com as APIs para [canal](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true), [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true), [chatMessage](/graph/api/resources/chatMessage?view=graph-rest-beta&preserve-view=true), [chatMessageHostedContent](/graph/api/resources/chatMessageHostedContent?view=graph-rest-beta&preserve-view=true), ou [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true).
- Obter uma lista de [permissões específicas de recursos concedidos](/graph/api/resources/resourcespecificpermissiongrant?view=graph-rest-beta&preserve-view=true) para uma [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true), que especifica as aplicações da equipe e as permissões específicas de recursos correspondentes que lhes foram concedidas.
- [Obter](/graph/api/teamsasyncoperation-get?view=graph-rest-beta&preserve-view=true) uma [operação assíncrona específica](/graph/api/resources/teamsasyncoperation?view=graph-rest-beta&preserve-view=true), ou [lista](/graph/api/chat-list-operations?view=graph-rest-beta&preserve-view=true) todas as operações assíncronas que funcionam em um [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true).
- Pode especificar um aplicativo[Teams](/graph/api/resources/teamsapp?view=graph-rest-beta&preserve-view=true) ao [criar um chat](/graph/api/chat-post?view=graph-rest-beta&preserve-view=true).
- Usar uma única ação [provisionEmail](/graph/api/channel-provisionemail?view=graph-rest-beta&preserve-view=true) para obter o endereço de email de um [canal](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true), se houver, ou criar um, se não houver. Usar a ação [removeEmail](/graph/api/channel-removeemail?view=graph-rest-beta&preserve-view=true) para remover o endereço de email.

### <a name="teamwork--shifts"></a>Trabalho em equipe | Turnos
- Suporte para as entidades [offerShiftRequest](/graph/api/resources/offershiftrequest?view=graph-rest-beta&preserve-view=true), [timeOff](/graph/api/resources/timeoff?view=graph-rest-beta&preserve-view=true), [timeOffReason](/graph/api/resources/timeoffreason?view=graph-rest-beta&preserve-view=true), e [timeOffRequest](/graph/api/resources/timeoffrequest?view=graph-rest-beta&preserve-view=true) para notificações de alteração síncronas.
- Suporte para gerenciar [recursos do cartão de ponto](/graph/api/resources/timecard?view=graph-rest-beta&preserve-view=true) e funcionalidades comuns, tais como [entrada do relógio](/graph/api/timecard-clockin?view=graph-rest-beta&preserve-view=true), [saída do relógio](/graph/api/timecard-clockout?view=graph-rest-beta&preserve-view=true), [partida inicial](/graph/api/timecard-startbreak?view=graph-rest-beta&preserve-view=true), [partida final](/graph/api/timecard-endbreak?view=graph-rest-beta&preserve-view=true), [confirmar](/graph/api/timecard-confirm?view=graph-rest-beta&preserve-view=true), e [substituir](/graph/api/timecard-replace?view=graph-rest-beta&preserve-view=true).


## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote em novos recursos no [Microsoft Tech Community](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).
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
