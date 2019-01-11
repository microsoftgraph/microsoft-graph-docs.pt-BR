---
title: tipo de recurso de oAuth2PermissionGrant
description: Representa os escopos de OAuth 2.0 (permissões delegadas) que tiverem sido concedidos a um aplicativo (representado por uma entidade de serviço) como parte do processo de consentimento do usuário ou administrador.
localization_priority: Normal
ms.openlocfilehash: 835e4a2c1a8d19c9c21e706adbf2f10a6a505bb3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884445"
---
# <a name="oauth2permissiongrant-resource-type"></a>tipo de recurso de oAuth2PermissionGrant

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa os escopos de OAuth 2.0 (permissões delegadas) que tiverem sido concedidos a um aplicativo (representado por uma entidade de serviço) como parte do processo de consentimento do usuário ou administrador.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant"
}-->

```json
{
  "clientId": "string",
  "consentType": "string",
  "expiryTime": "String (timestamp)",
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string",
  "startTime": "String (timestamp)"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|clientId|Cadeia de caracteres| A id da entidade de segurança do serviço concedido consentimento para representar o usuário ao acessar o recurso (representado pela propriedade resourceId). |
|consentType|Cadeia de caracteres| Indica se o consentimento foi fornecido pelo administrador (em nome da organização) ou por um indivíduo. Os valores possíveis são *AllPrincipals* ou *Principal*. |
|expiryTime|DateTimeOffset| Atualmente, o valor de tempo de expiração será ignorado. |
|id|Cadeia de caracteres| Identificador exclusivo. Somente leitura.|
|principalId|Cadeia de caracteres| Este valor é null se consentType for *AllPrincipals* e o consentimento se aplica a todos os usuários na organização. Se consentType for *Principal*, essa propriedade especifica a id do usuário que concedidas consentimento e aplica-se somente para esse usuário. |
|resourceId|Cadeia de caracteres| Especifica a id da entidade de serviço recurso ao qual tem permissão para acesso. |
|escopo|Cadeia de caracteres| Especifica o valor da declaração [escopo](/graph/permissions-reference) que o aplicativo de recurso deve esperar que no token de acesso OAuth 2.0. Por exemplo, *User.Read* |
|startTime|DateTimeOffset| Atualmente, o valor de hora de início será ignorado. |

## <a name="relationships"></a>Relações
Nenhum


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter oAuth2PermissionGrant](../api/oauth2permissiongrant-get.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) |Leia as propriedades e os relacionamentos do objeto oAuth2PermissionGrant.|
|[Lista oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md) | coleção [oAuth2PermissionGrant](oauth2permissiongrant.md) | Recupere uma lista de objetos oauth2PermissionGrant. |
|[Atualizar oAuth2PermissionGrant](../api/oauth2permissiongrant-update.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) |Atualize o objeto oAuth2PermissionGrant. |
|[Excluir oAuth2PermissionGrant](../api/oauth2permissiongrant-delete.md) | Nenhum |Exclua objeto oAuth2PermissionGrant. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
