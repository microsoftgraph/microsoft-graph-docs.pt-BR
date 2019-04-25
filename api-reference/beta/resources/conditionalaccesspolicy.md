---
title: tipo de recurso conditionalAccessPolicy
description: Indica os atributos relacionados a uma política de acesso condicional ou políticas disparadas pela atividade de entrada correspondente
localization_priority: Normal
ms.openlocfilehash: 7b043e739f84715fb02fbdbd25599e5cfccc284a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543368"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="844c6-103">tipo de recurso conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="844c6-103">conditionalAccessPolicy resource type</span></span>
<span data-ttu-id="844c6-104">Indica os atributos relacionados a uma política de acesso condicional ou políticas disparadas pela atividade de entrada correspondente</span><span class="sxs-lookup"><span data-stu-id="844c6-104">Indicates the attributes related a conditional access policy or policies that's triggered by the corresponding sign-in activity</span></span>



## <a name="properties"></a><span data-ttu-id="844c6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="844c6-105">Properties</span></span>
| <span data-ttu-id="844c6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="844c6-106">Property</span></span>     | <span data-ttu-id="844c6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="844c6-107">Type</span></span>   |<span data-ttu-id="844c6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="844c6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="844c6-109">displayName</span><span class="sxs-lookup"><span data-stu-id="844c6-109">displayName</span></span>|<span data-ttu-id="844c6-110">String</span><span class="sxs-lookup"><span data-stu-id="844c6-110">String</span></span>|<span data-ttu-id="844c6-111">Refere-se ao nome da política de acesso condicional (exemplo: "exigir MFA de Salesforce").</span><span class="sxs-lookup"><span data-stu-id="844c6-111">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="844c6-112">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="844c6-112">enforcedGrantControls</span></span>|<span data-ttu-id="844c6-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="844c6-113">String collection</span></span>|<span data-ttu-id="844c6-114">Refere-se aos controles Grant impostos pela política de acesso condicional (exemplo: "requer autenticação multifator").</span><span class="sxs-lookup"><span data-stu-id="844c6-114">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="844c6-115">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="844c6-115">enforcedSessionControls</span></span>|<span data-ttu-id="844c6-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="844c6-116">String collection</span></span>|<span data-ttu-id="844c6-117">Refere-se aos controles de sessão aplicados pela política de acesso condicional (exemplo: "exigir controles de aplicação imposta)").</span><span class="sxs-lookup"><span data-stu-id="844c6-117">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="844c6-118">id</span><span class="sxs-lookup"><span data-stu-id="844c6-118">id</span></span>|<span data-ttu-id="844c6-119">String</span><span class="sxs-lookup"><span data-stu-id="844c6-119">String</span></span>|<span data-ttu-id="844c6-120">GUID exclusivo da política de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="844c6-120">Unique GUID of the conditional access policy</span></span>|
|<span data-ttu-id="844c6-121">result</span><span class="sxs-lookup"><span data-stu-id="844c6-121">result</span></span>|<span data-ttu-id="844c6-122">String</span><span class="sxs-lookup"><span data-stu-id="844c6-122">String</span></span>| <span data-ttu-id="844c6-123">Indica o resultado da política de autoridade de certificação que foi disparada. Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="844c6-123">Indicates the result of the CA policy that was triggered.Possible values are:</span></span><br/> `success` <br/> `failure` <br/> <span data-ttu-id="844c6-124">`notApplied`-A política não é aplicada porque as condições da política não foram atendidas.</span><span class="sxs-lookup"><span data-stu-id="844c6-124">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span> <br/> <span data-ttu-id="844c6-125">`notEnabled`– Isso ocorre devido à política em estado desabilitado.</span><span class="sxs-lookup"><span data-stu-id="844c6-125">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="844c6-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="844c6-126">JSON representation</span></span>

<span data-ttu-id="844c6-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="844c6-127">Here is a JSON representation of the resource.</span></span>

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
