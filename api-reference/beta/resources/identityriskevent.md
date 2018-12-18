---
title: tipo de recurso de identityRiskEvent
description: 'Um evento de risco detectado pelo Windows Azure Active Directory proteção de identidade. É o tipo de base para cada tipo de evento de risco específico:'
author: cloudhandler
ms.openlocfilehash: 4abe473b47d3ce52fd5b75b6adfd08dbc4af54fc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351734"
---
# <a name="identityriskevent-resource-type"></a>tipo de recurso de identityRiskEvent

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Um evento de risco detectado pelo [Windows Azure Active Directory proteção de identidade](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/). É o tipo de base para cada tipo de evento de risco específico:

| Tipo de evento         | Descrição|
|:---------------|:-----------|
|[anonymousipRiskEvent](anonymousipriskevent.md) | Entradas de endereços IP anônimos. |
|[malwareRiskEvent](malwareriskevent.md) | Entradas de dispositivos infectados por malware. |
|[impossibleTravelRiskEvent](impossibletravelriskevent.md) | Impossível viagens para atípicos locais. |
|[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md) | Usuários com credenciais perdidas. |
|[suspiciousIpRiskEvent](suspiciousipriskevent.md) | Entradas de endereços IP suspeitos. |
|[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md) | Entradas de familiarizado locais. |

Informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Windows Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter identityRiskEvent](../api/identityriskevent-get.md) | [identityRiskEvent](identityriskevent.md) |Leia as propriedades e os relacionamentos do objeto identityRiskEvent.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| A data e hora em que o evento de risco foi fechado|
|createdDateTime|dateTimeOffset| A data e hora em que o evento de risco foi criado. Sempre é maior ou igual ao datetime do evento risco em si. Esta é a propriedade correta a ser usado como um filtro ao consultar eventos de risco.|
|id|string| Somente leitura|
|riskEventDateTime|dateTimeOffset| A data e hora quando o evento de risco ocorreu|
|riskEventStatus|string| Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskLevel|string| Os valores possíveis são: `low`, `medium`, `high`.|
|riskEventType|string| O tipo de risco|
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
<!-- {
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->