---
title: Tipo de recurso reviewSet
description: Representa o conjunto estático de informações armazenadas eletronicamente coletadas para uso em uma solicitação de litígio, investigação ou regulamentação.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 25c33dd911d9c14d91131508fad37c1fea149b9a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445898"
---
# <a name="reviewset-resource-type"></a>Tipo de recurso reviewSet

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o conjunto estático de informações armazenadas eletronicamente coletadas para uso em uma solicitação de litígio, investigação ou regulamentação.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar reviewSets](../api/ediscovery-case-list-reviewsets.md) | [coleção microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) | Obter uma coleção de **objetos reviewset.** |
| [Criar reviewSet](../api/ediscovery-case-post-reviewsets.md) | [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) | Criar um novo **conjuntos de revisão**. |
| [Obter reviewSet](../api/ediscovery-reviewset-get.md) | [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) | Leia as propriedades e as relações de um **objeto reviewSet.** |
| [Listar consultas](../api/ediscovery-reviewsetquery-list.md)|[coleção microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md)|Obter uma lista de **recursos reviewSetQuery.**|
| [export](../api/ediscovery-reviewset-export.md) | Nenhum(a) | Inicie uma exportação de dados do **conjuntos de revisão.** |
| [addToReviewSet](../api/ediscovery-reviewset-addtoreviewset.md)|Nenhum(a)|Adicione dados de **uma sourceCollection** a um **conjuntos de revisão**.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|createdBy        | [identitySet](/graph/api/resources/identityset) | O usuário que criou o conjunto de revisão. Somente leitura. |
|createdDateTime  |DateTimeOffset| A data em que o conjunto de revisão foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura. |
|displayName      |String| O nome do conjunto de revisão. O nome é exclusivo com um limite máximo de 64 caracteres. |
|id               |String| O identificador exclusivo do conjunto de revisão. Somente leitura. |

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
| consultas |[coleção microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ediscovery.reviewSet",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.ediscovery.reviewSet",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reviewSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
