---
title: tipo de recurso locatedRiskEvent
description: 'Um evento de risco detectado pela Proteção de Identidade do Azure Active Directory que se baseia nos dados de localização. Os tipos de eventos de risco localizados incluem:'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: cloudhandler
ms.openlocfilehash: c53c503132a0b280c8b7fb02c99816d2ee7a5f03
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2021
ms.locfileid: "51490988"
---
# <a name="locatedriskevent-resource-type"></a>tipo de recurso locatedRiskEvent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um evento de risco detectado pela Proteção de Identidade [do Azure Active Directory](/azure/active-directory/identity-protection/overview-identity-protection) que se baseia nos dados de localização. Os tipos de eventos de risco localizados incluem:
* [entrar de endereços IP anônimos](anonymousipriskevent.md)
* [entrar de dispositivos infectados por malware](malwareriskevent.md)
* [viagem impossível para locais atípicos](impossibletravelriskevent.md)
* [entrar de endereços IP suspeitos](suspiciousipriskevent.md)
* [entrar de locais desconhecidos](unfamiliarlocationriskevent.md) Informações completas sobre eventos de risco podem ser encontradas na documentação da Proteção de Identidade do [Azure AD.](/azure/active-directory/identity-protection/overview-identity-protection)


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter locatedRiskEvent](../api/locatedriskevent-get.md) | [locatedRiskEvent](locatedriskevent.md) |Leia propriedades e relações do objeto locatedRiskEvent.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| A data e a hora em que o evento de risco foi fechado|
|createdDateTime|dateTimeOffset| A data e a hora em que o evento de risco foi criado. Isso é sempre maior ou igual ao tempo de data do evento de risco em si. Essa é a propriedade correta a ser usada como filtro ao consultar eventos de risco.|
|id|string| Somente leitura|
|ipAddress|string| O endereço IP da assinatura|
|location|cadeia de caracteres| O local anexado ao endereço IP da login|
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