---
title: tipo de recurso de conditionalAccessPolicy
description: Indica que os atributos relacionados a uma política de acesso condicional ou diretivas que é disparado pela atividade correspondente entrar
ms.openlocfilehash: 56a06d6b5fcba96dc472eb63fe24ba3920b0dd09
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040872"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="c149e-103">tipo de recurso de conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="c149e-103">conditionalAccessPolicy resource type</span></span>
<span data-ttu-id="c149e-104">Indica que os atributos relacionados a uma política de acesso condicional ou diretivas que é disparado pela atividade correspondente entrar</span><span class="sxs-lookup"><span data-stu-id="c149e-104">Indicates the attributes related a conditional access policy or policies that's triggered by the corresponding sign-in activity</span></span>



## <a name="properties"></a><span data-ttu-id="c149e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c149e-105">Properties</span></span>
| <span data-ttu-id="c149e-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c149e-106">Property</span></span>     | <span data-ttu-id="c149e-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c149e-107">Type</span></span>   |<span data-ttu-id="c149e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c149e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c149e-109">displayName</span><span class="sxs-lookup"><span data-stu-id="c149e-109">displayName</span></span>|<span data-ttu-id="c149e-110">String</span><span class="sxs-lookup"><span data-stu-id="c149e-110">String</span></span>|<span data-ttu-id="c149e-111">Refere-se com o nome da política de acesso condicional (exemplo: "Exigir MFA para a equipe de vendas").</span><span class="sxs-lookup"><span data-stu-id="c149e-111">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="c149e-112">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="c149e-112">enforcedGrantControls</span></span>|<span data-ttu-id="c149e-113">String collection</span><span class="sxs-lookup"><span data-stu-id="c149e-113">String collection</span></span>|<span data-ttu-id="c149e-114">Refere-se aos controles grant impostos com a política de acesso condicional (exemplo: "Exigem a autenticação multifator").</span><span class="sxs-lookup"><span data-stu-id="c149e-114">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="c149e-115">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="c149e-115">enforcedSessionControls</span></span>|<span data-ttu-id="c149e-116">String collection</span><span class="sxs-lookup"><span data-stu-id="c149e-116">String collection</span></span>|<span data-ttu-id="c149e-117">Refere-se aos controles sessão impostos com a política de acesso condicional (exemplo: "Exigem controles app imposto").</span><span class="sxs-lookup"><span data-stu-id="c149e-117">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="c149e-118">id</span><span class="sxs-lookup"><span data-stu-id="c149e-118">id</span></span>|<span data-ttu-id="c149e-119">String</span><span class="sxs-lookup"><span data-stu-id="c149e-119">String</span></span>|<span data-ttu-id="c149e-120">GUID exclusivo da política de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="c149e-120">Unique GUID of the conditional access policy</span></span>|
|<span data-ttu-id="c149e-121">result</span><span class="sxs-lookup"><span data-stu-id="c149e-121">result</span></span>|<span data-ttu-id="c149e-122">String</span><span class="sxs-lookup"><span data-stu-id="c149e-122">String</span></span>| <span data-ttu-id="c149e-123">Indica o resultado da política de autoridade de certificação que tiver sido disparado. Valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="c149e-123">Indicates the result of the CA policy that was triggered.Possible values are:</span></span><br/> `success` <br/> `failure` <br/> <span data-ttu-id="c149e-124">`notApplied`-Diretiva não será aplicada, porque as condições da diretiva não foram atendidas.</span><span class="sxs-lookup"><span data-stu-id="c149e-124">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span> <br/> <span data-ttu-id="c149e-125">`notEnabled`-Isso acontece devido à política em estado desabilitado.</span><span class="sxs-lookup"><span data-stu-id="c149e-125">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c149e-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c149e-126">JSON representation</span></span>

<span data-ttu-id="c149e-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c149e-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
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
  "description": "conditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->