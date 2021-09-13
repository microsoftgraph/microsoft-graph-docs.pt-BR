---
title: tipo de recurso de tendência
description: Rico relacionamento conectando um usuário a documentos que têm tendências em torno do usuário (são relevantes para o usuário). Os arquivos do OneDrive e os arquivos armazenados em sites de equipe do Microsoft Office SharePoint Online podem ser uma tendência em torno do usuário.
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5cf846ca79088e250b4e37fa97495896fd88fe44
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109133"
---
# <a name="trending-resource-type"></a>tipo de recurso de tendência

Namespace: microsoft.graph

Rico relacionamento conectando um usuário a documentos que têm tendências em torno do usuário (são relevantes para o usuário). Os arquivos do OneDrive e os arquivos armazenados em sites de equipe do Microsoft Office SharePoint Online podem ser uma tendência em torno do usuário.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar tendências](../api/insights-list-trending.md) |coleção [tendências](insights-trending.md) | Obter uma lista de arquivos de tendência.|

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                              | Descrição  |
| ------------- |---------------                    | -------------|
| id                    | Cadeia de caracteres                    | Identificador exclusivo da relação. Somente leitura.        |
| weight                | Duplo                    | Valor que indica o quanto o documento está em tendência no momento. Quanto maior o número, mais o documento está na tendência ao redor do usuário (quanto mais relevante for). Os documentos retornados são organizados por esse valor.  |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)    | Propriedades que você pode usar para visualizar o documento em sua experiência. |
| resourceReference     | [resourceReference](insights-resourcereference.md)        | Fazer referência a propriedades do documento de tendência, como a URL e o tipo do documento. |
| lastModifiedDateTime  | DateTimeOffset            | |
## <a name="relationships"></a>Relações

| Propriedade      | Tipo          | Descrição  |
| ------------- |---------------| -------------|
| recurso      | entidade        | Usado para navegar até o documento de tendência. |

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

