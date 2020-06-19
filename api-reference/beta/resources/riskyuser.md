---
title: tipo de recurso riskyUser
description: Representa usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2390ff2f9aab1fe74aa6aebf0cfdbeeb6a2d5131
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793588"
---
# <a name="riskyuser-resource-type"></a>tipo de recurso riskyUser

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.

Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).

>**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.

## <a name="methods"></a>Methods

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Listar riskyUsers](../api/riskyusers-list.md) | coleção [riskyUser](riskyuser.md)|Listar usuários arriscados e suas propriedades.|
|[Obter riskyUser](../api/riskyusers-get.md) | [riskyUser](riskyuser.md)|Obtenha um usuário arriscado específico e suas propriedades.|
|[Histórico de lista](../api/riskyuser-list-history.md) | coleção [riskyUserHistoryItem](riskyuserhistoryitem.md)|Obter o histórico de riscos de um usuário do Azure AD.|
|[Confirmar riskyUsers comprometido](../api/riskyusers-confirmcompromised.md)|Nenhuma |Confirmar um usuário arriscado como comprometido.|
|[Ignorar riskyUsers](../api/riskyusers-dismiss.md)|Nenhuma | Descartar o risco de um usuário arriscado.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|`id`|`string`|ID exclusiva do usuário em risco|
|`isDeleted`|`bool`|Indica se o usuário é excluído. Os valores possíveis são: `true` ,`false`|
|`isProcessing`|`bool`|Indica wehther que o estado arriscado de um usuário está sendo processado pelo backend|
|`riskLastUpdatedDateTime`|`datetime`|A data e a hora em que o usuário arriscado foi atualizado pela última vez|
|`riskLevel`|`riskLevel`| Os valores possíveis são baixo, médio, alto, oculto, nenhum, unknownFutureValue.  |
|`riskState`|`riskState`| Os valores possíveis são None, confirmedSafe, remediated, atRisk, unknownFutureValue.  |
|`riskDetail`|`riskDetail`| Os valores possíveis são None, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, Hidden, adminConfirmedUserCompromised, unknownFutureValue.  |
|`userDisplayName`|`string`|Nome de exibição do usuário arriscado|
|`userPrincipalName`|`string`|Nome UPN de usuário arriscado|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUser"
}-->

```json
{
"id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isProcessing": "boolean",
"isDeleted": "boolean",
"riskDetail":  "string",
"riskLevel":  "string",
"riskState":  "string",
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
