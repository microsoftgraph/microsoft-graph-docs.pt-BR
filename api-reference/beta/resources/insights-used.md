---
title: tipo de recurso usedInsight
description: Uma percepção representando documentos usados por um usuário específico. O insights retorna os documentos mais relevantes que um usuário tenha exibido ou acessado.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 407822dc4ff3f0536b0cbff3bf2894ad96d5d878
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333549"
---
# <a name="usedinsight-resource-type"></a>tipo de recurso usedInsight

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma percepção representando documentos usados por um usuário específico. O insights retorna os documentos mais relevantes que um usuário tenha exibido ou acessado. Isso inclui documentos em:

- OneDrive for Business
- SharePoint

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar usados](../api/insights-list-used.md) |coleção [usedInsight](insights-used.md)| Obtenha uma lista de arquivos usados.|

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                      | Descrição  |
| -------------         |---------------            | -------------|
| id                    | String                    | Identificador exclusivo da relação. Somente leitura.        |
| lastUsed              | [usageDetails](insights-usagedetails.md)              | Informações sobre quando o item foi exibido e modificado pela última vez pelo usuário. Somente leitura.     |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | Propriedades que você pode usar para visualizar o documento em sua experiência. Somente leitura      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | Propriedades de referência do documento usado, como a URL e o tipo do documento. Somente leitura     |

## <a name="relationships"></a>Relações

| Propriedade      | Tipo          | Descrição  |
| ------------- |---------------| -------------|
| recurso      | coleção [Entity](entity.md)    | Usado para navegar até o item que foi usado. Para anexos de arquivo, o tipo ** é fileattachment. Para anexos vinculados, o tipo é *driveItem*. |

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
