---
title: tipo de recurso sharedInsight
description: 'Uma percepção representando arquivos compartilhados com ou por um usuário específico. Há suporte para os seguintes arquivos compartilhados:'
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 47228e6597f24b9a6d662c7d87643322acaed40b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006231"
---
# <a name="sharedinsight-resource-type"></a>tipo de recurso sharedInsight

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma percepção representando arquivos compartilhados com ou por um usuário específico. Há suporte para os seguintes arquivos compartilhados:

- Arquivos anexados diretamente em um email ou convite de reunião.
- OneDrive for bussiness e anexos modernos do SharePoint-arquivos armazenados no OneDrive for Business e SharePoint que os usuários compartilham como links em um email.

**Observação**: no momento, estamos trabalhando para preencher os resultados da API compartilhada com dados. Pode haver alguns dados ausentes nas primeiras semanas após o lançamento.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar compartilhados](../api/insights-list-shared.md) |coleção [insights_shared](insights-shared.md)| Obter uma lista de arquivos compartilhados.|

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                      | Descrição  |
| -------------         |---------------            | -------------|
| id                    | String                    | Identificador exclusivo da relação. Somente leitura.        |
| lastShared            | [sharingDetail](insights-sharingdetail.md)                | Detalhes sobre o item compartilhado. Somente leitura.        |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | Propriedades que você pode usar para visualizar o documento em sua experiência. Somente leitura      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | Propriedades de referência do documento compartilhado, como a URL e o tipo do documento. Somente leitura       |

## <a name="relationships"></a>Relações

| Propriedade      | Tipo          | Descrição  |
| ------------- |---------------| -------------|
| recurso      | coleção Entity | Usado para navegar até o item compartilhado. Para anexos de arquivo, o tipo ** é fileattachment. Para anexos vinculados, o tipo é *driveItem*. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso
<!--{
  "blockType":"resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedInsight"
}-->
```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
