---
title: tipo de recurso de oAuth2Permission
description: Representa um OAuth 2.0 delegada escopo de permissão. O OAuth 2.0 especificado escopos permissão delegada podem ser solicitados por aplicativos do cliente (por meio da coleção **requiredResourceAccess** no objeto de aplicativo) ao chamar um aplicativo de recurso. A propriedade **appRoles** da entidade servicePrincipal e da entidade do aplicativo é uma coleção de **oAuth2Permission**.
localization_priority: Normal
ms.openlocfilehash: 8d8bb0bb5af17b7322bd6be37ac48ae9edbeba42
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510810"
---
# <a name="oauth2permission-resource-type"></a>tipo de recurso de oAuth2Permission

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um OAuth 2.0 delegada escopo de permissão. O OAuth 2.0 especificado escopos permissão delegada podem ser solicitados por aplicativos do cliente (por meio da coleção **requiredResourceAccess** no objeto de [aplicativo](application.md) ) ao chamar um aplicativo de recurso. A propriedade **appRoles** da entidade [servicePrincipal](serviceprincipal.md) e da entidade do [aplicativo](application.md) é uma coleção de **oAuth2Permission**.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permission"
}-->

```json
{
  "adminConsentDescription": "string",
  "adminConsentDisplayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "type": "string",
  "userConsentDescription": "string",
  "userConsentDisplayName": "string",
  "value": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|adminConsentDescription|String|Texto de ajuda de permissão que aparece nas experiências de atribuição de consentimento e app admin.|
|adminConsentDisplayName|String|Nome para exibição da permissão que aparece nas experiências de atribuição de consentimento e app admin.|
|id|Guid|Identificador de permissão de escopo exclusiva dentro da coleção oauth2Permissions.|
|isEnabled|Boolean|Ao criar ou atualizar uma permissão, essa propriedade deverá ser definida como **true** (o que é o padrão). Para excluir uma permissão, essa propriedade primeiro deve ser definida como **false**.  Nesse momento, em uma chamada subsequente, a permissão pode ser removida.|
|type|String|Especifica se esta permissão de escopo pode ser consentiu por um usuário final, ou se é uma permissão de todo o inquilino deve ser consentiu por um administrador da empresa.  Valores possíveis são "Usuário" ou "Admin".|
|userConsentDescription|String|Texto de ajuda de permissão que aparece na experiência de consentimento do usuário final.|
|userConsentDisplayName|String|Nome para exibição da permissão que aparece na experiência de consentimento do usuário final.|
|valor|String|O valor da declaração escopo que deve esperar que o aplicativo de recurso no token de acesso OAuth 2.0.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/oauth2permission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
