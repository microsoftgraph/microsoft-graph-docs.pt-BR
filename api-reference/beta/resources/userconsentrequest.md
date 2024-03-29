---
title: Tipo de recurso userConsentRequest
description: Uma solicitação criada por um usuário para usar um aplicativo que exige acesso a dados organizacionais que o usuário não tem autorização para conceder consentimento a si mesmo.
author: psignoret
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ba332a2ebdfa8735bd1e4cf750479aae203277f2
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61649760"
---
# <a name="userconsentrequest-resource-type"></a>Tipo de recurso userConsentRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um [userConsentRequest](../resources/userconsentrequest.md) é criado por um usuário quando ele está solicitando acesso a um aplicativo que exige uma autorização de administrador para acessar. 

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userConsentRequests](../api/appconsentrequest-list-userconsentrequests.md)|[Coleção userConsentRequest](../resources/userconsentrequest.md)|Recupere uma coleção de [objetos userConsentRequest](userconsentrequest.md) para [um appConsentRequest](appconsentrequest.md).|
|[Obter userConsentRequest](../api/userconsentrequest-get.md)|[userConsentRequest](../resources/userconsentrequest.md)|Leia as propriedades e as relações de um [objeto userConsentRequest.](../resources/userconsentrequest.md)|
|[filterByCurrentUser](../api/userconsentrequest-filterByCurrentUser.md)|[Coleção userConsentRequest](../resources/userconsentrequest.md)|Leia as propriedades dos [objetos userConsentRequest](../resources/userconsentrequest.md) para [um appConsentRequest](appconsentrequest.md) para o qual o usuário atual é o revistor.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|approvalId|String|A id da aprovação. Esse valor é igual ao valor do `id` .|
|completedDateTime|DateTimeOffset|A data e a hora em **que o status** da solicitação foi marcado como `Completed` . As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou a solicitação.|
|createdDateTime|DateTimeOffset|A data e a hora em que a solicitação foi criada. As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Suporta `$filter` ( `eq` somente) e `$orderby` .|
|customData|String|Campo de texto livre para definir quaisquer dados personalizados para a solicitação de consentimento do usuário. Não usado.|
|id|String|Identificador da solicitação. |
|motivo|String|A justificativa do usuário para exigir acesso ao aplicativo. Suporta `$filter` ( `eq` somente) e `$orderby` .  |
|status|String|O status da solicitação de consentimento do aplicativo do usuário. Os valores possíveis são: `Initializing` `InProgress` , e `Completed` . Suporta `$filter` ( `eq` somente) e `$orderby` . |

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

