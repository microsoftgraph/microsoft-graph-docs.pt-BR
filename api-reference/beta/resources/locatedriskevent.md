---
title: tipo de recurso locatedRiskEvent
description: 'Um evento de risco detectado pela proteção de identidade do Azure Active Directory com base nos dados do local. Os tipos de eventos de risco localizados incluem:'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: 461f20233e92edca48b9dd51fa417b33ab9f386c
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404669"
---
# <a name="locatedriskevent-resource-type"></a>tipo de recurso locatedRiskEvent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um evento de risco detectado pela [proteção de identidade do Azure Active Directory](/azure/active-directory/identity-protection/overview-identity-protection) com base nos dados do local. Os tipos de eventos de risco localizados incluem:
* [entradas de endereços IP anônimos](anonymousipriskevent.md)
* [entradas de dispositivos infectados por malware](malwareriskevent.md)
* [impossível viajar para locais atypical](impossibletravelriskevent.md)
* [entradas de endereços IP suspeitos](suspiciousipriskevent.md)
* [entradas de locais desconhecidos](unfamiliarlocationriskevent.md) As informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Azure ad](/azure/active-directory/identity-protection/overview-identity-protection).


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter locatedRiskEvent](../api/locatedriskevent-get.md) | [locatedRiskEvent](locatedriskevent.md) |Leia as propriedades e os relacionamentos do objeto locatedRiskEvent.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| A data e a hora em que o evento de risco foi fechado|
|createdDateTime|dateTimeOffset| A data e a hora em que o evento de risco foi criado. Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito. Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.|
|id|string| Somente leitura|
|ipAddress|string| O endereço IP do logon|
|location|cadeia de caracteres| O local anexado ao endereço IP do logon|
|riskEventDateTime|dateTimeOffset| A data e a hora em que o evento de risco ocorreu|
|riskEventStatus|string| Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskLevel|cadeia de caracteres| Os valores possíveis são: `low`, `medium`, `high`.|
|riskEventType|string| O tipo de risco|
|userDisplayName|string| O nome do usuário em risco|
|userId|cadeia de caracteres| A identificação do usuário em risco|
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
   "abstract": true,
   "keyProperty": "id",
   "baseType":"microsoft.graph.identityRiskEvent",
  "@odata.type": "microsoft.graph.locatedRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "ipAddress": "string",
  "location": "string",
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
  "description": "locatedRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->