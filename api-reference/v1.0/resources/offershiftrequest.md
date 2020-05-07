---
title: tipo de recurso offerShiftRequest
description: Representa uma solicitação para oferecer uma mudança para outro usuário na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c507b8043c377dca0e13e079ff37e9499c00fbe1
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155114"
---
# <a name="offershiftrequest-resource-type"></a>tipo de recurso offerShiftRequest

Namespace: microsoft.graph

Representa uma solicitação para oferecer uma mudança para outro usuário na equipe.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/offershiftrequest-list.md) | Coleção de [offerShiftRequest](offershiftrequest.md) | Leia as propriedades e os relacionamentos de todos os objetos **offerShiftRequest** de uma equipe. |
| [Create](../api/offershiftrequest-post.md) | [offerShiftRequest](offershiftrequest.md) | Criar uma instância de um objeto **offerShiftRequest** . |
| [Get](../api/offershiftrequest-get.md) | [offerShiftRequest](offershiftrequest.md) | Leia as propriedades e os relacionamentos de um objeto **offerShiftRequest** . |
|[Aprovar](../api/offershiftrequest-approve.md)|Nenhum|Aprovar um **offerShiftRequest**. |
|[Aceito](../api/offershiftrequest-decline.md)|Nenhum|Recusar um **offerShiftRequest**. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|recipientActionDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|recipientActionMessage|Cadeia de caracteres| Mensagem personalizada enviada pelo destinatário da solicitação de mudança de oferta. |
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
