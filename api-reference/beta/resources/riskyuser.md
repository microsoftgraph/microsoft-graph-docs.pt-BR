---
title: tipo de recurso riskyUser
description: Representa os usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários em risco no Azure AD.
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
ms.openlocfilehash: d2e0942e92b1dcd648812503a923dac51a640be1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960317"
---
# <a name="riskyuser-resource-type"></a>tipo de recurso riskyUser

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários em risco no Azure AD.

Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).

>**Observação:** Usar a API riskyUsers requer uma licença do Azure AD Premium P2.

## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Listar riskyUsers](../api/riskyusers-list.md) | [Coleção riskyUser](riskyuser.md)|Listar usuários arriscados e suas propriedades.|
|[Obter riskyUser](../api/riskyusers-get.md) | [riskyUser](riskyuser.md)|Obter um usuário de risco específico e suas propriedades.|
|[Histórico de listas](../api/riskyuser-list-history.md) | [coleção riskyUserHistoryItem](riskyuserhistoryitem.md)|Obter o histórico de risco de um usuário do Azure AD.|
|[Confirmar riskyUsers comprometidos](../api/riskyusers-confirmcompromised.md)|Nenhum |Confirme um usuário arriscado como comprometido.|
|[Descartar riskyUsers](../api/riskyusers-dismiss.md)|Nenhum | Descartar o risco de um usuário arriscado.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|id|cadeia de caracteres|ID exclusiva do usuário em risco.|
|isDeleted|boolean|Indica se o usuário foi excluído. Os valores possíveis são: `true` e `false`.|
|isProcessing|booliano|Indica se o estado de risco de um usuário está sendo processado pelo back-end.|
|riskLastUpdatedDateTime|DateTimeOffset|A data e a hora em que o usuário arriscado foi atualizado pela última vez.  O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`|
|riskLevel|riskLevel| Nível do usuário arriscado detectado. Os valores possíveis `low` são , , , , , `medium` `high` `hidden` `none` `unknownFutureValue` .  |
|riskState|riskState| Estado do risco do usuário. Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.  |
|riskDetail|riskDetail| Os valores possíveis `none` são , , , , , , , `adminGeneratedTemporaryPassword` , , , `userPerformedSecuredPasswordChange` , , `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised` `unknownFutureValue` .  |
|userDisplayName|cadeia de caracteres|Nome de exibição de usuário arriscado.|
|userPrincipalName|string|Nome principal do usuário arriscado.|

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
