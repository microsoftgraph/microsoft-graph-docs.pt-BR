---
title: tipo de recurso de tendência
description: Relação avançada conectando um usuário a documentos que estão em tendência ao usuário (são relevantes para o usuário). Os arquivos do OneDrive e os arquivos armazenados em sites de equipe do SharePoint podem ser tendências em torno do usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 7a9c9cf9323aa24bd50c1f817a1293088e1a4373
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054767"
---
# <a name="trending-resource-type"></a>tipo de recurso de tendência

Namespace: microsoft.graph

Relação avançada conectando um usuário a documentos que estão em tendência ao usuário (são relevantes para o usuário). Os arquivos do OneDrive e os arquivos armazenados em sites de equipe do SharePoint podem ser tendências em torno do usuário.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar tendências](../api/insights-list-trending.md) |coleção [tendências](insights-trending.md) | Obtenha uma lista de arquivos de tendência.|

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                              | Descrição  |
| ------------- |---------------                    | -------------|
| id                    | String                    | Identificador exclusivo da relação. Somente leitura.        |
| weight                | Duplo                    | Valor que indica quanto o documento está em tendência no momento. Quanto maior o número, mais o documento está atualmente em tendência ao usuário (o que é mais relevante). Os documentos retornados são classificados por esse valor.  |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)    | Propriedades que você pode usar para visualizar o documento em sua experiência. |
| resourceReference     | [resourceReference](insights-resourcereference.md)        | Propriedades de referência do documento de tendência, como a URL e o tipo do documento. |
| lastModifiedDateTime  | DateTimeOffset            | |
## <a name="relationships"></a>Relações

| Propriedade      | Tipo          | Descrição  |
| ------------- |---------------| -------------|
| recurso      | entidade        | Usado para navegar para o documento de tendência. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "resource"
  ],
  "@odata.type": "microsoft.graph.trending"
}-->

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": {"@odata.type": "microsoft.graph.resourceVisualization"},
  "resourceReference": {"@odata.type": "microsoft.graph.resourceReference"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

