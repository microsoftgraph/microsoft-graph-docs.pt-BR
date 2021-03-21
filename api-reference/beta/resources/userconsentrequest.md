---
title: Tipo de recurso userConsentRequest
description: Uma solicitação criada por um usuário para usar um aplicativo que exige acesso a dados organizacionais que o usuário não tem autorização para conceder consentimento a si mesmo.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d3d91688a0a385ea319dee6df90b45c52bd4ec89
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965023"
---
# <a name="userconsentrequest-resource-type"></a>Tipo de recurso userConsentRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um [userConsentRequest](../resources/userconsentrequest.md) é criado por um usuário quando ele está solicitando acesso a um aplicativo que exige uma autorização de administrador para acessar. 

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userConsentRequests](../api/userconsentrequest-list.md)|[Coleção userConsentRequest](../resources/userconsentrequest.md)|Obter uma lista dos [objetos userConsentRequest](../resources/userconsentrequest.md) e suas propriedades.|
|[Obter userConsentRequest](../api/userconsentrequest-get.md)|[userConsentRequest](../resources/userconsentrequest.md)|Leia as propriedades e as relações de um [objeto userConsentRequest.](../resources/userconsentrequest.md)|
|[Listar userConsentRequests: filterByCurrentUser](../api/userconsentrequest-filterByCurrentUser.md)|[Coleção userConsentRequest](../resources/userconsentrequest.md)|Obter uma lista dos [objetos userConsentRequest](../resources/userconsentrequest.md) e suas propriedades.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|approvalId|Cadeia de caracteres|A id da aprovação. Esse valor é igual ao valor do `id` .|
|completedDateTime|DateTimeOffset|A data e a hora em **que o status** da solicitação foi marcado como `Completed` . As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou a solicitação.|
|createdDateTime|DateTimeOffset|A data e a hora em que a solicitação foi criada. As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Suporta `$filter` ( `eq` somente) e `$orderby` .|
|customData|Cadeia de caracteres|Campo de texto livre para definir quaisquer dados personalizados para a solicitação de consentimento do usuário. Não usado.|
|id|Cadeia de caracteres|Identificador da solicitação. |
|motivo|Cadeia de caracteres|A justificativa do usuário para exigir acesso ao aplicativo. Suporta `$filter` ( `eq` somente) e `$orderby` .  |
|status|Cadeia de caracteres|O status da solicitação de consentimento do aplicativo do usuário. Os valores possíveis são: `Initializing` `InProgress` , e `Completed` . Suporta `$filter` ( `eq` somente) e `$orderby` . |

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|aprovação|[aprovação](../resources/approval.md)|Decisões de aprovação associadas a uma solicitação.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userConsentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userConsentRequest",
  "id": "String (identifier)",
  "status": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "approvalId": "String",
  "customData": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "reason": "String"
}
```

