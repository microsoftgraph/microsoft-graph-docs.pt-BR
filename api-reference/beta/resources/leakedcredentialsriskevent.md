---
title: tipo de recurso de leakedCredentialsRiskEvent
description: Um evento de risco detectado pelo Windows Azure Active Directory identidade proteção onde credenciais da conta foram detectadas à solta. Informações completas sobre eventos de risco podem ser encontradas na documentação de proteção de identidade do Windows Azure AD.
localization_priority: Normal
ms.openlocfilehash: 7a8f2a8cf72b713fab30887fcc4d81b8a88e71ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815978"
---
# <a name="leakedcredentialsriskevent-resource-type"></a>tipo de recurso de leakedCredentialsRiskEvent

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Um evento de risco detectado pelo [Proteção de identidade do Windows Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) onde credenciais da conta foram detectadas à solta. Informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Windows Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md) | [leakedCredentialsRiskEvent](leakedcredentialsriskevent.md) |Leia as propriedades e os relacionamentos do objeto leakedCredentialsRiskEvent.|

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
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
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
  "description": "leakedCredentialsRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
