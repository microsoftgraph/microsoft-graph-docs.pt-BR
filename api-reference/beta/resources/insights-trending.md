---
title: tipo de recurso de tendência
description: Relação avançada conectando um usuário a documentos que estão em tendência ao usuário (são relevantes para o usuário). Os arquivos do OneDrive e os arquivos armazenados em sites de equipe do SharePoint podem ser tendências em torno do usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 07fe0f50d6961f0fce6c426c7fb2431f17127bf7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551306"
---
# <a name="trending-resource-type"></a>tipo de recurso de tendência

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Relação avançada conectando um usuário a documentos que estão em tendência ao usuário (são relevantes para o usuário). Os arquivos do OneDrive e os arquivos armazenados em sites de equipe do SharePoint podem ser tendências em torno do usuário.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar tendências](../api/insights-list-trending.md) |coleção [insights_trending](insights-trending.md)| Obtenha uma lista de arquivos de tendência.|

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                              | Descrição  |
| ------------- |---------------                    | -------------|
| id                    | String                    | Identificador exclusivo da relação. Somente leitura.        |
| weight                | Duplo                    | Valor que indica quanto o documento está em tendência no momento. Quanto maior o número, mais o documento está atualmente em tendência ao usuário (o que é mais relevante). Os documentos retornados são classificados por esse valor.  |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)    | Propriedades que você pode usar para visualizar o documento em sua experiência. |
| resourceReference     | [resourceReference](insights-resourcereference.md)        | Propriedades de referência do documento de tendência, como a URL e o tipo do documento. |

## <a name="relationships"></a>Relações

| Propriedade      | Tipo          | Descrição  |
| ------------- |---------------| -------------|
| recurso      | Entidade        | Usado para navegar para o documento de tendência. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-trending.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
