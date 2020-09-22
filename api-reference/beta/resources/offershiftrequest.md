---
title: tipo de recurso offerShiftRequest
description: Representa o tipo de solicitação de mudança para oferecer uma mudança para outro usuário na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e7c41461848fab45f3d291b175e6c584f98326fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021270"
---
# <a name="offershiftrequest-resource-type"></a>tipo de recurso offerShiftRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o tipo de solicitação de mudança para oferecer uma mudança para outro usuário na equipe.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar](../api/offershiftrequest-post.md) | [offerShiftRequest](offershiftrequest.md) | Criar uma instância de um objeto offerShiftRequest. |
| [Get](../api/offershiftrequest-get.md) | [offerShiftRequest](offershiftrequest.md) | Leia as propriedades e os relacionamentos do objeto offerShiftRequest. |
| [Lista](../api/offershiftrequest-list.md) | Coleção de [offerShiftRequest](offershiftrequest.md) | Leia as propriedades e as relações de todos os objetos offerShiftRequest de uma equipe. |
|[Aprovar](../api/offershiftrequest-approve.md)|Nenhum|Aprovar um offerShiftRequest. |
|[Aceito](../api/offershiftrequest-decline.md)|Nenhum|Recusar um offerShiftRequest. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|recipientActionDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|recipientActionMessage|String| Mensagem personalizada enviada pelo destinatário da solicitação de mudança de oferta. |
|recipientUserId|String| ID de usuário do destinatário da solicitação de mudança de oferta.|
|senderShiftId|String| ID de usuário do remetente da solicitação de mudança de oferta.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.offerShiftRequest",
  "baseType": ""
}-->

```json
{
  "recipientActionDateTime": "String (timestamp)",
  "recipientActionMessage": "String",
  "recipientUserId": "String",
  "senderShiftId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "offerShiftRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


