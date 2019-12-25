---
title: tipo de recurso impossibleTravelRiskEvent
description: Um evento de risco detectado pela proteção de identidade do Azure Active Directory onde dois logons de conta ocorrem de locais atypical para o usuário e não seria possível viajar entre os locais na duração entre os logons. complete information about eventos de risco podem ser encontrados na documentação de proteção de identidade do Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: be2b5db09a20264525e783e05771f6d1da2783e2
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866781"
---
# <a name="impossibletravelriskevent-resource-type"></a>tipo de recurso impossibleTravelRiskEvent

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
>A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020. Para obter detalhes, consulte [Preterition of the IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).

Um evento de risco detectado pela [proteção de identidade do Active Directory do Azure](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) onde dois logons de conta ocorrem a partir de locais atypical para o usuário e seria impossível viajar entre os locais na duração entre as entradas. Complete as informações sobre os eventos de risco podem ser encontradas na [documentação do Azure ad Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) | [impossibleTravelRiskEvent](impossibletravelriskevent.md) |Leia as propriedades e os relacionamentos do objeto impossibleTravelRiskEvent.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| A data e a hora em que o evento de risco foi fechado|
|createdDateTime|dateTimeOffset| A data e a hora em que o evento de risco foi criado. Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito. Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.|
|deviceInformation|string| Informações sobre o dispositivo|
|id|string| Somente leitura|
|ipAddress|string| O endereço IP da segunda entrada|
|isAtypicalLocation|booliano| Se um dos locais for atypical para o usuário|
|location|cadeia de caracteres| O local anexado ao endereço IP da segunda entrada|
|previousIPAddress|string| O endereço IP do primeiro logon|
|previousLocation|string| O local anexado ao endereço IP do primeiro logon|
|previousSigninDateTime|dateTimeOffset| A data e a hora da primeira entrada|
|riskEventDateTime|dateTimeOffset| A data e a hora da segunda entrada|
|riskEventStatus|string| Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskLevel|cadeia de caracteres| Os valores possíveis são: `low`, `medium`, `high`.|
|riskEventType|string| O tipo de risco|
|userAgent|string| A cadeia de caracteres do agente do usuário do navegador|
|userDisplayName|string| O nome do usuário em risco|
|userId|cadeia de caracteres| A identificação do usuário em risco|
|userPrincipalName|string| O nome principal de usuário do usuário em risco|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|impactedUser|[Usuário](user.md)| Somente leitura. Anulável.|

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
