---
title: tipo de recurso de tendência
description: Rico relacionamento conectando um usuário a documentos que têm tendências em torno do usuário (são relevantes para o usuário). Os arquivos do OneDrive e os arquivos armazenados em sites de equipe do Microsoft Office SharePoint Online podem ser uma tendência em torno do usuário.
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 74b47304e70a31014144b0c52fef46d6105f7e04
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723909"
---
# <a name="trending-resource-type"></a>tipo de recurso de tendência

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Rico relacionamento conectando um usuário a documentos que têm tendências em torno do usuário (são relevantes para o usuário). Os arquivos do OneDrive e os arquivos armazenados em sites de equipe do Microsoft Office SharePoint Online podem ser uma tendência em torno do usuário.

## <a name="methods"></a>Methods

| Método                                            | Tipo de retorno                                 | Descrição                   |
| :------------------------------------------------ | :------------------------------------------ | :---------------------------- |
| [Listar tendências](../api/insights-list-trending.md) | coleção [tendências](insights-trending.md)  | Obter uma lista de arquivos de tendência. |

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                                                       | Descrição                                                                                                                                                                                                              |
| --------------------- | ---------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| id                    | String                                                     | Identificador exclusivo da relação. Somente leitura.                                                                                                                                                                        |
| weight                | Duplo                                                     | Valor que indica o quanto o documento está em tendência no momento. Quanto maior o número, mais o documento está na tendência ao redor do usuário (quanto mais relevante for). Os documentos retornados são organizados por esse valor. |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md) | Propriedades que você pode usar para visualizar o documento em sua experiência.                                                                                                                                                |
| resourceReference     | [resourceReference](insights-resourcereference.md)         | Fazer referência a propriedades do documento de tendência, como a URL e o tipo do documento.                                                                                                                                 |
| lastModifiedDateTime  | DateTimeOffset                                             |                                                                                                                                                                                                                          |

## <a name="relationships"></a>Relações

| Relação | Tipo   | Descrição                                   |
| ------------ | ------ | --------------------------------------------- |
| recurso     | entidade | Usado para navegar até o documento de tendência. |

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
