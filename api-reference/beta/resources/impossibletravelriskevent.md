---
title: tipo de recurso de impossibleTravelRiskEvent
description: Um evento de risco detectado pelo Windows Azure Active Directory identidade proteção onde duas entradas do conta ocorrem de locais atípicos para o usuário e seria impossível viajam entre os locais em que a duração entre as informações completas de sign-ins. sobre eventos de risco podem ser encontrados na documentação de proteção de identidade do Windows Azure AD.
localization_priority: Normal
ms.openlocfilehash: 517a09963570ce2c4a9e58edf7b73babaaff0426
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529380"
---
# <a name="impossibletravelriskevent-resource-type"></a>tipo de recurso de impossibleTravelRiskEvent

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um evento de risco detectado pelo [Proteção de identidade do Windows Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) na qual duas entradas do conta ocorrem de locais atípicos para o usuário e seria impossível viajam entre os locais na duração entre concluir sign-ins. informações sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Windows Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) | [impossibleTravelRiskEvent](impossibletravelriskevent.md) |Leia as propriedades e os relacionamentos do objeto impossibleTravelRiskEvent.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| A data e hora em que o evento de risco foi fechado|
|createdDateTime|dateTimeOffset| A data e hora em que o evento de risco foi criado. Sempre é maior ou igual ao datetime do evento risco em si. Esta é a propriedade correta a ser usado como um filtro ao consultar eventos de risco.|
|deviceInformation|string| Informações sobre o dispositivo|
|id|string| Somente leitura|
|ipAddress|string| O endereço IP do segundo sign-in|
|isAtypicalLocation|booliano| Se um dos locais for atípico para o usuário|
|location|string| O local anexado ao endereço IP do segundo sign-in|
|previousIPAddress|string| O endereço IP do primeiro sign-in|
|previousLocation|string| O local anexado ao endereço IP do primeiro sign-in|
|previousSigninDateTime|dateTimeOffset| A data e hora do primeiro sign-in|
|riskEventDateTime|dateTimeOffset| A data e hora do segundo sign-in|
|riskEventStatus|string| Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskLevel|string| Os valores possíveis são: `low`, `medium`, `high`.|
|riskEventType|string| O tipo de risco|
|UserAgent|string| Cadeia de caracteres de agente de usuário do navegador|
|userDisplayName|string| O nome do usuário em risco|
|userId|string| A identificação do usuário em risco|
|userPrincipalName|string| O nome de usuário principal do usuário em risco|

## <a name="relationships"></a>Relacionamento
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|impactedUser|[user](user.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
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
  "userPrincipalName": "string"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/impossibletravelriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
