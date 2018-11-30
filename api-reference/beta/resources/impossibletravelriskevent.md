---
title: tipo de recurso de impossibleTravelRiskEvent
description: Um evento de risco detectado pelo Windows Azure Active Directory identidade proteção onde duas entradas do conta ocorrem de locais atípicos para o usuário e seria impossível viajam entre os locais em que a duração entre as informações completas de sign-ins. sobre eventos de risco podem ser encontrados na documentação de proteção de identidade do Windows Azure AD.
ms.openlocfilehash: 38e61927121f520e79fd1fec8b8e6443fa8b76e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033449"
---
# <a name="impossibletravelriskevent-resource-type"></a>tipo de recurso de impossibleTravelRiskEvent

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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
|userAgent|string| Cadeia de caracteres de agente de usuário do navegador|
|userDisplayName|string| O nome do usuário em risco|
|userId|string| A identificação do usuário em risco|
|userPrincipalName|string| O nome de usuário principal do usuário em risco|

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
<!-- {
  "type": "#page.annotation",
  "description": "impossibleTravelRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->