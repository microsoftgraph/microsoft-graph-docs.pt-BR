---
title: tipo de recurso oAuth2Permission
description: Representa um escopo de permissão delegada do OAuth 2,0. Os escopos de permissão delegada do OAuth 2,0 especificado podem ser solicitados por aplicativos cliente (por meio da coleção **requiredResourceAccess** no objeto Application) ao chamar um aplicativo de recurso. A propriedade **appRoles** da entidade servicePrincipalName e da entidade Application é uma coleção de **oAuth2Permission**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 16dfa93d13127d585cd5b56a56987bb22ab39d8f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009570"
---
# <a name="oauth2permission-resource-type"></a>tipo de recurso oAuth2Permission

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um escopo de permissão delegada do OAuth 2,0. Os escopos de permissão delegada do OAuth 2,0 especificado podem ser solicitados por aplicativos cliente (por meio da coleção **requiredResourceAccess** no objeto [Application](application.md) ) ao chamar um aplicativo de recurso. A propriedade **appRoles** da entidade [servicePrincipalName](serviceprincipal.md) e da entidade [Application](application.md) é uma coleção de **oAuth2Permission**.


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
|adminConsentDescription|String|Texto de ajuda de permissão que aparece nas experiências de atribuição de aplicativo e consentimento de administrador.|
|adminConsentDisplayName|String|Nome para exibição da permissão que aparece nas experiências de atribuição de aplicativo e consentimento de administrador.|
|id|Guid|Identificador de permissão de escopo exclusivo dentro da coleção oauth2Permissions.|
|isEnabled|Boolean|Ao criar ou atualizar uma permissão, essa propriedade deve ser definida como **true** (que é o padrão). Para excluir uma permissão, essa propriedade deve ser definida primeiro como **false**.  Nesse ponto, em uma chamada subsequente, a permissão pode ser removida.|
|type|String|Especifica se essa permissão de escopo pode ser consentida por um usuário final ou se é uma permissão em todo o locatário que deve ser consentida pelo administrador da empresa.  Os valores possíveis são "user" ou "admin".|
|userConsentDescription|String|Texto de ajuda de permissão que aparece na experiência de consentimento do usuário final.|
|userConsentDisplayName|String|Nome para exibição da permissão que aparece na experiência de consentimento do usuário final.|
|value|Cadeia de caracteres|O valor da declaração do escopo que o aplicativo de recursos deve esperar no token de acesso do OAuth 2,0.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
