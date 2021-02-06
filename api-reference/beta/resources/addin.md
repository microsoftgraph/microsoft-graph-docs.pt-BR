---
title: Tipo de recurso addIn
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 80c9e3c31a3bcc0d7b74e24373e5d1bb6947840f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134054"
---
# <a name="addin-resource-type"></a>Tipo de recurso addIn

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define o comportamento personalizado que um serviço de consumo pode usar para chamar um aplicativo em contextos específicos. Por exemplo, aplicativos que podem renderizar fluxos de [arquivos podem configurar os complementos para](/onedrive/developer/file-handlers/?view=odsp-graph-online) a funcionalidade de Manipulador de Arquivos. Isso permitirá que os serviços como o Microsoft 365 chamem o aplicativo no contexto de um documento no qual o usuário esteja trabalhando.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|guid||
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
