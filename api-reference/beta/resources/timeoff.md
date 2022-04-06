---
title: Tipo de recurso timeOff
description: Uma unidade que não funciona na agenda.
author: aaku
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5e237d23c82e46602087cfbab009c3ac9d7af16e
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723456"
---
# <a name="timeoff-resource-type"></a>Tipo de recurso timeOff

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma unidade que não funciona em um cronograma.

## <a name="methods"></a>Methods

| Método                                     | Tipo de retorno                      | Descrição                                           |
| :----------------------------------------- | :------------------------------- | :---------------------------------------------------- |
| [Criar](../api/schedule-post-timesoff.md) | [timeOff](timeoff.md)            | Crie um novo **objeto timeOff** .                      |
| [Lista](../api/schedule-list-timesoff.md)   | [Coleção timeOff](timeoff.md) | Obter a lista de **objetos timeOff** nesta agenda. |
| [Get](../api/timeoff-get.md)               | [timeOff](timeoff.md)            | Obter um **objeto timeOff** por ID.                       |
| [Replace](../api/timeoff-put.md)           | [timeOff](timeoff.md)            | Substitua um **objeto timeOff** .                         |
| [Delete](../api/timeoff-delete.md)         | Nenhum                             | **Exclua um objeto timeOff** da agenda.        |

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                          | Descrição                                                                                                                                                                                                                              |
| -------------------- | ----------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                   | `string`                      | ID do **timeOff**.                                                                                                                                                                                                                   |
| userId               | `string`                      | ID do usuário atribuído ao **timeOff**. Obrigatório.                                                                                                                                                                                    |
| sharedTimeOff        | [timeOffItem](timeoffitem.md) | A versão compartilhada deste **timeOff** que pode ser visualizada por funcionários e gerentes. Obrigatório.                                                                                                                                        |
| draftTimeOff         | [timeOffItem](timeoffitem.md) | A versão de rascunho deste **timeOff** que pode ser visualizada pelos gerentes. Obrigatório.                                                                                                                                                            |
| createdDateTime      | `DateTimeOffset`              | O carimbo de data/hora no **qual este timeOff** foi criado pela primeira vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
| lastModifiedDateTime | `DateTimeOffset`              | O carimbo de data/hora no **qual o timeOff** foi atualizado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.  |
| lastModifiedBy       | [identitySet](identityset.md) | A identidade que foi atualizada pela última **vez neste timeOff**.                                                                                                                                                                                         |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOff",
   "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "userId": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "sharedTimeOff": {"@odata.type":"microsoft.graph.timeOffItem"},
  "draftTimeOff": {"@odata.type":"microsoft.graph.timeOffItem"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "timeOff resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
