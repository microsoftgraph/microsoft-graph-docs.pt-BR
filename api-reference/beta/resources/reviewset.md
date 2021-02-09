---
title: Tipo de recurso reviewSet
description: Representa um conjunto estático de informações armazenadas eletronicamente coletadas para uso em uma solicitação regulamentar, investigação ou litígio.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: b6234fafbf0d6e36d5dcbb4143956447e26d3a0f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153491"
---
# <a name="reviewset-resource-type"></a>Tipo de recurso reviewSet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um conjunto estático de informações armazenadas eletronicamente coletadas para uso em uma solicitação regulamentar, investigação ou litígio.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar reviewSet](../api/reviewset-list.md) | [coleção reviewSet](reviewset.md) | Obter uma coleção de conjuntos de revisão. |
| [Obter reviewSet](../api/reviewset-get.md) | [reviewSet](reviewset.md) | Leia as propriedades e os relacionamentos de um **objeto reviewSet.** |
| [Criar reviewSet](../api/reviewset-post.md) | [reviewSet](reviewset.md) | Criar um novo conjunto de revisão. |
| [Listar consultas](../api/reviewsetquery-list.md)|[Coleção reviewSetQuery](../resources/reviewsetquery.md)|Obter os recursos reviewSetQuery da propriedade de navegação de consultas.|
| [Criar consultas](../api/reviewsetquery-post.md)|[reviewSetQuery](../resources/reviewsetquery.md)|Crie um novo objeto reviewSetQuery.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|createdBy        | [identitySet](/graph/api/resources/identityset) | O usuário que criou o conjunto de revisão. Somente leitura. |
|createdDateTime  |DateTimeOffset| A data e a hora em que o conjunto de revisão foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura. |
|displayName      |String| O nome do conjunto de revisão. O nome é exclusivo com um limite máximo de 64 caracteres. |
|id               |String| O identificador exclusivo do conjunto de revisão. Somente leitura. |

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Revisar a consulta do conjunto |[Coleção reviewSetQuery](reviewsetquery.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSet",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.reviewSet",
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
