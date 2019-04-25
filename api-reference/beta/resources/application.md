---
title: tipo de recurso do aplicativo
description: 'Representa um aplicativo. Qualquer aplicativo que terceirize a autenticação no Azure Active Directory (Azure AD) deve estar registrado em um diretório. O registro do aplicativo envolve informar o Azure AD sobre seu aplicativo, incluindo a URL onde ele está localizado, a URL para enviar respostas após a autenticação, o URI para identificar seu aplicativo e muito mais. Para saber mais, confira Noções básicas de como registrar um aplicativo no Azure AD. Herda de directoryObject. '
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 694f6b12dd8fe1fd59f12cafebd47c842a4077cb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548198"
---
# <a name="application-resource-type"></a>tipo de recurso do aplicativo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um aplicativo. Qualquer aplicativo que terceirize a autenticação no Azure Active Directory (Azure AD) deve estar registrado em um diretório. O registro do aplicativo envolve informar o Azure AD sobre seu aplicativo, incluindo a URL onde ele está localizado, a URL para enviar respostas após a autenticação, o URI para identificar seu aplicativo e muito mais. Para saber mais, confira [Noções básicas de como registrar um aplicativo no Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-authentication-scenarios/#basics-of-registering-an-application-in-azure-ad). Herda de [directoryObject](directoryobject.md). 

> **Observação:** atualmente, as alterações no tipo de recurso do aplicativo encontram-se em desenvolvimento. Para saber mais, confira [Problemas conhecidos com o Microsoft Graph](/graph/known-issues#application-and-serviceprincipal-api-changes).

Esse recurso permite:

- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/application-delta.md).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Obter aplicativo](../api/application-get.md) | application |Leia as propriedades e as relações do objeto application.|
|[Criar aplicativo](../api/application-post-applications.md) | application | Cria (registra) um novo aplicativo.|
|[Listar aplicativos](../api/application-list.md) | application | Recupere a lista de aplicativos na organização. |
|[Atualizar aplicativo](../api/application-update.md) | application |Atualize o objeto application. |
|[Excluir aplicativo](../api/application-delete.md) | Nenhum |Exclua o objeto application. |
|[Listar políticas atribuídas](../api/policy-list-assigned.md)| Coleção [policy](policy.md)| Obtenha todas as políticas atribuídas a esse objeto.|
|[Criar proprietário](../api/application-post-owners.md) |[directoryObject](directoryobject.md)| Crie um novo proprietário postando na coleção owners.|
|[Listar proprietários](../api/application-list-owners.md) |Coleção [directoryObject](directoryobject.md)| Obtenha uma coleção de objetos owner.|
|[delta](../api/application-delta.md)|Coleção application| Obtenha alterações incrementais para aplicativos. |
|[Criar chamada](../api/application-post-calls.md)|[call](call.md)|Crie uma nova chamada postando na coleção calls.|
|[Criar reunião online](../api/application-post-onlinemeetings.md)|[onlineMeeting](onlinemeeting.md)|Crie uma nova reunião online postando na coleção onlineMeetings.|

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|api|[api](api.md)| Especifica configurações para um aplicativo de API. |
|appId| String | O identificador exclusivo para o aplicativo que está atribuído a um aplicativo pelo Azure AD. Não anulável. Somente leitura. |
|appRoles|Coleção [appRole](approle.md)|A coleção de funções de aplicativo que um aplicativo pode declarar. Essas funções podem ser atribuídas a usuários, grupos ou entidades de serviço. Não anulável.|
|createdDateTime|DateTimeOffset| A data e a hora que o aplicativo foi registrado. |
|deletedDateTime|DateTimeOffset| A data e a hora que o aplicativo foi excluído. |
|displayName|String|O nome de exibição do aplicativo. |
|id|String|O identificador exclusivo do aplicativo. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura. |
|identifierUris|Coleção String| Os URIs que identificam o aplicativo. Para saber mais, confira [Objetos do aplicativo e objetos da entidade de serviço](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/). O operador *any* é obrigatório para expressões de filtro em propriedades de vários valores. Não anulável. |
|informações |[informationalUrl](informationalurl.md)| Informações de perfil básicas do aplicativo. |
|isFallbackPublicClient|Booliano| Especifica o tipo de aplicativo de fallback como cliente público, como um aplicativo instalado em execução em um dispositivo móvel. O valor padrão é *false*. Isso significa que o tipo de aplicativo de fallback é cliente confidencial como o aplicativo Web. Há determinados cenários em que o Azure AD não pode determinar o tipo de aplicativo cliente (por exemplo, o fluxo [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3), no qual ele é configurado sem especificar um URI de redirecionamento). Nesses casos, o Azure AD interpretará o tipo de aplicativo com base no valor dessa propriedade.|
|keyCredentials|Coleção [keyCredential](keycredential.md)|A coleção de credenciais chaves associada ao aplicativo Não anulável. |
|logo|Stream|O principal logotipo do aplicativo. Não anulável. |
|optionalClaims|optionalClaims| Reserved for future use. |
|orgRestrictions|Coleção String| Reserved for future use. |
|parentalControlSettings|[parentalControlSettings](parentalcontrolsettings.md) |Especifica as configurações de controle parental de um aplicativo.|
|passwordCredentials|Coleção [passwordCredential](passwordcredential.md)|A coleção de credenciais de senha associada ao aplicativo. Não anulável.|
|publicClient|[publicClient](publicclient.md)| Especifica configurações para clientes instalados, como dispositivos móveis ou da área de trabalho. |
|publisherDomain| String | O domínio do publicador verificado para o aplicativo. Somente leitura.|
|requiredResourceAccess|[requiredResourceAccess](requiredresourceaccess.md) collection|Especifica os recursos para os quais esse aplicativo requer acesso e o conjunto de escopos de permissão e funções de aplicativo do OAuth necessários em cada um desses recursos. Essa pré-configuração de acesso necessário aos recursos impulsiona a experiência de consentimento. Não anulável.|
|signInAudience | String | Especifica a quais contas da Microsoft são compatíveis com o aplicativo atual. Os valores compatíveis são:<ul><li>**AzureADMyOrg**: usuários com uma conta corporativa ou de estudante da Microsoft no locatário do Azure AD da organização (ou seja, locatário único)</li><li>**AzureADMultipleOrgs**: usuários com uma conta corporativa ou de estudante da Microsoft no locatário do Azure AD da organização (ou seja, multilocatário)</li> <li>**AzureADandPersonalMicrosoftAccount**: usuários com uma conta pessoal da Microsoft ou uma conta corporativa ou de estudante no locatário do Azure AD de qualquer organização</li></ul> | `AzureADandPersonalMicrosoftAccount` |
|marcações|Coleção String| Sequências personalizadas que podem ser usadas para categorizar e identificar o aplicativo. |
|web|[web](web.md)| Especifica configurações para um aplicativo Web. |

