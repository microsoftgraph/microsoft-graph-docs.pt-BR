---
title: tipo de recurso usedInsight
description: Uma percepção representando documentos usados por um usuário específico. O insights retorna os documentos mais relevantes exibidos ou modificados por um usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 06dec4840edae33d51ddb64fb48d93aaa8ccdfda
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986061"
---
# <a name="usedinsight-resource-type"></a>tipo de recurso usedInsight

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma percepção representando documentos usados por um usuário específico. O insights retorna os documentos mais relevantes exibidos ou modificados por um usuário. Isso inclui documentos em:

- OneDrive for Business
- Microsoft Office SharePoint Online

## <a name="methods"></a>Methods

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar usados](../api/insights-list-used.md) |coleção [usedInsight](insights-used.md)| Obtenha uma lista de arquivos usados.|

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                      | Descrição  |
| -------------         |---------------            | -------------|
| id                    | String                    | Identificador exclusivo da relação. Somente leitura.        |
| lastUsed              | [usageDetails](insights-usagedetails.md)              | Informações sobre quando o item foi visualizado ou modificado pela última vez pelo usuário. Somente leitura.      |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | Propriedades que você pode usar para visualizar o documento em sua experiência. Somente leitura      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | Propriedades de referência do documento usado, como a URL e o tipo do documento. Somente leitura     |

## <a name="relationships"></a>Relações

| Propriedade      | Tipo          | Descrição  |
| ------------- |---------------| -------------|
| recurso      | coleção [Entity](entity.md)    | Usado para navegar até o item que foi usado. Para anexos de arquivo, o tipo é *Fileattachment*. Para anexos vinculados, o tipo é *driveItem*. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "resource"
  ],
  "@odata.type": "microsoft.graph.usedInsight"
}-->

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": { "@odata.type": "microsoft.graph.resourceVisualization" },
  "resourceReference": { "@odata.type": "microsoft.graph.resourceReference" }
}
```


