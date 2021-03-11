---
title: Tipo de recurso offerShiftRequest
description: Representa o tipo de solicitação de turno para oferecer uma mudança para outro usuário na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0f80e8578422aa00d6af1d2df22a0dfb7472c8c8
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721478"
---
# <a name="offershiftrequest-resource-type"></a>Tipo de recurso offerShiftRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o tipo de solicitação de turno para oferecer uma mudança para outro usuário na equipe.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar](../api/offershiftrequest-post.md) | [offerShiftRequest](offershiftrequest.md) | Crie uma instância de um objeto offerShiftRequest. |
| [Get](../api/offershiftrequest-get.md) | [offerShiftRequest](offershiftrequest.md) | Ler propriedades e relações do objeto offerShiftRequest. |
| [List](../api/offershiftrequest-list.md) | Coleção [of offerShiftRequest](offershiftrequest.md) | Leia propriedades e relações de todos os objetos offerShiftRequest em uma equipe. |
|[Aprovar](../api/offershiftrequest-approve.md)|Nenhum(a)|Aprovar uma ofertaShiftRequest. |
|[Declínio](../api/offershiftrequest-decline.md)|Nenhum(a)|Recusar uma ofertaShiftRequest. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|recipientActionDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|recipientActionMessage|Cadeia de caracteres| Mensagem personalizada enviada pelo destinatário da solicitação de turno de oferta. |
|recipientUserId|Cadeia de caracteres| ID do usuário do destinatário da solicitação de turno de oferta.|
|senderShiftId|Cadeia de caracteres| ID do usuário do remetente da solicitação de turno de oferta.|

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


