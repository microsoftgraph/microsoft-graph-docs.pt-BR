---
title: tipo de recurso riskyUser
description: item de usuários arriscados
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2810ffc35b1550ae75a21b5f8baebb91c444799f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984184"
---
# <a name="riskyuser-resource-type"></a>tipo de recurso riskyUser

Namespace: microsoft.graph

Representa usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.

Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).

>**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar riskyUsers](../api/riskyuser-list.md)|coleção [riskyUser](../resources/riskyuser.md)|Obtenha uma lista dos objetos **riskyUser** e suas propriedades.|
|[Obter riskyUser](../api/riskyuser-get.md)|[riskyUser](../resources/riskyuser.md)|Leia as propriedades e os relacionamentos de um objeto **riskyUser** .|
|[Ignorar um riskyUser](../api/riskyuser-dismiss.md)|Nenhum|Descarte o risco de um ou mais objetos **riskyUser** . |
|[Confirmar um riskyUser como comprometido](../api/riskyuser-confirmcompromised.md)|Nenhum|Confirme um ou mais objetos **riskyUser** como comprometidos.|
|[Histórico de lista](../api/riskyuser-list-history.md)|coleção [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Obtenha o **riskyUserHistoryItems** da propriedade de navegação History.|
|[Obter histórico](../api/riskyuser-get-riskyuserhistoryitem.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Leia as propriedades e os relacionamentos de um objeto [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) .|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID exclusiva do usuário em risco.|
|isDeleted|Boolean|Indica se o usuário é excluído. Os valores possíveis são: `true` , `false`|
|isprocessoing|Boolean|Indica wehther que o estado arriscado de um usuário está sendo processado pelo backend|
|riskDetail|riskDetail|Detalhes do risco detectado. Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLastUpdatedDateTime|DateTimeOffset|A data e a hora em que o usuário arriscado foi atualizado pela última vez.|
|riskLevel|riskLevel|Nível do usuário arriscado detectado. Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|Estado do risco do usuário. Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|userDisplayName|Cadeia de caracteres|Nome de exibição do usuário arriscado.|
|userPrincipalName|String|Nome UPN de usuário arriscado.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|histórico|coleção [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|   A atividade relacionada à alteração no nível de risco do usuário|

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


