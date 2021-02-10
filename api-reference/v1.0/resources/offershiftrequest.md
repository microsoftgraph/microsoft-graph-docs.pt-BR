---
title: Tipo de recurso offerShiftRequest
description: Representa uma solicitação para oferecer uma mudança para outro usuário na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d17ca029d29b2b8f27a923adf4ef019ac002f404
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158720"
---
# <a name="offershiftrequest-resource-type"></a>Tipo de recurso offerShiftRequest

Namespace: microsoft.graph

Representa uma solicitação para oferecer uma mudança para outro usuário na equipe.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/offershiftrequest-list.md) | Coleção de [offerShiftRequest](offershiftrequest.md) | Leia as propriedades e os relacionamentos de todos os **objetos offerShiftRequest** em uma equipe. |
| [Criar](../api/offershiftrequest-post.md) | [offerShiftRequest](offershiftrequest.md) | Crie uma instância de um **objeto offerShiftRequest.** |
| [Get](../api/offershiftrequest-get.md) | [offerShiftRequest](offershiftrequest.md) | Leia as propriedades e os relacionamentos de um **objeto offerShiftRequest.** |
|[Aprovar](../api/offershiftrequest-approve.md)|Nenhum|Aprovar uma **ofertaShiftRequest**. |
|[Recusar](../api/offershiftrequest-decline.md)|Nenhum|Recusar uma **ofertaShiftRequest**. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|recipientActionDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|recipientActionMessage|Cadeia de caracteres| Mensagem personalizada enviada pelo destinatário da solicitação de turno de oferta. |
|recipientUserId|Cadeia de caracteres| ID de usuário do destinatário da solicitação de mudança de oferta.|
|senderShiftId|Cadeia de caracteres| ID de usuário do remetente da solicitação de mudança de oferta.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.offerShiftRequest"
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

