---
title: tipo de recurso riskyUser
description: item de usuários arriscados
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 8d01e80acf9f05061cf69998d6ba94c444b67dd1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078613"
---
# <a name="riskyuser-resource-type"></a>tipo de recurso riskyUser

Namespace: microsoft.graph

Representa os usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários em risco no Azure AD.

Para obter mais informações sobre eventos de risco, [consulte Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).

>**Observação:** Usar a API riskyUsers requer uma Azure AD Premium P2 de usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar riskyUsers](../api/riskyuser-list.md)|[Coleção riskyUser](../resources/riskyuser.md)|Obter uma lista dos **objetos riskyUser** e suas propriedades.|
|[Obter riskyUser](../api/riskyuser-get.md)|[riskyUser](../resources/riskyuser.md)|Leia as propriedades e as relações de um **objeto riskyUser.**|
|[Descartar um riskyUser](../api/riskyuser-dismiss.md)|Nenhum(a)|Descartar o risco de um ou mais **objetos riskyUser.** |
|[Confirmar um riskyUser como comprometido](../api/riskyuser-confirmcompromised.md)|Nenhum(a)|Confirme um ou mais **objetos riskyUser** como comprometidos.|
|[Histórico de listas](../api/riskyuser-list-history.md)|[coleção riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Obter **os riskyUserHistoryItems** da propriedade de navegação histórico.|
|[Obter histórico](../api/riskyuser-get-riskyuserhistoryitem.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Leia as propriedades e as relações de um [objeto riskyUserHistoryItem.](../resources/riskyuserhistoryitem.md)|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID exclusiva do usuário em risco.|
|isDeleted|Booliano|Indica se o usuário foi excluído. Os valores possíveis são: `true` e `false`.|
|isProcessing|Boolean|Indica se o estado de risco de um usuário está sendo processado pelo back-end.|
|riskDetail|riskDetail|Detalhes do risco detectado. Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLastUpdatedDateTime|DateTimeOffset|A data e a hora em que o usuário arriscado foi atualizado pela última vez.  O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
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
