---
title: tipo de recurso addIn
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: a5f0d078bf73603ccedf905c2cd496223fbd426e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508412"
---
# <a name="addin-resource-type"></a>tipo de recurso addIn

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define o comportamento personalizado que um serviço de consumo pode usar para chamar um aplicativo em contextos específicos. Por exemplo, aplicativos que podem renderizar fluxos de arquivos [podem configurar suplementos](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) para a funcionalidade do manipulador de arquivos. Isso permitirá que serviços como o Office 365 chamem o aplicativo no contexto de um documento em que o usuário esteja trabalhando.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|#c0||
|properties|Coleção [KeyValue](keyvalue.md)||
|type|string||

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addIn"
}-->

```json
{
  "id": "guid",
  "properties": [{"@odata.type": "microsoft.graph.keyValue"}],
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "addIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
