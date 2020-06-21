---
title: tipo de recurso appliedConditionalAccessPolicy
description: Indica os atributos relacionados à política ou políticas de acesso condicional aplicadas que são disparadas pela atividade de entrada correspondente.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0e58058a174b630daa5022aed0dff78b7c2f3099
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44788686"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a><span data-ttu-id="2140c-103">tipo de recurso appliedConditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="2140c-103">appliedConditionalAccessPolicy resource type</span></span>

<span data-ttu-id="2140c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2140c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2140c-105">Indica os atributos relacionados à política ou políticas de acesso condicional aplicadas que são disparadas pela atividade de entrada correspondente.</span><span class="sxs-lookup"><span data-stu-id="2140c-105">Indicates the attributes related to applied conditional access policy or policies that are triggered by the corresponding sign-in activity.</span></span>

## <a name="properties"></a><span data-ttu-id="2140c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2140c-106">Properties</span></span>

| <span data-ttu-id="2140c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2140c-107">Property</span></span>   | <span data-ttu-id="2140c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2140c-108">Type</span></span> |<span data-ttu-id="2140c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2140c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2140c-110">displayName</span><span class="sxs-lookup"><span data-stu-id="2140c-110">displayName</span></span>|<span data-ttu-id="2140c-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2140c-111">String</span></span>|<span data-ttu-id="2140c-112">Refere-se ao nome da política de acesso condicional (exemplo: "exigir MFA de Salesforce").</span><span class="sxs-lookup"><span data-stu-id="2140c-112">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="2140c-113">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="2140c-113">enforcedGrantControls</span></span>|<span data-ttu-id="2140c-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2140c-114">String collection</span></span>|<span data-ttu-id="2140c-115">Refere-se aos controles Grant impostos pela política de acesso condicional (exemplo: "requer autenticação multifator").</span><span class="sxs-lookup"><span data-stu-id="2140c-115">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="2140c-116">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="2140c-116">enforcedSessionControls</span></span>|<span data-ttu-id="2140c-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2140c-117">String collection</span></span>|<span data-ttu-id="2140c-118">Refere-se aos controles de sessão aplicados pela política de acesso condicional (exemplo: "exigir controles de aplicação imposta)").</span><span class="sxs-lookup"><span data-stu-id="2140c-118">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="2140c-119">id</span><span class="sxs-lookup"><span data-stu-id="2140c-119">id</span></span>|<span data-ttu-id="2140c-120">String</span><span class="sxs-lookup"><span data-stu-id="2140c-120">String</span></span>|<span data-ttu-id="2140c-121">GUID exclusivo da política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="2140c-121">Unique GUID of the conditional access policy.</span></span>|
|<span data-ttu-id="2140c-122">resultado</span><span class="sxs-lookup"><span data-stu-id="2140c-122">result</span></span>|<span data-ttu-id="2140c-123">String</span><span class="sxs-lookup"><span data-stu-id="2140c-123">String</span></span>| <span data-ttu-id="2140c-124">Indica o resultado da política de autoridade de certificação que foi disparada.</span><span class="sxs-lookup"><span data-stu-id="2140c-124">Indicates the result of the CA policy that was triggered.</span></span> <span data-ttu-id="2140c-125">Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="2140c-125">Possible values are:</span></span><br/>`success`<br/>`failure`<br/><span data-ttu-id="2140c-126">`notApplied`-A política não é aplicada porque as condições da política não foram atendidas.</span><span class="sxs-lookup"><span data-stu-id="2140c-126">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span><br/><span data-ttu-id="2140c-127">`notEnabled`– Isso ocorre devido à política em estado desabilitado.</span><span class="sxs-lookup"><span data-stu-id="2140c-127">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2140c-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2140c-128">JSON representation</span></span>

<span data-ttu-id="2140c-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2140c-129">Here is a JSON representation of the resource.</span></span>

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
