---
title: Tipo de recurso usedInsight
description: Uma visão que representa documentos usados por um usuário específico. As percepções retornam os documentos mais relevantes que um usuário exibiu ou modificou.
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 4163fa241a31b259e87c312b90f07ed05893f682
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036484"
---
# <a name="usedinsight-resource-type"></a>Tipo de recurso usedInsight

Namespace: microsoft.graph

Uma visão que representa documentos usados por um usuário específico. As percepções retornam os documentos mais relevantes que um usuário exibiu ou modificou. Isso inclui documentos em:

- OneDrive for Business
- SharePoint

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar usados](../api/insights-list-used.md) |coleção [usedInsight](insights-used.md)| Obter uma lista de arquivos usados.|

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                      | Descrição  |
| -------------         |---------------            | -------------|
| id                    | Cadeia de caracteres                    | Identificador exclusivo da relação. Somente leitura.        |
| lastUsed              | [usageDetails](insights-usagedetails.md)              | Informações sobre quando o item foi exibido pela última vez ou modificado pelo usuário. Somente leitura.      |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | Propriedades que você pode usar para visualizar o documento em sua experiência. Somente leitura      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | Fazer referência a propriedades do documento usado, como a URL e o tipo do documento. Somente leitura     |

## <a name="relationships"></a>Relações

| Propriedade      | Tipo          | Descrição  |
| ------------- |---------------| -------------|
| recurso      | [coleção entity](entity.md)    | Usado para navegar até o item usado. Para anexos de arquivo, o tipo *é fileAttachment*. Para anexos vinculados, o tipo é *driveItem*. |

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

