---
title: tipo de recurso identityRiskEvent
description: 'Um evento de risco detectado pela proteção de identidade do Azure Active Directory. É o tipo base para cada tipo de evento de risco específico:'
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: b5c36ab898805c0638cc199ff8cfb893444f04ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506388"
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
|id|string| Somente leitura|
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
|impactedUser|[user](user.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso. 

<!-- {
  "blockType": "resource",
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
  "userPrincipalName": "string"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/identityriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
