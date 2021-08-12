---
title: Tipo de recurso offerShiftRequest
description: Representa uma solicitação para oferecer uma mudança para outro usuário na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e3ef8c7dee695255c7802780f786d4555adc61dae78db191010e7e88d6e3190a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54138525"
---
# <a name="offershiftrequest-resource-type"></a>Tipo de recurso offerShiftRequest

Namespace: microsoft.graph

Representa uma solicitação para oferecer uma mudança para outro usuário na equipe.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/offershiftrequest-list.md) | Coleção [of offerShiftRequest](offershiftrequest.md) | Leia as propriedades e as relações de todos os **objetos offerShiftRequest** em uma equipe. |
| [Criar](../api/offershiftrequest-post.md) | [offerShiftRequest](offershiftrequest.md) | Crie uma instância de um **objeto offerShiftRequest.** |
| [Obter](../api/offershiftrequest-get.md) | [offerShiftRequest](offershiftrequest.md) | Leia as propriedades e as relações de um **objeto offerShiftRequest.** |
|[Aprovar](../api/offershiftrequest-approve.md)|None|Aprovar uma **ofertaShiftRequest**. |
|[Declínio](../api/offershiftrequest-decline.md)|None|Recusar uma **ofertaShiftRequest**. |

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

