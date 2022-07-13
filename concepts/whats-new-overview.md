---
title: Novidades do Microsoft Graph
description: Exiba os destaques das novidades Microsoft Graph nos últimos dois meses, o que foi adicionado em versões anteriores e como você pode compartilhar suas ideias.
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 26b4024a3fd23fb2ea9f2ee04a02894b16db6e0d
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735331"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Recursos, incluindo APIs e ferramentas, no status de _visualização_ podem mudar sem aviso prévio e alguns podem nunca ser promovidos ao status de disponibilidade geral (GA). Não utilize recursos de visualização em aplicativos de produção.

## <a name="july-2022-new-in-preview-only"></a>Julho de 2022: novo apenas na visualização

### <a name="cloud-communications--call"></a>Comunicações na nuvem | Chamadas
[Ingresse a uma chamada agendada](/graph/api/application-post-calls?view=graph-rest-beta&preserve-view=true) com uma ID ou código de acesso à reunião.

### <a name="cloud-communications--online-meeting"></a>Comunicações na nuvem | Reunião online
[Criar](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true#example-4-create-an-online-meeting-that-requires-a-passcode) uma [reunião online](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) que requer uma senha.

### <a name="users"></a>Usuários
[Obtenha](/graph/api/user-get?view=graph-rest-beta&preserve-view=true) o identificador de segurança (SID) de um usuário em cenários do Windows.

## <a name="june-2022-new-and-generally-available"></a>Junho de 2022: novo e disponível para o público geral

### <a name="cloud-communications--call-records"></a>Comunicações na nuvem | Registros de chamadas
Obtenha informações sobre o codec de áudio, codec de vídeo, protocolo de transporte de rede e saltos de rota de rastreamento para um [fluxo de mídia](/graph/api/resources/callrecords-mediastream) ao [obter um registro de chamada](/graph/api/callrecords-callrecord-get) e expandir cada [segmento](/graph/api/resources/callrecords-segment) de uma [sessão](/graph/api/resources/callrecords-session).

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
- [Liste as unidades administrativas ](/graph/api/device-list-memberOf) que um [dispositivo](/graph/api/resources/device) é membro.
- Gerenciar dispositivos como membros em uma [unidade administrativa](/graph/api/resources/administrativeunit): [listar membros](/graph/api/administrativeunit-list-members) incluindo dispositivos, e [obter](/graph/api/administrativeunit-get-members), [adicionar](/graph/api/administrativeunit-post-members), e [remover](/graph/api/administrativeunit-delete-members) um dispositivo como membro. 
- [Obtenha](/graph/api/application-get) o status e outros detalhes de [certificação de segurança e conformidade](/graph/api/resources/certification) de um [programa](/graph/api/resources/application) para proteger os dados do cliente. Para obter mais informações, consulte [Certificação Microsoft 365](/microsoft-365-app-certification/docs/enterprise-app-certification-guide).
- Defina as [configurações de federação com o Azure AD](/graph/api/resources/internalDomainFederation).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- Configure e gerencie as [configurações da política de métodos de autenticação de Passagem de Acesso Temporário](/graph/api/resources/temporaryAccessPassAuthenticationMethodConfiguration) no seu locatário.
- Obtenha a [política básica em um diretório para configurações de acesso entre locatários](/graph/api/resources/crosstenantaccesspolicy), [configuração padrão](/graph/api/resources/crosstenantaccesspolicyconfigurationdefault) de como uma organização interage com organizações externas do Azure Active Directory e [configurações específicas de parceiros](/graph/api/resources/crosstenantaccesspolicyconfigurationpartner) para organizações externas do Azure Active Directory.

### <a name="reports--microsoft-365-usage-reports"></a>Relatórios | Relatórios de uso do Microsoft 365
Encontre novas colunas nos relatórios do Teams gerados pelos seguintes métodos:
  - [getTeamsUserActivityCounts](/graph/api/reportroot-getteamsuseractivitycounts)
  - [getTeamsUserActivityUserDetail](/graph/api/reportroot-getTeamsUserActivityUserDetail)
  - [getTeamsDeviceUsageUserDetail](/graph/api/reportroot-getTeamsDeviceUsageUserDetail)
  - [getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts)
  - [getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getTeamsDeviceUsageDistributionUserCounts)
- A coluna Windows Phone nos relatórios do Teams gerados pelos seguintes métodos:
  - [getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts)
  - [getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getTeamsDeviceUsageDistributionUserCounts)

### <a name="teamwork"></a>Trabalho em equipe
Assine as notificações de alteração do seguinte no Teams:
- [equipe e canal](teams-changenotifications-team-and-channel.md)
- [associação de equipe e canal](teams-changenotifications-teammembership.md)
- [chat](teams-changenotifications-chat.md)
- [associação do chat](teams-changenotifications-chatmembership.md)
- [mensagens de chat em todos os chats](/graph/teams-changenotifications-chatmessage#subscribe-to-changes-at-the-user-level) dos quais um determinado usuário faz parte.

## <a name="june-2022-new-in-preview-only"></a>Junho de 2022: novo somente na visualização

### <a name="applications"></a>Aplicativos
Especifique [objetos vinculados](/graph/api/resources/synchronization-synchronizationLinkedObjects?view=graph-rest-beta&preserve-view=true) que podem ser [provisionados durante o provisionamento sob demanda](/graph/api/resources/synchronization-synchronizationJobSubject?view=graph-rest-beta&preserve-view=true), incluindo principais como gerente, membros e proprietários.

### <a name="compliance--ediscovery"></a>Conformidade | Descoberta eletrônica
Acesse a [API de Descoberta Eletrônica](/graph/api/resources/security-ediscoverycase?view=graph-rest-beta&preserve-view=true) do namespace de [segurança](/graph/api/resources/security-api-overview?view=graph-rest-beta&preserve-view=true) no futuro, em vez do namespace de conformidade.

### <a name="compliance--records-management"></a>Conformidade | Gerenciamento de registros
Use a [API de gerenciamento de registros do Microsoft Purview](/graph/api/resources/security-recordsmanagement-overview?view=graph-rest-beta&preserve-view=true) de estreia para ajudar as organizações a gerenciar a retenção e a exclusão de dados para cumprir as obrigações legais e os regulamentos de conformidade.

### <a name="customer-booking"></a>Reserva de clientes
- Gerencie o idioma da página de reserva de autoatendimento de uma [empresa](/graph/api/resources/bookingbusiness?view=graph-rest-beta&preserve-view=true) ou de um [serviço](/graph/api/resources/bookingservice?view=graph-rest-beta&preserve-view=true) fornecido pela empresa.
- Especifique nas [informações do cliente](/graph/api/resources/bookingCustomerInformation?view=graph-rest-beta&preserve-view=true) se as notificações por SMS estão habilitada para um [compromisso](/graph/api/resources/bookingappointment?view=graph-rest-beta&preserve-view=true) do cliente.
- Especifique se a junção anônima está habilitada para um [serviço](/graph/api/resources/bookingservice?view=graph-rest-beta&preserve-view=true) e se deve gerar uma URL da Web de junção anônima para um compromisso para o serviço.
- Diferencie a função de um [membro da equipe](/graph/api/resources/bookingstaffmember?view=graph-rest-beta&preserve-view=true) como um agendador ou um membro.
- Especifique se deseja notificar um [membro da equipe](/graph/api/resources/bookingstaffmember?view=graph-rest-beta&preserve-view=true) por email quando uma reserva for atribuída ou atualizada para o membro.

### <a name="device-and-app-management--cloud-pc"></a>Gerenciamento de dispositivos e aplicativos | PC na nuvem
Obtenha as seguintes informações para uma [política de provisionamento](/graph/api/resources/cloudPcProvisioningPolicy?view=graph-rest-beta&preserve-view=true) de PCs na Nuvem:
- O nome do grupo no qual os PCs na Nuvem residem.
- O número de horas de espera antes que o reprovisionamento/desprovisionamento aconteça.
- Se o administrador local (como o usuário final do PC na Nuvem) está habilitado.
- O serviço que gerencia a conexão de rede do Azure, que atualmente é o Windows 365 ou o Microsoft Dev Box.

### <a name="device-and-app-management--multi-tenant-management"></a>Gerenciamento de dispositivos e aplicativos | Gerenciamento multilocatário
[Obtenha](/graph/api/managedtenants-managedtenant-list-myroles?view=graph-rest-beta&preserve-view=true) a coleção de [funções atribuídas a um usuário conectado](/graph/api/resources/managedtenants-myRole?view=graph-rest-beta&preserve-view=true) para um [locatário gerenciado](/graph/api/resources/managedtenants-managedTenant?view=graph-rest-beta&preserve-view=true).

### <a name="education"></a>Educação
- [Crie](/graph/api/educationassignment-setupfeedbackresourcesfolder?view=graph-rest-beta&preserve-view=true) uma pasta do SharePoint em uma [atribuição](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true) para carregar documentos de comentários.
- [Crie](/graph/api/educationfeedbackresourceoutcome-post-outcomes?view=graph-rest-beta&preserve-view=true) um [documento de comentários](/graph/api/resources/educationFeedbackResourceOutcome?view=graph-rest-beta&preserve-view=true) em um [envio](/graph/api/resources/educationsubmission?view=graph-rest-beta&preserve-view=true) na pasta de comentários associada à atribuição.

### <a name="groups"></a>Grupos
Especifique se um [grupo](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) está [ configurado para gravar de volta ](/graph/api/resources/groupWritebackConfiguration?view=graph-rest-beta&preserve-view=true) propriedades de objeto de grupo no Active Directory local.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
- [Promover](/graph/api/domain-promote?view=graph-rest-beta&preserve-view=true) um subdomínio verificado no domínio raiz.
- [Obtenha](/graph/api/application-get?view=graph-rest-beta&preserve-view=true) a URL para os metadados do SAML para federação de um [programa](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) de locatário único.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
Ocultar links de redefinição de senha de autoatendimento (SSPR) nas [configurações de visibilidade de texto da página de logon](/graph/api/resources/loginpagetextvisibilitysettings?view=graph-rest-beta&preserve-view=true) na página de entrada de um locatário. 

### <a name="teamwork"></a>Teamwork
- Obtenha os detalhes de [fixando](/graph/api/resources/messagePinnedEventMessageDetail?view=graph-rest-beta&preserve-view=true) ou [desafixando](/graph/api/resources/messageUnpinnedEventMessageDetail?view=graph-rest-beta&preserve-view=true) uma [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) em um [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true) ou [canal](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true). 
- Como cenários com suporte para exportar o conteúdo do Teams, você pode [listar](/graph/api/teamwork-list-deletedteams?view=graph-rest-beta&preserve-view=true) as equipes que foram excluídas e [obter](/graph/api/deletedteam-getallmessages?view=graph-rest-beta&preserve-view=true) chats individuais, chats em grupo, chats de reunião e mensagens de canal de uma [equipe excluída](/graph/api/resources/deletedTeam?view=graph-rest-beta&preserve-view=true). Para obter mais informações, consulte [Exportar conteúdo com as APIs de exportação do Microsoft Teams](/microsoftteams/export-teams-content).


## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote em novos recursos no [Portal de Comentários da Microsoft](https://aka.ms/graphfeedback).
    Alguns novos recursos são originados como solicitações populares da comunidade de desenvolvedores. A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

    1. Estreia no status de visualização **_prévia_**. As atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

    2. Promovido para o status de **_disponibilidade geral_ (GA)**, se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/m365-dev-call) da chamada semanal da comunidade da plataforma Microsoft 365.
- Inscreva-se no [programa para desenvolvedores do Microsoft 365](https://developer.microsoft.com/office/dev-program), ganhe uma assinatura gratuita do Microsoft 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](https://developer.microsoft.com/graph/changelog/).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).
