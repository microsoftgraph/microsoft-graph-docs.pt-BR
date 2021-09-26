---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: c3c777812ca45cc1ad8d28bdbb266b63b0df3880
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59764511"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Recursos, incluindo APIs e ferramentas, no status de _visualização_ podem mudar sem aviso prévio e alguns podem nunca ser promovidos ao status de disponibilidade geral (GA). Não utilize recursos de visualização em aplicativos de produção.

## <a name="september-2021-new-and-generally-available"></a>Setembro de 2021: novo e disponível para o público em geral

### <a name="cloud-communications--online-meetings"></a>Comunicações na nuvem | Reuniões on-line
Use `OnlineMeetingArtifact.Read.All` como delegada ou permissão de aplicativo para ler artefatos de reuniões on-line. Para obter mais informações, consulte [permissões de reuniões on-line](permissions-reference.md#online-meetings-permissions).

### <a name="files"></a>Arquivos
- Obtenha os detalhes de qualquer vírus detectado em um [driveItem](/graph/api/resources/driveItem) por meio de uma propriedade de **malware**.
- Use a função [delta](/graph/api/driveitem-delta) para acompanhar as alterações não apenas no diretório raiz, mas também em outras pastas dentro de uma unidade.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
- Os provedores de controle de acesso baseado em função (RBAC) podem [gerenciar funções](/graph/api/resources/rolemanagement) do Azure Active Directory, [definindo ações de funções](/graph/api/resources/unifiedroledefinition)que podem ser realizadas em recursos específicos e [atribuindo funções](/graph/api/resources/unifiedroleassignment) aos usuários com base em tais definições de função, fornecendo o acesso correspondente a esses recursos.

### <a name="search--query"></a>Pesquisa | Consulta
- Agregar resultados de pesquisa do tipo numérico ou cadeia de caracteres que são importados pelos [conectores do Microsoft Graph](/microsoftsearch/connectors-overview) e que estão configurados no [esquema](/graph/api/resources/schema) para serem refináveis. Veja mais informações sobre [como refinar resultados de pesquisa usando agregações](search-concept-aggregation.md).
- [Classifique](/graph/api/resources/search-api-overview#sort-search-results) os resultados de pesquisa do OneDrive e do SharePoint em qualquer propriedade classificável. Para obter mais informações, consulte [Uso da API de Pesquisa da Microsoft para classificar resultados da pesquisa](search-concept-sort.md).

### <a name="teamwork"></a>Trabalho em equipe
- Usar uma única ação [provisionEmail](/graph/api/channel-provisionemail) para obter o endereço de email de um [canal](/graph/api/resources/channel), se houver, ou criar um, se não houver. Usar a ação [removeEmail](/graph/api/channel-removeemail) para remover o endereço de email.

### <a name="workbooks-and-charts"></a>Pastas de trabalho e gráficos
Criar linhas de tabela de forma assíncrona. Para um melhor desempenho, uma boa prática para criar várias linhas de tabela é agrupá-las em uma operação do tipo [criar tableRow](/graph/api/table-post-rows) e realizar a operação de forma assíncrona. Prossiga com a operação [GET workbookOperation](/graph/api/workbookoperation-get) e a função [tableRowOperationResult](/graph/api/workbook-tableRowOperationResult) para obter o novo recurso [workbookTableRow](/graph/api/resources/workbooktablerow).


## <a name="september-2021-new-in-preview-only"></a>Setembro de 2021: novos somente em versão prévia

### <a name="cloud-communications--online-meetings"></a>Comunicações na nuvem | Reuniões on-line
Obter o número total de participantes em um [relatório de presença de reunião](/graph/api/resources/meetingattendancereport?view=graph-rest-beta&preserve-view=true) de uma [reunião on-line](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true).

### <a name="compliance--ediscovery"></a>Conformidade | Descoberta eletrônica
A operação [criar caso](/graph/api/ediscovery-case-post?view=graph-rest-beta&preserve-view=true) sempre cria casos em formato grande. Isso expande o limite do tamanho de caso para acomodar um volume total de dados e um número total de itens mais altos. Para obter mais detalhes, consulte [vantagens de casos grandes](/microsoft-365/compliance/advanced-ediscovery-large-cases?view=o365-worldwide&preserve-view=true#benefits-of-large-cases).

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
- [Reprovisionar um computador na nuvem](/graph/api/manageddevice-reprovisioncloudpc?view=graph-rest-beta&preserve-view=true) como uma área de trabalho virtual gerenciada na nuvem registrada no Intune.
- [Redimensionar um computador na nuvem](/graph/api/manageddevice-resizecloudpc?view=graph-rest-beta&preserve-view=true) atualizando-o ou rebaixando-o para outra configuração com uma CPU virtual (vCPU) e um tamanho de armazenamento novos.

### <a name="education"></a>Educação
Suporte para adicionar tarefas apenas aos calendários dos alunos se você usar o cabeçalho de solicitação `Prefer: include-unknown-enum-members` para operações nos recursos [educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true) ou [educationAssignmentDefaults](/graph/api/resources/educationassignmentdefaults?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
[Excluir](/graph/api/accesspackageassignmentrequest-delete?view=graph-rest-beta&preserve-view=true) um [accessPackageAssignmentRequest](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true) para remover uma solicitação negada ou concluída.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
Permitir que os usuários executem a autenticação multifatorial usando um [token de software OATH](/graph/api/resources/softwareOathAuthenticationMethod?view=graph-rest-beta&preserve-view=true). Um token de software OATH é um gerador de números baseado em software que usa a Senha de Uso Único Baseada em Tempo (TOTP) padrão OATH.


## <a name="august-2021-new-and-generally-available"></a>Agosto de 2021: novo e disponível para o público em geral

### <a name="cloud-communications--calls"></a>Comunicações na nuvem | Chamadas
Um [participante](/graph/api/resources/participant) pode incluir metadados como um blob de dados na lista de participantes de uma [chamada](/graph/api/resources/call).

### <a name="cloud-communications--online-meetings"></a>Comunicações na nuvem | Reuniões on-line
- Criar uma [reunião on-line](/graph/api/resources/onlinemeeting) como um evento ao vivo, definindo as [configurações de transmissão](/graph/api/resources/broadcastMeetingSettings) e as [informações dos participantes da reunião](/graph/api/resources/meetingparticipantinfo) com a função de produtor. Veja um [exemplo](/graph/api/application-post-onlinemeetings#example-2-create-a-live-event-with-user-token).
- Habilitar, desabilitar ou limitar a duração do chat de uma reunião online usando a propriedade **allowMeetingChat**.
- Habilitar ou desabilitar reações a uma reunião online usando a propriedade **allowTeamworkReactions**.
- Permitir que um participante ligue sua câmera ou seus microfones usando, respectivamente, as propriedades **allowAttendeeToEnableCamera** ou **allowAttendeeToEnableMic**.

### <a name="cloud-communications--presence"></a>Comunicações na nuvem | Presença
- [Definir o estado de presença de um usuário](/graph/api/presence-setpresence), que é um estado agregado em cada cliente do Teams (desktop, celular ou web).
- [Limpar a sessão de presença](/graph/api/presence-clearpresence) para um usuário.


### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações mensais do Intune para a versão v1.0. Configure o filtro **Data** para agosto de 2021 e procure uma seção com esse mesmo cabeçalho.

### <a name="devices-and-apps--service-health-and-communications"></a>Dispositivos e aplicativos | Integridade do serviço e comunicações
GA da [API de comunicações de serviço](service-communications-concept-overview.md) no Microsoft Graph para acessar o status de integridade e as postagens do centro de mensagens sobre os serviços em nuvem da Microsoft.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
Obtenha uma coleção de escopos de revisão de acesso usados para definir revisores e revisores substitutos para uma [instância de revisores de acesso](/graph/api/resources/accessReviewInstance).

### <a name="sites-and-lists--taxonomy"></a>Sites e listas | Taxonomia
Acessar a taxonomia do [repositório de termos](/graph/api/resources/termstore-store) do SharePoint, a hierarquia que consiste de recursos de [grupo](/graph/api/resources/termstore-group), [conjunto](/graph/api/resources/termstore-set), e [termo](/graph/api/resources/termstore-term), e [relacionar](/graph/api/resources/termstore-relation) os recursos entre os termos.

### <a name="teamwork"></a>Trabalho em equipe
[Listar os chats](/graph/api/chat-list) dos quais um usuário faz parte, em um contexto delegado.

## <a name="august-2021-new-in-preview-only"></a>Agosto de 2021: novos somente em versão prévia

### <a name="cloud-communications--calls"></a>Comunicações na nuvem | Chamadas
- Colocar um [participante](/graph/api/resources/participant?view=graph-rest-beta&preserve-view=true) em espera e tocar música em segundo plano usando a ação [startHoldMusic](/graph/api/participant-startHoldMusic?view=graph-rest-beta&preserve-view=true).
- Reincorporar um participante colocado em espera em uma chamada anteriormente usando a ação [stopHoldMusic](/graph/api/participant-stopHoldMusic?view=graph-rest-beta&preserve-view=true).

### <a name="cloud-communications--online-meetings"></a>Comunicações na nuvem | Reuniões on-line
Configurar uma [reunião on-line](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) para gravar automaticamente.

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
[Encerrar o período de tolerância](/graph/api/cloudPC-endGracePeriod?view=graph-rest-beta&preserve-view=true) para um computador na nuvem. O período de tolerância permite que os usuários acessem os computadores na nuvem até sete dias antes da ocorrência do desprovisionamento. Encerrar o período de tolerância imediatamente desprovisiona o computador na nuvem sem aguardar os sete dias.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações mensais do Intune para a versão beta. Configure o filtro **Data** para agosto de 2021 e procure uma seção com esse mesmo cabeçalho.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
- [Reprocesse](/graph/api/accesspackageassignmentrequest-reprocess?view=graph-rest-beta&preserve-view=true) uma [solicitação de atribuição de pacote de acesso](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true) para repetir automaticamente a solicitação de acesso de um usuário ao pacote.
- [Reprocesse](/graph/api/accesspackageassignment-reprocess?view=graph-rest-beta&preserve-view=true)[ uma atribuição de pacote de acesso](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true) para reavaliar e impor automaticamente as atribuições de um usuário.
- [Obtenha um conjunto de requisitos de política](/graph/api/accesspackage-getapplicablepolicyrequirements?view=graph-rest-beta&preserve-view=true) para criar uma [solicitação de atribuição para um pacote de acesso](/graph/api/resources/accesspackageassignmentrequestrequirements?view=graph-rest-beta&preserve-view=true).
- Obtenha uma coleção de recursos de [revisão de acesso](/graph/api/resources/accessreviewreviewer?view=graph-rest-beta&preserve-view=true) que é usada para definir revisores contatados para uma [instância de revisores de acesso](/graph/api/resources/accessReviewInstance?view=graph-rest-beta&preserve-view=true).
- Obtenha ou defina a duração de inatividade a partir da qual as recomendações são definidas nas [configurações de agendamento de uma revisão de acesso](/graph/api/resources/accessReviewScheduleSettings?view=graph-rest-beta&preserve-view=true) usando a propriedade **RecommendationLookBackDuration**.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- As organizações podem usar [políticas para aplicar as melhores práticas para aplicativos usando métodos de autenticação de aplicativos](/graph/api/resources/applicationauthmethodpolicy?view=graph-rest-beta&preserve-view=true). Essas políticas podem ser aplicadas a [aplicativos e entidades de serviço específicos](/graph/api/resources/appmanagementpolicy?view=graph-rest-beta&preserve-view=true) ou a [todos os aplicativos e entidades de serviço em um locatário](/resources/tenantappmanagementpolicy?view=graph-rest-beta&preserve-view=true).
- Suporte para paginação na propriedade de navegação **appRoleAssignments** para [usuários](/api/user-list-approleassignments?view=graph-rest-beta&preserve-view=true), [grupos](/api/group-list-approleassignments?view=graph-rest-beta&preserve-view=true) e [entidades de serviço](/api/serviceprincipal-list-approleassignments?view=graph-rest-beta&preserve-view=true).
- Permitir que um locatário do Azure Active Directory (Azure AD) defina uma [federação com outra organização cujo provedor de identidade (IdP) ofereça suporte ao protocolo SAML ou WS-Fed](/graph/api/resources/samlOrWsFedExternalDomainFederation?view=graph-rest-beta&preserve-view=true). Isso permite que o locatário do Azure AD dê acesso aos seus recursos para usuários convidados.

### <a name="teamwork"></a>Trabalho em equipe
- Obter [informações sobre uma reunião on-line](/graph/api/resources/teamworkOnlineMeetingInfo?view=graph-rest-beta&preserve-view=true) que esteja associada a um [chat](/api/resources/chat?view=graph-rest-beta&preserve-view=true).
- Obter o identificador do locatário no qual um **chat** é criado.

### <a name="users"></a>Usuários
Use os últimos valores de data/hora de login interativo e não interativo do [signInActivity](/graph/api/resources/signInActivity?view=graph-rest-beta&preserve-view=true) dos usuários para [gerenciar contas inativas](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts).

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
