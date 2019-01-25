---
title: tipo de recurso de requiredResourceAccess
description: Especifica o conjunto de escopos de permissão de OAuth 2.0 e funções de aplicativo em que um aplicativo requer acesso ao recurso especificado. Os escopos de permissão especificados OAuth 2.0 podem ser solicitados por aplicativos do cliente (por meio da coleção **requiredResourceAccess** ) quando um aplicativo de recurso de chamada. A propriedade **requiredResourceAccess** da entidade do aplicativo é uma coleção de **ReqiredResourceAccess**.
localization_priority: Normal
ms.openlocfilehash: a2c7e337bbe441275f395c2333b8cee918e6b9da
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512966"
---
# <a name="requiredresourceaccess-resource-type"></a>tipo de recurso de requiredResourceAccess

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica o conjunto de escopos de permissão de OAuth 2.0 e funções de aplicativo em que um aplicativo requer acesso ao recurso especificado. Os escopos de permissão especificados OAuth 2.0 podem ser solicitados por aplicativos do cliente (por meio da coleção **requiredResourceAccess** ) quando um aplicativo de recurso de chamada. A propriedade **requiredResourceAccess** da entidade do [aplicativo](application.md) é uma coleção de **ReqiredResourceAccess**.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}-->

```json
{
  "resourceAccess": [{"@odata.type": "microsoft.graph.resourceAccess"}],
  "resourceAppId": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|resourceAccess|Coleção [ResourceAccess](resourceaccess.md)|A lista de escopos de permissão OAuth2.0 e funções de aplicativo que requer que o aplicativo do recurso especificado.|
|resourceAppId|String|O identificador exclusivo para o recurso que o aplicativo exija acesso à.  Este deve ser igual a **appId** declaradas na aplicação de recurso de destino.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/requiredresourceaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
