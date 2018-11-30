---
title: tipo de recurso de servicePrincipal
description: Representa uma instância de um aplicativo em um diretório. Herda de directoryObject.
ms.openlocfilehash: c3a08efb1dea1109bd32d59a479260e14089783d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038509"
---
# <a name="serviceprincipal-resource-type"></a>tipo de recurso de servicePrincipal

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa uma instância de um aplicativo em um diretório. Herda de [directoryObject](directoryobject.md).

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
|accountEnabled|Booliano| **true** se a conta de serviço principal estiver ativada; Caso contrário, **false**.            |
|appDisplayName|String|O nome de exibição exposto pelo aplicativo associado.|
|appId|Cadeia de caracteres|O identificador exclusivo para o aplicativo associado (sua propriedade **appId** ).|
|appRoleAssignmentRequired|Booliano|Especifica se um **appRoleAssignment** a um usuário ou grupo é necessária antes que o Azure AD emitirá um usuário ou um token de acesso ao aplicativo. Não anulável. |
|appRoles|coleção [appRole](approle.md)|As funções do aplicativo expostas pelo aplicativo associado. Para obter mais informações, consulte a definição da propriedade **appRoles** sobre a entidade de [aplicativo](application.md) . Não anulável. |
|displayName|String|O nome de exibição para a entidade de serviço.|
|errorUrl|String|            |
|home page|String|A URL para a home page do aplicativo associado.|
|keyCredentials|coleção [keyCredential](keycredential.md)|A coleção de credenciais de chave associado ao serviço principal. Não anulável.            |
|logoutUrl|String| Especifica a URL que será usada pelo serviço de autorização da Microsoft para logout um usuário usando o [canal de frente](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou protocolos de logout SAML.  |
|oauth2Permissions|coleção [oAuth2Permission](oauth2permission.md)|As permissões de OAuth 2.0 expostas pelo aplicativo associado. Para obter mais informações, consulte a definição da propriedade **oauth2Permissions** sobre a entidade de [aplicativo](application.md) . Não anulável.            |
|id|String|O identificador exclusivo para a entidade de serviço. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura.|
|passwordCredentials|coleção [passwordCredential](passwordcredential.md)|A coleção de credenciais de senha associadas a entidade de serviço. Não anulável. |
|preferredTokenSigningKeyThumbprint|String|Reservado para uso interno apenas. Não gravar ou caso contrário, contam com esta propriedade. Pode ser removido em futuras versões. |
|publisherName|Cadeia de caracteres|O nome de exibição do inquilino no qual o aplicativo associado for especificado.|
|replyUrls|String collection|As URLs que os tokens do usuário são enviados para entrada com o aplicativo associado ou o redirecionamento códigos de autorização de URIs que OAuth 2.0 e tokens de acesso são enviados para o aplicativo associado. Não anulável. |
|samlMetadataUrl|String| |
|servicePrincipalNames|String collection|Os URIs que identificam o aplicativo associado. Para mais informações, consulte [objetos de aplicativo e objetos de entidade de serviço](https://msdn.microsoft.com/library/azure/dn132633.aspx). Operador **any** é necessário para expressões de filtro propriedades de valores múltiplos.  Não anulável. |
|marcas|Coleção de cadeias de caracteres| Não anulável. |

## <a name="relationships"></a>Relações
| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|appRoleAssignedTo|[appRoleAssignment](approleassignment.md)|Entidades (usuários, grupos e entidades de serviço) que são atribuídas a essa entidade de serviço. Somente leitura.|
|appRoleAssignments|coleção [appRoleAssignment](approleassignment.md)|Aplicativos que a entidade de serviço é atribuída a. Somente leitura. Anulável.|
|createdObjects|Coleção [directoryObject](directoryobject.md)|Objetos de diretório criados por essa entidade de serviço. Somente leitura. Anulável.|
|memberOf|Coleção [directoryObject](directoryobject.md)|Funções que essa entidade de serviço é um membro de. Métodos HTTP: Obtenha somente leitura. Anulável.|
|oauth2PermissionGrants|coleção [oAuth2PermissionGrant](oauth2permissiongrant.md)|Concede de representação de usuário associado a essa entidade de serviço. Somente leitura. Anulável.|
|ownedObjects|Coleção [directoryObject](directoryobject.md)|Objetos de diretório pertencentes a essa entidade de serviço. Somente leitura. Anulável.|
|owners|Coleção [directoryObject](directoryobject.md)|Objetos de diretório que são proprietários dessa entidade de serviço. Os proprietários são um conjunto de usuários não seja o administrador que têm permissão para modificar esse objeto. Somente leitura. Anulável.|
|Política|coleção de [políticas](policy.md)|As políticas atribuídas para essa entidade de serviço.|

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter servicePrincipal](../api/serviceprincipal-get.md) | [servicePrincipal](serviceprincipal.md) |Leia as propriedades e os relacionamentos do objeto servicePrincipal.|
|[Lista servicePrincipals](../api/serviceprincipal-list.md) | coleção [servicePrincipal](serviceprincipal.md) | Recupere uma lista de objetos servicePrincipal. |
|[Criar appRoleAssignment](../api/serviceprincipal-post-approleassignments.md) |[appRoleAssignment](approleassignment.md)| Crie um novo appRoleAssignment pelo lançamento à coleção appRoleAssignments.|
|[Lista appRoleAssignments](../api/serviceprincipal-list-approleassignments.md) |coleção [appRoleAssignment](approleassignment.md)| Obtenha uma coleção de objetos appRoleAssignment.|
|[Listar createdObjects](../api/serviceprincipal-list-createdobjects.md) |Coleção [directoryObject](directoryobject.md)| Obtenha uma coleção de objetos createdObject.|
|[Listar memberOf](../api/serviceprincipal-list-memberof.md) |Coleção [directoryObject](directoryobject.md)| Obtenha os grupos que esse serviço principal é um membro direto da propriedade membro navegação.|
|[Membro de lista transitivo](../api/serviceprincipal-list-transitivememberof.md) |Coleção [directoryObject](directoryobject.md)| Liste os grupos que essa entidade de serviço é um membro de. Essa operação é transitiva e inclui os grupos que esse serviço principal é um membro aninhado do. |
|[Políticas de lista atribuída](../api/policy-list-assigned.md)| coleção de [políticas](policy.md)| Obtenha todas as diretivas atribuídas a este objeto.|
|[Lista oauth2PermissionGrants](../api/serviceprincipal-list-oauth2permissiongrants.md) |coleção [oAuth2PermissionGrant](oauth2permissiongrant.md)| Obtenha uma coleção de objetos oAuth2PermissionGrant.|
|[Listar ownedObjects](../api/serviceprincipal-list-ownedobjects.md) |Coleção [directoryObject](directoryobject.md)| Obtenha uma coleção de objetos ownedObject.|
|[Adicionar proprietário](../api/serviceprincipal-post-owners.md) |[directoryObject](directoryobject.md)| Crie um novo proprietário pelo lançamento à coleção proprietários.|
|[Listar proprietários](../api/serviceprincipal-list-owners.md) |Coleção [directoryObject](directoryobject.md)| Obtenha um proprietário de conjunto de objeto.|
|[Update](../api/serviceprincipal-update.md) | [servicePrincipal](serviceprincipal.md)  |Atualize o objeto servicePrincipal. |
|[Delete](../api/serviceprincipal-delete.md) | Nenhum |Exclua objeto servicePrincipal. |
|[checkMemberGroups](../api/serviceprincipal-checkmembergroups.md)|Coleção de cadeias de caracteres||
|[getMemberGroups](../api/serviceprincipal-getmembergroups.md)|Coleção de cadeias de caracteres||
|[getMemberObjects](../api/serviceprincipal-getmemberobjects.md)|Coleção de cadeias de caracteres||
|[delta](../api/serviceprincipal-delta.md)|coleção servicePrincipal| Obtenha as alterações incrementais para entidades de serviço. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
