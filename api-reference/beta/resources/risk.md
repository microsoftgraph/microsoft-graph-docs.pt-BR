---
title: tipo de recurso de risco
description: Agrega o nível de risco, o estado de risco e detalhes de riscos para o usuário riscado, entrar ou evento de risco.
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: 6f8fb05b39c14e3d56ddff211a5d35d77b87b814
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927265"
---
# <a name="risk-resource-type"></a>tipo de recurso de risco

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Agrega o nível de risco, o estado de risco e detalhes de riscos para o usuário riscado, entrar ou evento de risco.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|`stateDetail`|riskDetail|Fornece o motivo por trás de um estado específico de um usuário riscado, entrar ou um evento de risco. Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. O valor `none` significa que nenhuma ação foi realizada no usuário ou entrar até o momento. |
|`riskLevelAggregated`|riskLevel|Fornece o nível de risco geral de um usuário riscado, entrar ou um evento de risco. Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`. O valor `hidden` significa que o usuário ou entrar não foi habilitada para a proteção de identidade do Windows Azure AD.|
|`riskLevelDuringSignIn`|riskLeve|Fornece o nível de risco de um sign-in durante o sign-in (isto é, com base nos eventos risco em tempo real). Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`. O valor `hidden` significa que o sign-in não foi habilitado para a proteção de identidade do Windows Azure AD.|
|`state`|riskState|Fornece o 'estado de risco' de um usuário riscado, entrar ou um evento de risco. Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identityRiskEvent"
}-->

```json
{
    "stateDetail":  {"@odata.type": "microsoft.graph.riskDetail"},
    "riskLevelAggregated":  {"@odata.type": "microsoft.graph.riskLevel"},
    "riskLevelDuringSignIn":  {"@odata.type": "microsoft.graph.riskLevel"},
    "state":  {"@odata.type": "microsoft.graph.riskState"}
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
