---
title: tipo de recurso appliedConditionalAccessPolicy
description: Indica os atributos relacionados à política ou políticas de acesso condicional aplicadas que são disparadas pela atividade de entrada correspondente.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d8b569436152e2a57e152f0fe2f2c632f0d2d93a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033246"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a><span data-ttu-id="6d02c-103">tipo de recurso appliedConditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="6d02c-103">appliedConditionalAccessPolicy resource type</span></span>

<span data-ttu-id="6d02c-104">Indica os atributos relacionados à política ou políticas de acesso condicional aplicadas que são disparadas pela atividade de entrada correspondente.</span><span class="sxs-lookup"><span data-stu-id="6d02c-104">Indicates the attributes related to applied conditional access policy or policies that are triggered by the corresponding sign-in activity.</span></span>

## <a name="properties"></a><span data-ttu-id="6d02c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d02c-105">Properties</span></span>

| <span data-ttu-id="6d02c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d02c-106">Property</span></span>   | <span data-ttu-id="6d02c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d02c-107">Type</span></span> |<span data-ttu-id="6d02c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d02c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d02c-109">displayName</span><span class="sxs-lookup"><span data-stu-id="6d02c-109">displayName</span></span>|<span data-ttu-id="6d02c-110">String</span><span class="sxs-lookup"><span data-stu-id="6d02c-110">String</span></span>|<span data-ttu-id="6d02c-111">Refere-se ao nome da política de acesso condicional (exemplo: "exigir MFA de Salesforce").</span><span class="sxs-lookup"><span data-stu-id="6d02c-111">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="6d02c-112">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="6d02c-112">enforcedGrantControls</span></span>|<span data-ttu-id="6d02c-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d02c-113">String collection</span></span>|<span data-ttu-id="6d02c-114">Refere-se aos controles Grant impostos pela política de acesso condicional (exemplo: "requer autenticação multifator").</span><span class="sxs-lookup"><span data-stu-id="6d02c-114">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="6d02c-115">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="6d02c-115">enforcedSessionControls</span></span>|<span data-ttu-id="6d02c-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d02c-116">String collection</span></span>|<span data-ttu-id="6d02c-117">Refere-se aos controles de sessão aplicados pela política de acesso condicional (exemplo: "exigir controles de aplicação imposta)").</span><span class="sxs-lookup"><span data-stu-id="6d02c-117">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="6d02c-118">id</span><span class="sxs-lookup"><span data-stu-id="6d02c-118">id</span></span>|<span data-ttu-id="6d02c-119">String</span><span class="sxs-lookup"><span data-stu-id="6d02c-119">String</span></span>|<span data-ttu-id="6d02c-120">GUID exclusivo da vigilância de acesso condicional. y</span><span class="sxs-lookup"><span data-stu-id="6d02c-120">Unique GUID of the conditional access polic.y</span></span>|
|<span data-ttu-id="6d02c-121">resultado</span><span class="sxs-lookup"><span data-stu-id="6d02c-121">result</span></span>|<span data-ttu-id="6d02c-122">String</span><span class="sxs-lookup"><span data-stu-id="6d02c-122">String</span></span>| <span data-ttu-id="6d02c-123">Indica o resultado da política de autoridade de certificação que foi disparada.</span><span class="sxs-lookup"><span data-stu-id="6d02c-123">Indicates the result of the CA policy that was triggered.</span></span> <span data-ttu-id="6d02c-124">Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="6d02c-124">Possible values are:</span></span><br/>`success`<br/>`failure`<br/><span data-ttu-id="6d02c-125">`notApplied`-A política não é aplicada porque as condições da política não foram atendidas.</span><span class="sxs-lookup"><span data-stu-id="6d02c-125">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span><br/><span data-ttu-id="6d02c-126">`notEnabled`– Isso ocorre devido à política em estado desabilitado.</span><span class="sxs-lookup"><span data-stu-id="6d02c-126">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d02c-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d02c-127">JSON representation</span></span>

<span data-ttu-id="6d02c-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d02c-128">Here is a JSON representation of the resource.</span></span>

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
