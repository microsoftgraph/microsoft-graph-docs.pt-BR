---
title: Tipo de recurso offerShiftRequest
description: Representa uma solicitação para oferecer uma mudança para outro usuário na equipe.
ms.localizationpriority: medium
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 10e96e9260f1027db87884bc8b01582fb7743a75
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094223"
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
|[Aprovar](../api/offershiftrequest-approve.md)|Nenhum(a)|Aprovar uma **ofertaShiftRequest**. |
|[Declínio](../api/offershiftrequest-decline.md)|Nenhum(a)|Recusar uma **ofertaShiftRequest**. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|recipientActionDateTime|DateTimeOffset|O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|recipientActionMessage|Cadeia de caracteres| Mensagem personalizada enviada pelo destinatário da solicitação de turno de oferta. |
|recipientUserId|Cadeia de caracteres| ID do usuário do destinatário da solicitação de turno de oferta.|
|senderShiftId|String| ID do usuário do remetente da solicitação de turno de oferta.|

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

