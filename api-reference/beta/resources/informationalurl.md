---
title: tipo de recurso de informationalUrl
description: Informações básicas de perfil do aplicativo.
localization_priority: Normal
ms.openlocfilehash: 5085c144045631c530cbb66f5e1f27186a63b380
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513645"
---
# <a name="informationalurl-resource-type"></a>tipo de recurso de informationalUrl

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Informações básicas de perfil do aplicativo.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|Marketing|String| Link para a página de marketing do aplicativo. Por exemplo, https://www.contoso.com/app/marketing |
|Privacidade.|String| Link para a declaração de privacidade do aplicativo. Por exemplo, https://www.contoso.com/app/privacy |
|Suporte|String| Link para a página de suporte do aplicativo. Por exemplo, https://www.contoso.com/app/support |
|termsOfService|String| Link para os termos do aplicativo de instrução de serviço. Por exemplo, https://www.contoso.com/app/termsofservice |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationalUrl"
}-->

```json
{
  "marketing": "String",
  "privacy": "String",
  "support": "String",
  "termsOfService": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/informationalurl.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
