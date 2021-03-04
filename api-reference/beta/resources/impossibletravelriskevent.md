---
title: Tipo de recurso impossibleTravelRiskEvent
description: Um evento de risco detectado pela Proteção de Identidade do Azure Active Directory em que duas insinuidades de conta ocorrem de locais atípicos para o usuário e seria impossível viajar entre os locais durante a duração entre as insíções. Informações completas sobre eventos de risco podem ser encontradas na documentação da Proteção de Identidade do Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: c62dfda856bf2761290fff93b505669348eded0e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440231"
---
# <a name="impossibletravelriskevent-resource-type-deprecated"></a>tipo de recurso impossibleTravelRiskEvent (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
>A **API identityRiskEvents** está preterida e interromperá o retorno de dados em 10 de janeiro de 2020. Para obter detalhes, [consulte Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).

Um evento de risco detectado pela Proteção de Identidade do [Azure Active Directory](/azure/active-directory/identity-protection/overview-identity-protection) em que duas insinuidades de conta ocorrem de locais atípicos para o usuário e seria impossível viajar entre os locais durante a duração entre as insíções. Informações completas sobre eventos de risco podem ser encontradas na documentação da Proteção de Identidade do [Azure AD.](/azure/active-directory/identity-protection/overview-identity-protection)


## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) | [impossibleTravelRiskEvent](impossibletravelriskevent.md) |Ler propriedades e relações do objeto impossibleTravelRiskEvent.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| A data e a hora em que o evento de risco foi fechado|
|createdDateTime|dateTimeOffset| A data e a hora em que o evento de risco foi criado. Isso é sempre maior ou igual ao tempo de data do evento de risco em si. Essa é a propriedade correta a ser usada como filtro ao consultar eventos de risco.|
|deviceInformation|string| Informações sobre o dispositivo|
|id|string| Somente leitura|
|ipAddress|string| O endereço IP do segundo login|
|isAtypicalLocation|booliano| Se um dos locais for atípico para o usuário|
|location|cadeia de caracteres| O local anexado ao endereço IP do segundo login|
|previousIPAddress|string| O endereço IP do primeiro login|
|previousLocation|string| O local anexado ao endereço IP do primeiro login|
|previousSigninDateTime|dateTimeOffset| A data e a hora do primeiro login|
|riskEventDateTime|dateTimeOffset| A data e a hora do segundo login|
|riskEventStatus|string| Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskLevel|cadeia de caracteres| Os valores possíveis são: `low`, `medium`, `high`.|
|riskEventType|string| O tipo de risco|
|userAgent|string| Cadeia de caracteres de agente de usuário do navegador|
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
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.impossibleTravelRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "deviceInformation": "string",
  "id": "string (identifier)",
  "ipAddress": "string",
  "isAtypicalLocation": true,
  "location": "string",
  "previousIPAddress": "string",
  "previousLocation": "string",
  "previousSigninDateTime": "String (timestamp)",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userAgent": "string",
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
  "description": "impossibleTravelRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
