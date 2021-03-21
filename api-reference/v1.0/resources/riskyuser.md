---
title: tipo de recurso riskyUser
description: item de usuários arriscados
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 82b622838ddd5e7fb8c00a969184bdd729926b23
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961080"
---
# <a name="riskyuser-resource-type"></a>tipo de recurso riskyUser

Namespace: microsoft.graph

Representa os usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários em risco no Azure AD.

Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).

>**Observação:** Usar a API riskyUsers requer uma licença do Azure AD Premium P2.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar riskyUsers](../api/riskyuser-list.md)|[Coleção riskyUser](../resources/riskyuser.md)|Obter uma lista dos **objetos riskyUser** e suas propriedades.|
|[Obter riskyUser](../api/riskyuser-get.md)|[riskyUser](../resources/riskyuser.md)|Leia as propriedades e as relações de um **objeto riskyUser.**|
|[Descartar um riskyUser](../api/riskyuser-dismiss.md)|Nenhum|Descartar o risco de um ou mais **objetos riskyUser.** |
|[Confirmar um riskyUser como comprometido](../api/riskyuser-confirmcompromised.md)|Nenhum|Confirme um ou mais **objetos riskyUser** como comprometidos.|
|[Histórico de listas](../api/riskyuser-list-history.md)|[coleção riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Obter **os riskyUserHistoryItems** da propriedade de navegação histórico.|
|[Obter histórico](../api/riskyuser-get-riskyuserhistoryitem.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Leia as propriedades e as relações de um [objeto riskyUserHistoryItem.](../resources/riskyuserhistoryitem.md)|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID exclusiva do usuário em risco.|
|isDeleted|Booliano|Indica se o usuário foi excluído. Os valores possíveis são: `true` e `false`.|
|isProcessing|Booliano|Indica se o estado de risco de um usuário está sendo processado pelo back-end.|
|riskDetail|riskDetail|Detalhes do risco detectado. Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLastUpdatedDateTime|DateTimeOffset|A data e a hora em que o usuário arriscado foi atualizado pela última vez.  O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`|
|riskLevel|riskLevel|Nível do usuário arriscado detectado. Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|Estado do risco do usuário. Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|userDisplayName|Cadeia de caracteres|Nome de exibição de usuário arriscado.|
|userPrincipalName|Cadeia de caracteres|Nome principal do usuário arriscado.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|history|[coleção riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|   A atividade relacionada à alteração no nível de risco do usuário|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskyUser",
  "id": "String (identifier)",
  "isDeleted": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String"
}
```
