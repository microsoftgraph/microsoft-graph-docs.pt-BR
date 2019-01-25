---
title: tipo de recurso de risco
description: Agrega o nível de risco, o estado de risco e detalhes de riscos para o usuário riscado, entrar ou evento de risco.
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: 48fda9624e45072240bc694b8b5e152fe3ef0764
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524818"
---
# <a name="risk-resource-type"></a><span data-ttu-id="da304-103">tipo de recurso de risco</span><span class="sxs-lookup"><span data-stu-id="da304-103">risk resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da304-104">Agrega o nível de risco, o estado de risco e detalhes de riscos para o usuário riscado, entrar ou evento de risco.</span><span class="sxs-lookup"><span data-stu-id="da304-104">Aggregates the risk level, risk state and risk detail for the risky user, sign in, or risk event.</span></span>

## <a name="properties"></a><span data-ttu-id="da304-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da304-105">Properties</span></span>

| <span data-ttu-id="da304-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da304-106">Property</span></span>   | <span data-ttu-id="da304-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="da304-107">Type</span></span>|<span data-ttu-id="da304-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="da304-108">Description</span></span>|
|:---------------|:--------|:----------|
|`stateDetail`|<span data-ttu-id="da304-109">riskDetail</span><span class="sxs-lookup"><span data-stu-id="da304-109">riskDetail</span></span>|<span data-ttu-id="da304-110">Fornece o motivo por trás de um estado específico de um usuário riscado, entrar ou um evento de risco.</span><span class="sxs-lookup"><span data-stu-id="da304-110">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="da304-111">Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="da304-111">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="da304-112">O valor `none` significa que nenhuma ação foi realizada no usuário ou entrar até o momento.</span><span class="sxs-lookup"><span data-stu-id="da304-112">The value `none` means that no action has been performed on the user or sign-in so far.</span></span> |
|`riskLevelAggregated`|<span data-ttu-id="da304-113">riskLevel</span><span class="sxs-lookup"><span data-stu-id="da304-113">riskLevel</span></span>|<span data-ttu-id="da304-114">Fornece o nível de risco geral de um usuário riscado, entrar ou um evento de risco.</span><span class="sxs-lookup"><span data-stu-id="da304-114">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="da304-115">Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="da304-115">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="da304-116">O valor `hidden` significa que o usuário ou entrar não foi habilitada para a proteção de identidade do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="da304-116">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskLevelDuringSignIn`|<span data-ttu-id="da304-117">riskLeve</span><span class="sxs-lookup"><span data-stu-id="da304-117">riskLeve</span></span>|<span data-ttu-id="da304-118">Fornece o nível de risco de um sign-in durante o sign-in (isto é, com base nos eventos risco em tempo real).</span><span class="sxs-lookup"><span data-stu-id="da304-118">Provides the risk level of a sign-in during the sign-in (i.e. based on the real-time risk events).</span></span> <span data-ttu-id="da304-119">Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="da304-119">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="da304-120">O valor `hidden` significa que o sign-in não foi habilitado para a proteção de identidade do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="da304-120">The value `hidden` means the sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`state`|<span data-ttu-id="da304-121">riskState</span><span class="sxs-lookup"><span data-stu-id="da304-121">riskState</span></span>|<span data-ttu-id="da304-122">Fornece o 'estado de risco' de um usuário riscado, entrar ou um evento de risco.</span><span class="sxs-lookup"><span data-stu-id="da304-122">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="da304-123">Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="da304-123">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="da304-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da304-124">JSON representation</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/risk.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
