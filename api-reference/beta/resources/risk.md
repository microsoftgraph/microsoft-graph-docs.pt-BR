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
# <a name="risk-resource-type"></a><span data-ttu-id="6a9b9-103">tipo de recurso de risco</span><span class="sxs-lookup"><span data-stu-id="6a9b9-103">risk resource type</span></span>

> <span data-ttu-id="6a9b9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6a9b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a9b9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6a9b9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a9b9-106">Agrega o nível de risco, o estado de risco e detalhes de riscos para o usuário riscado, entrar ou evento de risco.</span><span class="sxs-lookup"><span data-stu-id="6a9b9-106">Aggregates the risk level, risk state and risk detail for the risky user, sign in, or risk event.</span></span>

## <a name="properties"></a><span data-ttu-id="6a9b9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a9b9-107">Properties</span></span>

| <span data-ttu-id="6a9b9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a9b9-108">Property</span></span>   | <span data-ttu-id="6a9b9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a9b9-109">Type</span></span>|<span data-ttu-id="6a9b9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a9b9-110">Description</span></span>|
|:---------------|:--------|:----------|
|`stateDetail`|<span data-ttu-id="6a9b9-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="6a9b9-111">riskDetail</span></span>|<span data-ttu-id="6a9b9-112">Fornece o motivo por trás de um estado específico de um usuário riscado, entrar ou um evento de risco.</span><span class="sxs-lookup"><span data-stu-id="6a9b9-112">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="6a9b9-113">Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6a9b9-113">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="6a9b9-114">O valor `none` significa que nenhuma ação foi realizada no usuário ou entrar até o momento.</span><span class="sxs-lookup"><span data-stu-id="6a9b9-114">The value `none` means that no action has been performed on the user or sign-in so far.</span></span> |
|`riskLevelAggregated`|<span data-ttu-id="6a9b9-115">riskLevel</span><span class="sxs-lookup"><span data-stu-id="6a9b9-115">riskLevel</span></span>|<span data-ttu-id="6a9b9-116">Fornece o nível de risco geral de um usuário riscado, entrar ou um evento de risco.</span><span class="sxs-lookup"><span data-stu-id="6a9b9-116">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="6a9b9-117">Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6a9b9-117">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="6a9b9-118">O valor `hidden` significa que o usuário ou entrar não foi habilitada para a proteção de identidade do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6a9b9-118">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskLevelDuringSignIn`|<span data-ttu-id="6a9b9-119">riskLeve</span><span class="sxs-lookup"><span data-stu-id="6a9b9-119">riskLeve</span></span>|<span data-ttu-id="6a9b9-120">Fornece o nível de risco de um sign-in durante o sign-in (isto é, com base nos eventos risco em tempo real).</span><span class="sxs-lookup"><span data-stu-id="6a9b9-120">Provides the risk level of a sign-in during the sign-in (i.e. based on the real-time risk events).</span></span> <span data-ttu-id="6a9b9-121">Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6a9b9-121">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="6a9b9-122">O valor `hidden` significa que o sign-in não foi habilitado para a proteção de identidade do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6a9b9-122">The value `hidden` means the sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`state`|<span data-ttu-id="6a9b9-123">riskState</span><span class="sxs-lookup"><span data-stu-id="6a9b9-123">riskState</span></span>|<span data-ttu-id="6a9b9-124">Fornece o 'estado de risco' de um usuário riscado, entrar ou um evento de risco.</span><span class="sxs-lookup"><span data-stu-id="6a9b9-124">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="6a9b9-125">Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6a9b9-125">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6a9b9-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a9b9-126">JSON representation</span></span>

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
