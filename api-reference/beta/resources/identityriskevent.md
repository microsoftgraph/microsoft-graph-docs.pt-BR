---
title: Tipo de recurso identityRiskEvent
description: 'Um evento de risco detectado pela Proteção de Identidade do Azure Active Directory. É o tipo base para cada tipo de evento de risco específico:'
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: acb48ce5ef63abf5ec2a09d8a3365a744bb8a668
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440287"
---
# <a name="identityriskevent-resource-type-deprecated"></a>Tipo de recurso identityRiskEvent (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
>A **API identityRiskEvents** está preterida e interromperá o retorno de dados em 10 de janeiro de 2020. Para obter detalhes, [consulte Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).

Um evento de risco detectado pela Proteção de Identidade [do Azure Active Directory](/azure/active-directory/identity-protection/overview-identity-protection). É o tipo base para cada tipo de evento de risco específico:

| Tipo de evento         | Descrição|
|:---------------|:-----------|
|[anonymousipRiskEvent](anonymousipriskevent.md) | Entrar de endereços IP anônimos. |
|[malwareRiskEvent](malwareriskevent.md) | Entrar de dispositivos infectados por malware. |
|[impossibleTravelRiskEvent](impossibletravelriskevent.md) | Viagem impossível para locais atípicos. |
|[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md) | Usuários com credenciais vazadas. |
|[suspiciousIpRiskEvent](suspiciousipriskevent.md) | Entrar de endereços IP suspeitos. |
|[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md) | Entrar de locais desconhecidos. |

Informações completas sobre eventos de risco podem ser encontradas na documentação da Proteção de Identidade do [Azure AD.](/azure/active-directory/active-directory-reporting-risk-events)

## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter identityRiskEvent](../api/identityriskevent-get.md) | [identityRiskEvent](identityriskevent.md) |Leia propriedades e relações do objeto identityRiskEvent.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| A data e a hora em que o evento de risco foi fechado|
|createdDateTime|dateTimeOffset| A data e a hora em que o evento de risco foi criado. Isso é sempre maior ou igual ao tempo de data do evento de risco em si. Essa é a propriedade correta a ser usada como filtro ao consultar eventos de risco.|
|id|string| Somente leitura|
|riskEventDateTime|dateTimeOffset| A data e a hora em que o evento de risco ocorreu|
|riskEventStatus|string| Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskLevel|cadeia de caracteres| Os valores possíveis são: `low`, `medium`, `high`.|
|riskEventType|string| O tipo de risco|
|userDisplayName|string| O nome do usuário em risco|
|userId|cadeia de caracteres| A id do usuário em risco|
|userPrincipalName|string| O nome principal do usuário em risco|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|impactedUser|[user](user.md)| Somente leitura. Anulável.|

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
