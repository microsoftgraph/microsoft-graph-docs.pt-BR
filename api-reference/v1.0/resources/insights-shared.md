---
title: Tipo de recurso sharedInsight
description: 'Uma visão que representa arquivos compartilhados com ou por um usuário específico. Os seguintes arquivos compartilhados são suportados:'
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 73d02b3fa6ae6a9938b6c7174bbf942dcb6ed85ef2baa48ebc9f061908a9f369
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54184820"
---
# <a name="sharedinsight-resource-type"></a>Tipo de recurso sharedInsight

Namespace: microsoft.graph

Uma visão que representa arquivos compartilhados com ou por um usuário específico. Os seguintes arquivos compartilhados são suportados:

- Arquivos anexados diretamente em um email ou em um convite de reunião.
- OneDrive for Business e SharePoint modernos - arquivos armazenados em OneDrive for Business e SharePoint que os usuários compartilham como links em um email.

**Observação**: estamos trabalhando no momento para preencher os resultados da API Compartilhada com dados. Pode haver alguns dados ausentes nas primeiras semanas após o lançamento.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar compartilhado](../api/insights-list-shared.md) |coleção [sharedInsight](insights-shared.md)| Obter uma lista de arquivos compartilhados.|

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                      | Descrição  |
| -------------         |---------------            | -------------|
| id                    | Cadeia de caracteres                    | Identificador exclusivo da relação. Somente leitura.        |
| lastShared            | [sharingDetail](insights-sharingdetail.md)                | Detalhes sobre o item compartilhado. Somente leitura.        |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | Propriedades que você pode usar para visualizar o documento em sua experiência. Somente leitura      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | Fazer referência a propriedades do documento compartilhado, como a URL e o tipo do documento. Somente leitura       |

## <a name="relationships"></a>Relações

| Propriedade      | Tipo          | Descrição  |
| ------------- |---------------| -------------|
| recurso      | coleção entity | Usado para navegar até o item que foi compartilhado. Para anexos de arquivo, o tipo *é fileAttachment*. Para anexos vinculados, o tipo é *driveItem*. |

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

