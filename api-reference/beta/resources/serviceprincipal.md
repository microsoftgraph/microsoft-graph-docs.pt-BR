---
title: Tipo de recurso servicePrincipal
description: Representa uma instância de um aplicativo em um diretório. Herda do directoryObject.
localization_priority: Priority
ms.openlocfilehash: cd0ac4d440b2e10f935c02393419754989394816
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641152"
---
# <a name="serviceprincipal-resource-type"></a>Tipo de recurso servicePrincipal

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma instância de um aplicativo em um diretório. Herda do [directoryObject](directoryobject.md).

Esse recurso permite:

- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/serviceprincipal-delta.md).

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "appRoleAssignedTo",
    "appRoleAssignments",
    "createdObjects",
    "createdOnBehalfOf",
    "memberOf",
    "oauth2PermissionGrants",
    "ownedObjects",
    "owners"
  ],
  "@odata.type": "microsoft.graph.serviceprincipal"
}-->

```json
{
  "accountEnabled": true,
  "addIns": [{"@odata.type": "microsoft.graph.addIn"}],
  "appDisplayName": "string",
  "appId": "string",
  "appOwnerOrganizationId": "guid",
  "appRoleAssignmentRequired": true,
  "displayName": "string",
  "errorUrl": "string",
  "homepage": "string",
  "id": "string (identifier)",
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "logoutUrl": "string",
  "oauth2Permissions": [{"@odata.type": "microsoft.graph.oAuth2Permission"}],
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "preferredTokenSigningKeyThumbprint": "string",
  "publisherName": "string",
  "replyUrls": ["string"],
  "samlMetadataUrl": "string",
  "servicePrincipalNames": ["string"],
  "tags": ["string"]
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo |Descrição|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| **True** se a entidade de serviço estiver habilitada; caso contrário, **false**.            |
|appDisplayName|String|O nome de exibição exposto pelo aplicativo associado.|
|appId|String|O identificador exclusivo do aplicativo associado (sua propriedade **appId**).|
|appRoleAssignmentRequired|Boolean|Especifica se um **appRoleAssignment** de um usuário ou grupo é necessário antes que o Azure AD emita um token de usuário ou de acesso ao aplicativo. Não anulável. |
|appRoles|[appRole](approle.md) collection|As funções do aplicativo expostas pelo aplicativo associado. Para obter mais informações, confira definição da propriedade **appRoles** na entidade [aplicativo](application.md). Não anulável. |
|displayName|String|O nome de exibição da entidade de serviço.|
|errorUrl|String|            |
|homepage|String|A URL da home page do aplicativo associado.|
|keyCredentials|[keyCredential](keycredential.md) collection|A coleção de credenciais principais associada à entidade de serviço. Não anulável.            |
|logoutUrl|String| Especifica a URL que será usada pela autorização do serviço da Microsoft para fazer logoff de um usuário usando protocolos de logoff [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou SAML.  |
|oauth2Permissions|[oAuth2Permission](oauth2permission.md) collection|As permissões OAuth 2.0 expostas pelo aplicativo associado. Para obter mais informações, confira a definição da propriedade **oauth2Permissions** na entidade [aplicativo](application.md). Não anulável.            |
|id|String|O identificador exclusivo da entidade de serviço. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura.|
|passwordCredentials|[passwordCredential](passwordcredential.md) collection|A coleção de credenciais de senha associada à entidade de serviço. Não anulável. |
|preferredTokenSigningKeyThumbprint|String|Reservado apenas para uso interno. Não escreva ou dependa de alguma forma dessa propriedade. Pode ser removida em versões futuras. |
|publisherName|String|O nome de exibição do locatário no qual o aplicativo associado está especificado.|
|replyUrls|String collection|As URLs às quais os tokens de usuário são enviados para entrar com aplicativo associado ou os URIs de redirecionamento aos quais os códigos de autorização do OAuth 2.0 e tokens de acesso são enviados para o aplicativo associado. Não anulável. |
|samlMetadataUrl|String| |
|servicePrincipalNames|String collection|Os URIs que identificam o aplicativo associado. Para obter mais informações, confira [Objetos do aplicativo e da entidade de serviço](https://msdn.microsoft.com/library/azure/dn132633.aspx). O operador **any** é necessário para expressões de filtro em propriedades de vários valores.  Não anulável. |
|tags|String collection| Não anulável. |

## <a name="relationships"></a>Relações
| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|appRoleAssignedTo|[appRoleAssignment](approleassignment.md)|Entidades (usuários, grupos e entidades de serviço) que são atribuídas a essa entidade de serviço. Somente leitura.|
|appRoleAssignments|[appRoleAssignment](approleassignment.md) collection|Aplicativos aos quais a entidade de serviço é atribuída. Somente leitura. Anulável.|
|createdObjects|[directoryObject](directoryobject.md) collection|Objetos de diretório criados pela entidade de serviço. Somente leitura. Anulável.|
|memberOf|[directoryObject](directoryobject.md) collection|Funções das quais essa entidade de serviço é membro. Métodos HTTP: GET somente leitura. Anulável.|
|oauth2PermissionGrants|[oAuth2PermissionGrant](oauth2permissiongrant.md) collection|Concessões da representação de usuário associadas a essa entidade de serviço. Somente leitura. Anulável.|
|ownedObjects|[directoryObject](directoryobject.md) collection|Objetos de diretório que pertencem a essa entidade de serviço. Somente leitura. Anulável.|
|owners|[directoryObject](directoryobject.md) collection|Objetos de diretório que são proprietários dessa entidade de serviço. Os proprietários são um conjunto de usuários não administradores com permissão para modificar esse objeto. Somente leitura. Anulável.|
|política|[policy](policy.md) collection|As políticas atribuídas a essa entidade de serviço.|

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Get servicePrincipal](../api/serviceprincipal-get.md) | [servicePrincipal](serviceprincipal.md) |Leia as propriedades e as relações do objeto servicePrincipal.|
|[List servicePrincipals](../api/serviceprincipal-list.md) | [servicePrincipal](serviceprincipal.md) collection | Recupere uma lista de objetos servicePrincipal. |
|[Create appRoleAssignment](../api/serviceprincipal-post-approleassignments.md) |[appRoleAssignment](approleassignment.md)| Crie um novo appRoleAssignment postando-o na coleção appRoleAssignments.|
|[List appRoleAssignments](../api/serviceprincipal-list-approleassignments.md) |[appRoleAssignment](approleassignment.md) collection| Obtenha uma coleção de objeto appRoleAssignment.|
|[List createdObjects](../api/serviceprincipal-list-createdobjects.md) |[directoryObject](directoryobject.md) collection| Obtenha uma coleção de objeto createdObject.|
|[List memberOf](../api/serviceprincipal-list-memberof.md) |[directoryObject](directoryobject.md) collection| Obtenha grupos dos quais essa entidade de serviço é membro direto da propriedade de navegação memberOf.|
|[List transitive memberOf](../api/serviceprincipal-list-transitivememberof.md) |[directoryObject](directoryobject.md) collection| Liste os grupos dos quais essa entidade de serviço é membro. Essa operação é transitiva e inclui os grupos dos quais essa entidade de serviço é um membro aninhado. |
|[List assigned policies](../api/policy-list-assigned.md)| Coleção [policy](policy.md)| Obtenha todas as políticas atribuídas a esse objeto.|
|[List oauth2PermissionGrants](../api/serviceprincipal-list-oauth2permissiongrants.md) |[oAuth2PermissionGrant](oauth2permissiongrant.md) collection| Obtenha uma coleção de objeto oAuth2PermissionGrant.|
|[List ownedObjects](../api/serviceprincipal-list-ownedobjects.md) |[directoryObject](directoryobject.md) collection| Obtenha uma coleção de objeto ownedObject.|
|[Add owner](../api/serviceprincipal-post-owners.md) |[directoryObject](directoryobject.md)| Crie um novo proprietário postando na coleção owners.|
|[Listar proprietários](../api/serviceprincipal-list-owners.md) |[directoryObject](directoryobject.md) collection| Obtenha uma coleção de objeto owner.|
|[Update](../api/serviceprincipal-update.md) | [servicePrincipal](serviceprincipal.md)  |Atualize o objeto servicePrincipal. |
|[Delete](../api/serviceprincipal-delete.md) | Nenhum |Exclua o objeto servicePrincipal. |
|[checkMemberGroups](../api/serviceprincipal-checkmembergroups.md)|String collection||
|[getMemberGroups](../api/serviceprincipal-getmembergroups.md)|String collection||
|[getMemberObjects](../api/serviceprincipal-getmemberobjects.md)|String collection||
|[delta](../api/serviceprincipal-delta.md)|servicePrincipal collection| Obtenha alterações incrementais para entidades de serviço. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/serviceprincipal.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
