---
title: Tipo de recurso timeOffRequest
description: Representa um tipo de solicitação de turno para fazer timeOff.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 90124b48f69dbaa053c6facd7a2bb84e5d427be0c20bdbc9017bfa8e3a800ebc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124014"
---
# <a name="timeoffrequest-resource-type"></a>Tipo de recurso timeOffRequest

Namespace: microsoft.graph

Representa um tipo de solicitação de turno para [fazer timeOff](../resources/timeoff.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Get](../api/timeoffrequest-get.md) | [timeOffRequest](timeoffrequest.md) | Leia as propriedades e as relações de um **objeto timeOffRequest.** |
| [List](../api/timeoffrequest-list.md) | [Coleção timeOffRequest](timeoffrequest.md) | Obter a lista de **objetos timeOffRequest** nesta agenda.|
| [Delete](../api/timeoffrequest-delete.md) | None | **Exclua um objeto timeOffRequest.** |
| [Aprovar](../api/timeoffrequest-approve.md)|None|Aprovar uma solicitação de tempo de folga.|
| [Declínio](../api/timeoffrequest-decline.md)|None|Recusar uma solicitação de tempo de folga.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|startDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|timeOffReasonId|Cadeia de caracteres|O motivo da folga.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeOffRequest"
}-->

```json
{
  "endDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "timeOffReasonId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeOffRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

