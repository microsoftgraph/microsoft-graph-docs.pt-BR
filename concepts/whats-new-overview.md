---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: d8478b405804da10e7bad3de647b45751f14ae86
ms.sourcegitcommit: 59df7b4d5098a49403a315d19a0c048013cd592e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50723097"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use os recursos de visualização em aplicativos de produção.

## <a name="march-2021-new-and-generally-available"></a>Março de 2021: novo e disponível para o público geral

### <a name="applications"></a>Aplicativos
GA do recurso [applicationTemplate](/graph/api/resources/applicationtemplate) que suporta a [listagem](/graph/api/applicationtemplate-list) de aplicativos na galeria de aplicativos do Azure AD e a [adição](/graph/api/applicationtemplate-instantiate) de uma instância desse aplicativo a um diretório.

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
GA da [API de impressão em nuvem](universal-print-concept-overview.md) para Impressão Universal! Veja o [comunicado](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/universal-print-is-ready-for-business/ba-p/2176778) e confira como [começar com a Impressão Universal](https://docs.microsoft.com/universal-print/fundamentals/universal-print-license).

### <a name="teamwork"></a>Trabalho em equipe
- GA de mais algumas propriedades de [teamsAppDefinition](/graph/api/resources/teamsAppDefinition), que representam detalhes de uma versão de um aplicativo no catálogo de aplicativos do Microsoft Teams, incluindo o seguinte:
  - **createdBy**, **description**, **shortDescription**, **lastModifiedDateTime**
  - **publishingState**, que pode ser `submitted` e em revisão, `published` ou `rejected` pelo administrador
  - Relação de **bot** do tipo [teamworkBot](/graph/api/resources/teamworkbot), representando os detalhes do bot especificado no manifesto do aplicativo Teams.
- [Liste](/graph/api/chatmessage-list-chatmessagehostedcontents) ou [obtenha](/graph/api/chatmessagehostedcontent-get) conteúdo avançado hospedado em uma [chatMessage](/graph/api/resources/chatmessage), como imagens ou trechos de código.

## <a name="march-2021-new-in-preview-only"></a>Março de 2021: Novo apenas em versão prévia

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
Obtenha a data/hora mais recente (propriedade **lastSeenDateTime**) em que uma impressora interagiu com a Impressão Universal.

### <a name="sites-and-lists"></a>Sites e listas
- Suporta um tipo ou modelo de conteúdo específico para documentos ou conjuntos de documentos em conjuntos de sites específicos, por meio de um conjunto de novas propriedades e métodos na entidade [contentType](/graph/api/resources/contentType?view=graph-rest-beta&preserve-view=true). Os métodos incluem o seguinte:
  - [addCopy](/graph/api/contenttype-addcopy?view=graph-rest-beta&preserve-view=true)
  - [associateWithHubSites](/graph/api/contenttype-associatewithhubsites?view=graph-rest-beta&preserve-view=true)
  - [copyToDefaultContentLocation](/graph/api/contenttype-copytodefaultcontentlocation?view=graph-rest-beta&preserve-view=true)
  - [isPublished](/graph/api/contenttype-ispublished?view=graph-rest-beta&preserve-view=true)
  - [publish](/graph/api/contenttype-publish?view=graph-rest-beta&preserve-view=true)
  - [unpublish](/graph/api/contenttype-unpublish?view=graph-rest-beta&preserve-view=true)
- Personalize os tipos de conteúdo de acordo com as colunas. As colunas são representadas pela entidade [columnDefinition](/graph/api/resources/columndefinition?view=graph-rest-beta&preserve-view=true) e suportam o conjunto completo de operações CRUD.
- [Obtenha os tipos de conteúdo de um site que podem ser aplicados a uma lista](/graph/api/site-getApplicableContentTypesForList?view=graph-rest-beta&preserve-view=true).
- Diferencie os tipos de coluna pelas seguintes propriedades na entidade **columnDefinition**: booliana, calculada, escolha, moeda, dateTime, pesquisa, número, personOrGroup, texto. Essas categorias são mutuamente exclusivas.

### <a name="users"></a>Usuários
[Obtenha](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta&preserve-view=true) ou [atualize](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta&preserve-view=true) as [preferências de um usuário para traduzir idiomas](/graph/api/resources/translationpreferences?view=graph-rest-beta&preserve-view=true). Por exemplo, se deve ou não traduzir, traduzir automaticamente ou solicitar antes de traduzir idiomas específicos em mensagens, chats e páginas da Web e qualquer [substituição de tradução](/graph/api/resources/translationlanguageoverride?view=graph-rest-beta&preserve-view=true).

## <a name="february-2021-new-and-generally-available"></a>Fevereiro de 2021: novo e disponível para o público geral

### <a name="cloud-communications--online-meeting"></a>Comunicações em nuvem | Reunião online
Use permissões de aplicativo baseada em políticas `OnlineMeetings.Read.All` ou `OnlineMeetings.ReadWrite.All` sobre as operações e métodos do recurso [onlineMeeting](/graph/api/resources/onlinemeeting). Isso significa que os administradores podem [configurar a política de acesso a aplicativos](cloud-communication-online-meeting-application-access-policy.md) para permitir que os aplicativos acessem as reuniões online em nome de um usuário.

### <a name="sites-and-lists"></a>Sites e listas
Use o recurso de [permissão](/graph/api/resources/permission) e suas operações CRUD para gerenciar a permissão de compartilhamento concedida para um [driveItem](/graph/api/resources/driveitem). Permissões com uma faceta link representam links de compartilhamento criados no item. Permissões com uma faceta invitation representam permissões adicionadas convidando usuários ou grupos específicos para ter acesso ao arquivo.

## <a name="february-2021-new-in-preview-only"></a>Fevereiro de 2021: novo apenas em pré-visualização

### <a name="applications"></a>Aplicativos
Use permissões de aplicativo para as [APIs de sincronização](/graph/api/resources/synchronization-overview?view=graph-rest-beta&preserve-view=true) que automatizam o provisionamento (criação, manutenção) e o desprovisionamento (remoção) de identidades no Azure AD.

### <a name="cloud-communications--calls"></a>Comunicações na nuvem | Chamadas
Suporte para [gravação baseada em políticas para chamadas](/microsoftteams/teams-recording-policy) onde, usando a política administrativa, as chamadas são gravadas automaticamente para processamento e retenção subsequentes, conforme exigido pela política corporativa ou regulamentar relevante. Antes de um participante baseado em política ingressar em uma chamada, a política solicita o envio de um [participantJoiningNotification](/graph/api/resources/participantJoiningNotification?view=graph-rest-beta&preserve-view=true) ao bot associado à política que tem capacidade para lidar com o novo participante. O bot responde com [acceptJoinResponse](/graph/api/resources/acceptjoinresponse?view=graph-rest-beta&preserve-view=true), [rejectJoinResponse](/graph/api/resources/rejectjoinresponse?view=graph-rest-beta&preserve-view=true) ou [inviteNewBotResponse](/graph/api/resources/invitenewbotresponse?view=graph-rest-beta&preserve-view=true) em seu conteúdo de resposta.

### <a name="compliance--ediscovery"></a>Conformidade | Descoberta Eletrônica
- Use o recurso [legalHold](/graph/api/resources/ediscovery-legalhold?view=graph-rest-beta&preserve-view=true) e suas APIs para proteger o conteúdo indefinidamente contra exclusão, para fins de litígio, investigação interna ou outras ações legais.
- Use o recurso [sourceColection](/graph/api/resources/ediscovery-sourcecollection?view=graph-rest-beta&preserve-view=true) e suas APIs para pesquisar e identificar documentos relevantes de locais com ou sem custódia no Microsoft 365.
- Use o recurso [tag](/graph/api/resources/ediscovery-tag?view=graph-rest-beta&preserve-view=true) e as APIs para marcar documentos durante a revisão para separar o conteúdo responsivo e não responsivo.
- [Exporte](/graph/api/ediscovery-reviewset-export?view=graph-rest-beta&preserve-view=true) documentos de um [conjunto de revisão](/graph/api/resources/ediscovery-reviewset?view=graph-rest-beta&preserve-view=true).
- Use a ação [addToReviewSet](/graph/api/ediscovery-reviewset-addtoreviewset?view=graph-rest-beta&preserve-view=true) para adicionar documentos em uma **sourceColection** a um **reviewSet**.
- [Aplique tags](/graph/api/ediscovery-reviewsetquery-applytags?view=graph-rest-beta&preserve-view=true) a documentos baseados em uma [consulta de conjunto de revisão](/graph/api/resources/ediscovery-reviewsetquery?view=graph-rest-beta&preserve-view=true).
- API de Descoberta eletrônica definida no namespace `microsoft.graph.ediscovery`.
- Modelo de permissões delegadas alterado de `User.Read` para `eDiscovery.Read.All` e `eDiscovery.ReadWrite.All`.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
- Atualizações do Intune de [fevereiro](https://developer.microsoft.com/graph/changelog/?from=2021-02-01&to=2021-02-28&filterBy=Corporate%20management) para a versão beta.
- Novas propriedades definidas pelo Intune no recurso do [dispositivo](/graph/api/resources/device?view=graph-rest-beta&preserve-view=true): **deviceCategory**, **deviceOwnership**, **domainName**, **enrollmentProfileName**, **enrollmentType**, **isRooted**, **managementType**, and **registrationDateTime**.

### <a name="education"></a>Educação
Use [educationAssignmentDefaults](/graph/api/resources/educationAssignmentDefaults?view=graph-rest-beta&preserve-view=true) para especificar as práticas padrão em uma tarefa para uma classe, por exemplo, hora de vencimento da tarefa, URL do canal para notificações sobre uma tarefa. Você ainda pode personalizar valores ao criar uma tarefa.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
- Use o recurso [smsAuthenticationMethodConfiguration](/graph/api/resources/smsAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true) para [obter](/graph/api/smsauthenticationmethodconfiguration-get?view=graph-rest-beta&preserve-view=true), [atualizar](/graph/api/smsauthenticationmethodconfiguration-update?view=graph-rest-beta&preserve-view=true) ou [excluir](/graph/api/smsauthenticationmethodconfiguration-delete?view=graph-rest-beta&preserve-view=true) as definições de configuração de uma política de autenticação de mensagem de texto em uma organização.
- Use o recurso [temporaryAccessPassAuthenticationMethodConfiguration](/graph/api/resources/temporaryaccesspassauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true) para [obter](/graph/api/temporaryaccesspassauthenticationmethodconfiguration-get?view=graph-rest-beta&preserve-view=true), [atualizar](/graph/api/temporaryaccesspassauthenticationmethodconfiguration-update?view=graph-rest-beta&preserve-view=true) ou [excluir](/graph/api/temporaryaccesspassauthenticationmethodconfiguration-delete?view=graph-rest-beta&preserve-view=true) as definições de configuração de uma política de autenticação de passe de acesso temporário em uma organização.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
- Atribua informações de geolocalização a um recurso de [pacote de acesso](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true) na [solicitação de atribuição de pacote de acesso](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true).
- Obtenha uma lista de todos os [ambientes de recursos de pacote de acesso](/graph/api/resources/accesspackageresourceenvironment?view=graph-rest-beta&preserve-view=true) que representam as geolocalizações que armazenam os recursos do Microsoft Office SharePoint Online.
- Use permissões de aplicativos (`EntitlementManagement.Read.All` ou `EntitlementManagement.ReadWrite.All`) para operações dos seguintes recursos:
  - [accessPackage](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true)
  - [accessPackageAssignment](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true)
  - [accessPackageAssignmentPolicy](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true)
  - [accessPackageAssignmentRequest](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true)
  - [accessPackageAssignmentResourceRole](/graph/api/resources/accesspackageassignmentresourcerole?view=graph-rest-beta&preserve-view=true)
  - [accessPackageCatalog](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta&preserve-view=true)
  - [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta&preserve-view=true)
  - [connectedOrganization](/graph/api/resources/connectedorganization?view=graph-rest-beta&preserve-view=true)
  - [entitlementManagementSettings](/graph/api/resources/entitlementmanagementsettings?view=graph-rest-beta&preserve-view=true)

### <a name="reports--microsoft-365-usage-reports"></a>Relatórios | Relatórios de uso do Microsoft 365
Obtenha mais propriedades incluídas em [relatórios detalhados para uso do site SharePoint](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta&preserve-view=true): anonymousLinkCount, companyLinkCount, externalSharing, geolocation, secureLinkForGuestCount, secureLinkForMemberCount, siteSensitivityLabelId, e unmanagedDevicePolicy.

### <a name="tasks-and-plans"></a>Tarefas e planos
- Defina até 25 categorias em um objeto de [detalhes do plano](/graph/api/resources/plannerplandetails?view=graph-rest-beta&preserve-view=true) para um plano. Para cada categoria, especifique um rótulo descritivo e associe tarefas em um plano com uma ou mais destas categorias. 
- Use uma [lista de participantes](/graph/api/resources/plannerRoster?view=graph-rest-beta&preserve-view=true) para representar um conjunto de usuários colaborando em um [plano](/graph/api/resources/plannerplan?view=graph-rest-beta&preserve-view=true). Use a relação **rosterPlans** para obter as listas de participantes das quais o usuário é um [membro](/graph/api/resources/plannerrostermember?view=graph-rest-beta&preserve-view=true). 
- Para planos que são apresentados em experiências fora do Planner, como o Microsoft Teams, especifique nos [detalhes de contexto do plano](/graph/api/resources/plannerplancontextdetails?view=graph-rest-beta&preserve-view=true) como exibir o link para o [contexto do plano](/graph/api/resources/plannerPlanContext?view=graph-rest-beta&preserve-view=true). 

### <a name="use-sdks"></a>Usar SDKs
Experimente a versão prévia do [Microsoft Graph Java SDK v3](https://github.com/microsoftgraph/msgraph-sdk-java/tree/feature/v3)! Para mais informações, confira a [postagem no blog](https://developer.microsoft.com/graph/blogs/announcing-the-public-preview-of-microsoft-graph-java-sdk-v3/) relacionada.



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
