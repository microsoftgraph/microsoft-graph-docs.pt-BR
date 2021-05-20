---
title: Tipo de recurso leakedCredentialsRiskEvent
description: Um evento de risco detectado pela Azure Active Directory Identity Protection em que as credenciais de uma conta foram detectadas na natureza. Informações completas sobre eventos de risco podem ser encontradas na documentação da Proteção de Identidade do Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: cloudhandler
ms.openlocfilehash: 7d5cd0ab0c6869a5be04d1c227517c848540b480
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547082"
---
# <a name="leakedcredentialsriskevent-resource-type-deprecated"></a>Tipo de recurso leakedCredentialsRiskEvent (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
>A **API identityRiskEvents** está preterida e interromperá o retorno de dados em 10 de janeiro de 2020. Para obter detalhes, [consulte Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).

Um evento de risco detectado pelo [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) em que as credenciais de uma conta foram detectadas na natureza. Informações completas sobre eventos de risco podem ser encontradas na documentação da Proteção de Identidade do [Azure AD.](/azure/active-directory/identity-protection/overview-identity-protection)


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md) | [leakedCredentialsRiskEvent](leakedcredentialsriskevent.md) |Leia propriedades e relações do objeto leakedCredentialsRiskEvent.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| A data e a hora em que o evento de risco foi fechado|
|createdDateTime|dateTimeOffset| A data e a hora em que o evento de risco foi criado. Isso é sempre maior ou igual ao tempo de data do evento de risco em si. Essa é a propriedade correta a ser usada como filtro ao consultar eventos de risco.|
|id|cadeia de caracteres| Somente leitura|
|riskEventDateTime|dateTimeOffset| A data e a hora em que o evento de risco ocorreu|
|riskEventStatus|cadeia de caracteres| Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskLevel|cadeia de caracteres| Os valores possíveis são: `low`, `medium`, `high`.|
|riskEventType|cadeia de caracteres| O tipo de risco|
|userDisplayName|cadeia de caracteres| O nome do usuário em risco|
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
  "userPrincipalName": "string",
  "riskEventType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "leakedCredentialsRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
