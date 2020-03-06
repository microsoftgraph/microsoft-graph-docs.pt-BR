---
title: tipo de recurso publicClientApplication
description: Especifica configurações para aplicativo não Web ou API Web. (por exemplo, móvel ou outro cliente público, como um aplicativo instalado em um dispositivo de área de trabalho)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: fc920fe09a891248310e8acebafb4f2da4d36723
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533942"
---
# <a name="publicclientapplication-resource-type"></a>tipo de recurso publicClientApplication

Namespace: microsoft.graph

Especifica configurações para aplicativo não Web ou API não Web (por exemplo, dispositivos móveis ou outros clientes públicos, como um aplicativo instalado em um dispositivo Desktop).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|redirectUris|String collection| Especifica as URLs nas quais os tokens de usuário são enviados para entrada ou os URIs de redirecionamento nos quais os códigos de autorização OAuth 2,0 e tokens de acesso são enviados. |

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
