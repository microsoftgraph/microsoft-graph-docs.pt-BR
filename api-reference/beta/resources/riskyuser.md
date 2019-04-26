---
title: tipo de recurso riskyUser
description: Representa usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 179a6cbddf3e4b27c47761bd81aad1052ae7f728
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343532"
---
# <a name="riskyuser-resource-type"></a>tipo de recurso riskyUser

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.

Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).

>**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.

## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Listar riskyUsers](../api/riskyusers-list.md) | coleção [riskyUser](riskyUser.md)|Listar usuários arriscados e suas propriedades.|
|[Obter riskyUser](../api/riskyusers-get.md) | [riskyUser](riskyUser.md)|Obtenha um usuário arriscado específico e suas propriedades.|
|[Confirmar riskyUsers comprometido](../api/riskyusers-confirmcompromised.md)|Nenhum |Confirmar um usuário arriscado como comprometido.|
|[Ignorar riskyUsers](../api/riskyusers-dismiss.md)|Nenhum | DesCartar o risco de um usuário arriscado.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|`id`|`string`|ID exclusiva do usuário em risco|
|`isDeleted`|`bool`|Indica se o usuário é excluído. Os valores possíveis são `true`:,`false`|
|`isGuest`|`bool`|Indica se o usuário é um usuário convidado. Os valores possíveis são: `true` e `false`. True se a identidade do usuário está fora do locatário em consideração. Este usuário pode ser um usuário B2B ou B2C com identidade no Azure AD, no MSA ou no provedor de identidade de terceiros. False se a identidade do usuário está dentro do locatário em consideração|
|`isProcessing`|`bool`|Indica wehther que o estado arriscado de um usuário está sendo processado pelo backend|
|`riskLastUpdatedDateTime`|`datetime`|A data e a hora em que o usuário arriscado foi atualizado pela última vez|
|`riskLevel`|`riskLevel`| Os valores possíveis são baixo, médio, alto, oculto, nenhum, unknownFutureValue.  |
|`riskState`|`riskState`| Os valores possíveis são None, confirmedSafe, remediated, atRisk, unknownFutureValue.  |
|`riskDetail`|`riskDetail`| Os valores possíveis são None, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, oculto, adminConfirmedUserCompromised, unknownFutureValue.  |
|`userDisplayName`|`string`|Nome de exibição do usuário arriscado|
|`userPrincipalName`|`string`|Nome UPN de usuário arriscado|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|histórico|coleção [riskyUserHistoryItem](riskyuserhistoryitem.md)| |

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
"isGuest": "boolean",
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
