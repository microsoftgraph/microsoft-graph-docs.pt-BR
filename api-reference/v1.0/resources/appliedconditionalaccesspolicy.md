---
title: Tipo de recurso appliedConditionalAccessPolicy
description: Indica os atributos relacionados à política de acesso condicional ou políticas aplicadas que são disparadas pela atividade de entrada correspondente.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3aa114c23888ccc6852314e2274b8a89ca440344
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761525"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a><span data-ttu-id="3b1c4-103">Tipo de recurso appliedConditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="3b1c4-103">appliedConditionalAccessPolicy resource type</span></span>

<span data-ttu-id="3b1c4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b1c4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3b1c4-105">Indica os atributos relacionados à política de acesso condicional ou políticas aplicadas que são disparadas pela atividade de entrada correspondente.</span><span class="sxs-lookup"><span data-stu-id="3b1c4-105">Indicates the attributes related to applied conditional access policy or policies that are triggered by the corresponding sign-in activity.</span></span>

## <a name="properties"></a><span data-ttu-id="3b1c4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b1c4-106">Properties</span></span>

| <span data-ttu-id="3b1c4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b1c4-107">Property</span></span>   | <span data-ttu-id="3b1c4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b1c4-108">Type</span></span> |<span data-ttu-id="3b1c4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b1c4-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b1c4-110">displayName</span><span class="sxs-lookup"><span data-stu-id="3b1c4-110">displayName</span></span>|<span data-ttu-id="3b1c4-111">String</span><span class="sxs-lookup"><span data-stu-id="3b1c4-111">String</span></span>|<span data-ttu-id="3b1c4-112">Refere-se ao Nome da política de acesso condicional (exemplo: "Exigir MFA para Salesforce").</span><span class="sxs-lookup"><span data-stu-id="3b1c4-112">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="3b1c4-113">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="3b1c4-113">enforcedGrantControls</span></span>|<span data-ttu-id="3b1c4-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b1c4-114">String collection</span></span>|<span data-ttu-id="3b1c4-115">Refere-se aos controles de concessão imposto pela política de acesso condicional (exemplo: "Exigir autenticação multifacional").</span><span class="sxs-lookup"><span data-stu-id="3b1c4-115">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="3b1c4-116">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="3b1c4-116">enforcedSessionControls</span></span>|<span data-ttu-id="3b1c4-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b1c4-117">String collection</span></span>|<span data-ttu-id="3b1c4-118">Refere-se aos controles de sessão impostos pela política de acesso condicional (exemplo: "Exigir controles aplicados ao aplicativo").</span><span class="sxs-lookup"><span data-stu-id="3b1c4-118">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="3b1c4-119">id</span><span class="sxs-lookup"><span data-stu-id="3b1c4-119">id</span></span>|<span data-ttu-id="3b1c4-120">String</span><span class="sxs-lookup"><span data-stu-id="3b1c4-120">String</span></span>|<span data-ttu-id="3b1c4-121">GUID exclusivo da política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="3b1c4-121">Unique GUID of the conditional access policy.</span></span>|
|<span data-ttu-id="3b1c4-122">resultado</span><span class="sxs-lookup"><span data-stu-id="3b1c4-122">result</span></span>|<span data-ttu-id="3b1c4-123">String</span><span class="sxs-lookup"><span data-stu-id="3b1c4-123">String</span></span>| <span data-ttu-id="3b1c4-124">Indica o resultado da política de AC que foi disparada.</span><span class="sxs-lookup"><span data-stu-id="3b1c4-124">Indicates the result of the CA policy that was triggered.</span></span> <span data-ttu-id="3b1c4-125">Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="3b1c4-125">Possible values are:</span></span><br/>`success`<br/>`failure`<br/><span data-ttu-id="3b1c4-126">`notApplied` - A política não é aplicada porque as condições de política não foram atendidas.</span><span class="sxs-lookup"><span data-stu-id="3b1c4-126">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span><br/><span data-ttu-id="3b1c4-127">`notEnabled` - Isso ocorre devido à política em estado desabilitado.</span><span class="sxs-lookup"><span data-stu-id="3b1c4-127">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b1c4-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b1c4-128">JSON representation</span></span>

<span data-ttu-id="3b1c4-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3b1c4-129">Here is a JSON representation of the resource.</span></span>

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