## <a name="relationships"></a>Relações

| Relação | Tipo | Descrição |
|:---------------|:--------|:----------|
|calls           |Coleção [call](call.md)                   |Somente leitura. Anulável.|
|connectorGroup|[connectorGroup](connectorgroup.md)| O connectorGroup que o aplicativo está usando com o Proxy de aplicativo do Azure AD. Anulável.|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| Somente leitura.|
|onlineMeetings  |Coleção [onlineMeeting](onlinemeeting.md)|Somente leitura. Anulável.|
|owners|Coleção [directoryObject](directoryobject.md)|Objetos de diretório que são proprietários do aplicativo. Os proprietários são um conjunto de usuários não administradores e que têm permissão para modificar esse objeto. Requer a versão 2013-11-08 ou mais recente. Somente leitura. Anulável.|
|política|Coleção [policy](policy.md)|As políticas atribuídas a esse aplicativo.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "createdOnBehalfOf",
    "owners"
  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "api": {"@odata.type": "microsoft.graph.apiApplication"},
  "appId": "String",
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}],
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "identifierUris": ["String"],
  "info": {"@odata.type": "microsoft.graph.informationalUrl"},
  "isFallbackPublicClient": true,
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "logo": "Stream",
  "optionalClaims": [{"@odata.type": "microsoft.graph.optionalClaims"}],
  "orgRestrictions": ["Guid"],
  "parentalControlSettings": [{"@odata.type": "microsoft.graph.parentalControlSettings"}],
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "preAuthorizedApplications": [{"@odata.type": "microsoft.graph.preAuthorizedApplication"}],
  "publicClient": {"@odata.type": "microsoft.graph.publicClientApplication"},
  "publisherDomain": "String",
  "requiredResourceAccess": [{"@odata.type": "microsoft.graph.requiredResourceAccess"}],
  "signInAudience": "String",
  "tags": ["String"],
  "web": {"@odata.type": "microsoft.graph.webApplication"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/application.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
