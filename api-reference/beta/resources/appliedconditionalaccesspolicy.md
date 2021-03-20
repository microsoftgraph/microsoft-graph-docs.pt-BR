---
title: Tipo de recurso appliedConditionalAccessPolicy
description: Indica os atributos relacionados à política de acesso condicional ou políticas aplicadas que são disparadas pela atividade de entrada correspondente.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: ffb91b315772d017ce039237e353df68daa47bfc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952186"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a><span data-ttu-id="ea05c-103">Tipo de recurso appliedConditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="ea05c-103">appliedConditionalAccessPolicy resource type</span></span>

<span data-ttu-id="ea05c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea05c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea05c-105">Indica os atributos relacionados à política de acesso condicional ou políticas aplicadas que são disparadas pela atividade de entrada correspondente.</span><span class="sxs-lookup"><span data-stu-id="ea05c-105">Indicates the attributes related to applied conditional access policy or policies that are triggered by the corresponding sign-in activity.</span></span>

## <a name="properties"></a><span data-ttu-id="ea05c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea05c-106">Properties</span></span>

| <span data-ttu-id="ea05c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea05c-107">Property</span></span>   | <span data-ttu-id="ea05c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea05c-108">Type</span></span> |<span data-ttu-id="ea05c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea05c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea05c-110">conditionsSatisfied</span><span class="sxs-lookup"><span data-stu-id="ea05c-110">conditionsSatisfied</span></span>|<span data-ttu-id="ea05c-111">conditionalAccessConditions</span><span class="sxs-lookup"><span data-stu-id="ea05c-111">conditionalAccessConditions</span></span>|<span data-ttu-id="ea05c-112">Refere-se às condições de política de acesso condicional que são atendidas.</span><span class="sxs-lookup"><span data-stu-id="ea05c-112">Refers to the conditional access policy conditions that are satisfied.</span></span> <span data-ttu-id="ea05c-113">Os valores possíveis são: `none`, `application`, `users`, `devicePlatform`, `location`, `clientType`, `signInRisk`, `userRisk`, `time`, `deviceState`, `client`.</span><span class="sxs-lookup"><span data-stu-id="ea05c-113">Possible values are: `none`, `application`, `users`, `devicePlatform`, `location`, `clientType`, `signInRisk`, `userRisk`, `time`, `deviceState`, `client`.</span></span>|
|<span data-ttu-id="ea05c-114">conditionsNotSatisfied</span><span class="sxs-lookup"><span data-stu-id="ea05c-114">conditionsNotSatisfied</span></span>|<span data-ttu-id="ea05c-115">conditionalAccessConditions</span><span class="sxs-lookup"><span data-stu-id="ea05c-115">conditionalAccessConditions</span></span>|<span data-ttu-id="ea05c-116">Refere-se às condições de política de acesso condicional que não estão atendidas.</span><span class="sxs-lookup"><span data-stu-id="ea05c-116">Refers to the conditional access policy conditions that are not satisfied.</span></span> <span data-ttu-id="ea05c-117">Os valores possíveis são: `none`, `application`, `users`, `devicePlatform`, `location`, `clientType`, `signInRisk`, `userRisk`, `time`, `deviceState`, `client`.</span><span class="sxs-lookup"><span data-stu-id="ea05c-117">Possible values are: `none`, `application`, `users`, `devicePlatform`, `location`, `clientType`, `signInRisk`, `userRisk`, `time`, `deviceState`, `client`.</span></span>|
|<span data-ttu-id="ea05c-118">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="ea05c-118">enforcedGrantControls</span></span>|<span data-ttu-id="ea05c-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea05c-119">String collection</span></span>|<span data-ttu-id="ea05c-120">Refere-se aos controles de concessão imposto pela política de acesso condicional (exemplo: "Exigir autenticação multifacional").</span><span class="sxs-lookup"><span data-stu-id="ea05c-120">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="ea05c-121">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="ea05c-121">enforcedSessionControls</span></span>|<span data-ttu-id="ea05c-122">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea05c-122">String collection</span></span>|<span data-ttu-id="ea05c-123">Refere-se aos controles de sessão impostos pela política de acesso condicional (exemplo: "Exigir controles aplicados ao aplicativo").</span><span class="sxs-lookup"><span data-stu-id="ea05c-123">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="ea05c-124">id</span><span class="sxs-lookup"><span data-stu-id="ea05c-124">id</span></span>|<span data-ttu-id="ea05c-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea05c-125">String</span></span>|<span data-ttu-id="ea05c-126">Identificador da política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="ea05c-126">Identifier of the conditional access policy.</span></span>|
|<span data-ttu-id="ea05c-127">resultado</span><span class="sxs-lookup"><span data-stu-id="ea05c-127">result</span></span>|<span data-ttu-id="ea05c-128">appliedConditionalAccessPolicyResult</span><span class="sxs-lookup"><span data-stu-id="ea05c-128">appliedConditionalAccessPolicyResult</span></span>| <span data-ttu-id="ea05c-129">Indica o resultado da política de AC que foi disparada.</span><span class="sxs-lookup"><span data-stu-id="ea05c-129">Indicates the result of the CA policy that was triggered.</span></span> <span data-ttu-id="ea05c-130">Os valores possíveis são: , , , (A política não é aplicada porque as condições de política não foram atendidas), (Isso ocorre devido à política em estado `success` desabilitado), , , `failure` , `notApplied` `notEnabled` `unknown` `unknownFutureValue` `reportOnlySuccess` `reportOnlyFailure` , `reportOnlyNotApplied``reportOnlyInterrupted`</span><span class="sxs-lookup"><span data-stu-id="ea05c-130">Possible values are: `success`, `failure`, `notApplied` (Policy isn't applied because policy conditions were not met),`notEnabled` (This is due to the policy in disabled state), `unknown`, `unknownFutureValue`, `reportOnlySuccess`, `reportOnlyFailure`, `reportOnlyNotApplied`, `reportOnlyInterrupted`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea05c-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea05c-131">JSON representation</span></span>

<span data-ttu-id="ea05c-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea05c-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
}-->

```json
{
  "displayName": "String",
  "enforcedGrantControls": ["String"],
  "enforcedSessionControls": ["String"],
  "id": "String",
  "result": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appliedConditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
