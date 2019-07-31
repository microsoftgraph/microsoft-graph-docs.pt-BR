---
title: tipo de recurso publicClientApplication
description: Especifica configurações para aplicativo não Web ou API Web. (por exemplo, móvel ou outro cliente público, como um aplicativo instalado em um dispositivo de área de trabalho)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4503e65777b41fc2f864cd818697b048e3c8e435
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965541"
---
# <a name="publicclientapplication-resource-type"></a>tipo de recurso publicClientApplication

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica configurações para aplicativo não Web ou API Web. (por exemplo, móvel ou outro cliente público, como um aplicativo instalado em um dispositivo de área de trabalho)

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|redirectUris|Coleção de cadeias de caracteres| Especifica as URLs às quais os tokens de usuário são enviados para entrar ou os URIs de redirecionamento aos quais os códigos de autorização OAuth 2,0 e tokens de acesso são enviados. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publicClientApplication"
}-->

```json
{
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "installedClient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
