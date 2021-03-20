---
title: Tipo de recurso appliedConditionalAccessPolicy
description: Indica os atributos relacionados à política de acesso condicional ou políticas aplicadas que são disparadas pela atividade de entrada correspondente.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: e69125d4119e7d2083189f459ad7c86816ddcd8e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952554"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a><span data-ttu-id="0cf5c-103">Tipo de recurso appliedConditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="0cf5c-103">appliedConditionalAccessPolicy resource type</span></span>

<span data-ttu-id="0cf5c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cf5c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0cf5c-105">Indica os atributos relacionados à política de acesso condicional ou políticas aplicadas que são disparadas pela atividade de entrada correspondente.</span><span class="sxs-lookup"><span data-stu-id="0cf5c-105">Indicates the attributes related to applied conditional access policy or policies that are triggered by the corresponding sign-in activity.</span></span>

## <a name="properties"></a><span data-ttu-id="0cf5c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0cf5c-106">Properties</span></span>

| <span data-ttu-id="0cf5c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0cf5c-107">Property</span></span>   | <span data-ttu-id="0cf5c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cf5c-108">Type</span></span> |<span data-ttu-id="0cf5c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cf5c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cf5c-110">displayName</span><span class="sxs-lookup"><span data-stu-id="0cf5c-110">displayName</span></span>|<span data-ttu-id="0cf5c-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cf5c-111">String</span></span>|<span data-ttu-id="0cf5c-112">Refere-se ao Nome da política de acesso condicional (exemplo: "Exigir MFA para Salesforce").</span><span class="sxs-lookup"><span data-stu-id="0cf5c-112">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="0cf5c-113">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="0cf5c-113">enforcedGrantControls</span></span>|<span data-ttu-id="0cf5c-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cf5c-114">String collection</span></span>|<span data-ttu-id="0cf5c-115">Refere-se aos controles de concessão imposto pela política de acesso condicional (exemplo: "Exigir autenticação multifacional").</span><span class="sxs-lookup"><span data-stu-id="0cf5c-115">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="0cf5c-116">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="0cf5c-116">enforcedSessionControls</span></span>|<span data-ttu-id="0cf5c-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cf5c-117">String collection</span></span>|<span data-ttu-id="0cf5c-118">Refere-se aos controles de sessão impostos pela política de acesso condicional (exemplo: "Exigir controles aplicados ao aplicativo").</span><span class="sxs-lookup"><span data-stu-id="0cf5c-118">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="0cf5c-119">id</span><span class="sxs-lookup"><span data-stu-id="0cf5c-119">id</span></span>|<span data-ttu-id="0cf5c-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cf5c-120">String</span></span>|<span data-ttu-id="0cf5c-121">Um identificador da política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="0cf5c-121">An identifier of the conditional access policy.</span></span>|
|<span data-ttu-id="0cf5c-122">resultado</span><span class="sxs-lookup"><span data-stu-id="0cf5c-122">result</span></span>|<span data-ttu-id="0cf5c-123">appliedConditionalAccessPolicyResult</span><span class="sxs-lookup"><span data-stu-id="0cf5c-123">appliedConditionalAccessPolicyResult</span></span>| <span data-ttu-id="0cf5c-124">Indica o resultado da política de AC que foi disparada.</span><span class="sxs-lookup"><span data-stu-id="0cf5c-124">Indicates the result of the CA policy that was triggered.</span></span> <span data-ttu-id="0cf5c-125">Os valores possíveis são: , , , (A política não é aplicada porque as condições de política não foram atendidas), (Isso ocorre devido à política em estado `success` `failure` `notApplied` `notEnabled` desabilitado), `unknown` , `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="0cf5c-125">Possible values are: `success`, `failure`, `notApplied` (Policy isn't applied because policy conditions were not met),`notEnabled` (This is due to the policy in disabled state), `unknown`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0cf5c-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0cf5c-126">JSON representation</span></span>

<span data-ttu-id="0cf5c-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0cf5c-127">Here is a JSON representation of the resource.</span></span>

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

