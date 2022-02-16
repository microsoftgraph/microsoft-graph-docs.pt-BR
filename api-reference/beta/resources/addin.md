---
title: Tipo de recurso addIn
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 26dae722e9f706c5aa5ea89dfd375775975e7d11
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854449"
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
  "id": "GUID",
  "properties": [{"@odata.type": "microsoft.graph.keyValue"}],
  "type": "String"
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
