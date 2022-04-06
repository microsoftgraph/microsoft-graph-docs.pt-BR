---
title: Tipo de recurso riskyServicePrincipal
description: 'Representa as identidades de carga de trabalho do Azure AD que estão em risco, incluindo riscos para aplicativos, entidades de serviço e Identidades Gerenciadas. '
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ad89892a3cb33bb182a7df1a2e12d9355c2178b0
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723736"
---
# <a name="riskyserviceprincipal-resource-type"></a>Tipo de recurso riskyServicePrincipal

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as entidades de serviço do Azure AD que estão em risco. O Azure AD avalia continuamente o risco principal do serviço com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todas as entidades de serviço em risco no locatário do Azure AD.

Herda de [entidade](../resources/entity.md).

>**Observação:** Usar a API riskyServicePrincipal requer uma Azure AD Premium P2 de usuário.

## <a name="methods"></a>Methods

| Método                                                                                      | Tipo de retorno                                                                        | Descrição                                                     |
| :------------------------------------------------------------------------------------------ | :--------------------------------------------------------------------------------- | :-------------------------------------------------------------- |
| [Listar riskyServicePrincipals](../api/identityprotectionroot-list-riskyserviceprincipals.md) | [Coleção riskyServicePrincipal](../resources/riskyserviceprincipal.md)          | Listar entidades de serviço arriscadas e suas propriedades de risco.        |
| [Obter riskyServicePrincipal](../api/riskyserviceprincipal-get.md)                            | [riskyServicePrincipal](../resources/riskyserviceprincipal.md)                     | Obter uma entidade de serviço de risco específica e suas propriedades de risco. |
| [dismiss](../api/riskyserviceprincipal-dismiss.md)                                          | Nenhum                                                                               | Descartar o risco de uma entidade de serviço arriscada.                  |
| [confirmCompromised](../api/riskyserviceprincipal-confirmcompromised.md)                    | Nenhum                                                                               | Confirme uma entidade de serviço arriscada como comprometida.               |
| [Histórico de listas](../api/riskyserviceprincipal-list-history.md)                                | [Coleção riskyServicePrincipalHistoryItem](riskyserviceprincipalhistoryitem.md) | Obter o histórico de risco de uma entidade de serviço do Azure AD.          |

## <a name="properties"></a>Propriedades

| Propriedade                | Tipo           | Descrição                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| :---------------------- | :------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| accountEnabled          | Booliano        | `true` se a conta da entidade de serviço estiver habilitada; caso contrário, `false`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| appId                   | String         | O identificador global exclusivo do aplicativo associado (sua **propriedade appId** ), se for o caso.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| displayName             | String         | O nome de exibição da entidade de serviço.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| id                      | String         | O identificador exclusivo atribuído à entidade de serviço em risco. Herdado da [entidade](../resources/entity.md).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| isProcessing            | Boolean        | Indica se o Azure AD está  processamento do estado de risco da entidade de serviço.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| riskDetail              | riskDetail     | Detalhes do risco detectado. <br>**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Clientes P1 serão retornados `hidden`. <br/>Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, , `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, , `userPassedMFADrivenByRiskBasedPolicy``aiConfirmedSigninSafe`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, , `adminConfirmedUserCompromised`, `unknownFutureValue`, , `adminConfirmedServicePrincipalCompromised`, `adminDismissedAllRiskForServicePrincipal`. Observe que você deve usar o `Prefer: include-unknown-enum-members` header de solicitação para obter os seguintes valores nesta [enum evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `adminConfirmedServicePrincipalCompromised` , `adminDismissedAllRiskForServicePrincipal`. |
| riskLastUpdatedDateTime | DateTimeOffset | A data e a hora em que o estado de risco foi atualizado pela última vez. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2021 é `2021-01-01T00:00:00Z`. Suporta `$filter` (`eq`).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| riskLevel               | riskLevel      | Nível da identidade de carga de trabalho arriscada detectada. Os valores possíveis são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`. Suporta `$filter` (`eq`).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| riskState               | riskState      | Estado do risco da entidade de serviço. Os valores possíveis são `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| servicePrincipalType    | Cadeia de caracteres         | Identifica se a entidade de serviço representa um `Application`, um `ManagedIdentity`, ou um aplicativo herdado (`socialIdp`). Isso é definido pelo Azure AD internamente e é herdado [de servicePrincipal](../resources/servicePrincipal.md).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |

## <a name="relationships"></a>Relações

| Relação | Tipo                                                                               | Descrição                                                 |
| :----------- | :--------------------------------------------------------------------------------- | :---------------------------------------------------------- |
| history      | [Coleção riskyServicePrincipalHistoryItem](riskyserviceprincipalhistoryitem.md) | Representa o histórico de risco das entidades de serviço do Azure AD. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyServicePrincipal",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.riskyServicePrincipal",
  "id": "String (identifier)",
  "accountEnabled": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "displayName": "String",
  "appId": "String",
  "servicePrincipalType": "String"
}
```
