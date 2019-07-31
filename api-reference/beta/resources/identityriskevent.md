---
title: tipo de recurso identityRiskEvent
description: 'Um evento de risco detectado pela proteção de identidade do Azure Active Directory. É o tipo base para cada tipo de evento de risco específico:'
author: cloudhandler
localization_priority: Normal
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 7ea0a11931021e828660cc7b03991b8ea96ef1f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005797"
---
# <a name="identityriskevent-resource-type"></a>tipo de recurso identityRiskEvent

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um evento de risco detectado pela [proteção de identidade do Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/). É o tipo base para cada tipo de evento de risco específico:

| Tipo de evento         | Descrição|
|:---------------|:-----------|
|[anonymousipRiskEvent](anonymousipriskevent.md) | Entradas de endereços IP anônimos. |
|[malwareRiskEvent](malwareriskevent.md) | Entradas de dispositivos infectados por malware. |
|[impossibleTravelRiskEvent](impossibletravelriskevent.md) | Impossível viajar para locais do atypical. |
|[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md) | Usuários com credenciais vazadas. |
|[suspiciousIpRiskEvent](suspiciousipriskevent.md) | Entradas de endereços IP suspeitos. |
|[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md) | Entradas de locais desconhecidos. |

As informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Azure ad](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter identityRiskEvent](../api/identityriskevent-get.md) | [identityRiskEvent](identityriskevent.md) |Leia as propriedades e os relacionamentos do objeto identityRiskEvent.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| A data e a hora em que o evento de risco foi fechado|
|createdDateTime|dateTimeOffset| A data e a hora em que o evento de risco foi criado. Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito. Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.|
|id|cadeia de caracteres| Somente leitura|
|riskEventDateTime|dateTimeOffset| A data e a hora em que o evento de risco ocorreu|
|riskEventStatus|string| Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskLevel|cadeia de caracteres| Os valores possíveis são: `low`, `medium`, `high`.|
|riskEventType|string| O tipo de risco|
|userDisplayName|string| O nome do usuário em risco|
|userId|string| A identificação do usuário em risco|
|userPrincipalName|string| O nome principal de usuário do usuário em risco|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|impactedUser|[Usuário](user.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso. 

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identityRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string",
  "riskEventType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
