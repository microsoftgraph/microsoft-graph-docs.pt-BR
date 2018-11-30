---
title: tipo de recurso de targetResourcePolicy
description: 'Indica a política que foi afetada pela atividade de auditoria. Derivado do recurso targetResource.   '
ms.openlocfilehash: 20486c535d0df4b3745f5cfc3414b320a9374075
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038420"
---
# <a name="targetresourcepolicy-resource-type"></a><span data-ttu-id="cb5b0-104">tipo de recurso de targetResourcePolicy</span><span class="sxs-lookup"><span data-stu-id="cb5b0-104">targetResourcePolicy resource type</span></span>
<span data-ttu-id="cb5b0-105">Indica a política que foi afetada pela atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="cb5b0-105">Indicates the policy that was impacted by the audit activity.</span></span> <span data-ttu-id="cb5b0-106">Derivado do recurso [targetResource](targetresource.md) .</span><span class="sxs-lookup"><span data-stu-id="cb5b0-106">Derived from the [targetResource](targetresource.md) resource.</span></span>   



## <a name="properties"></a><span data-ttu-id="cb5b0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb5b0-107">Properties</span></span>
| <span data-ttu-id="cb5b0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb5b0-108">Property</span></span>     | <span data-ttu-id="cb5b0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb5b0-109">Type</span></span>   |<span data-ttu-id="cb5b0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb5b0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb5b0-111">policyType</span><span class="sxs-lookup"><span data-stu-id="cb5b0-111">policyType</span></span>|<span data-ttu-id="cb5b0-112">String</span><span class="sxs-lookup"><span data-stu-id="cb5b0-112">String</span></span>|<span data-ttu-id="cb5b0-113">Indica o nome da política que alterado ou foi direcionados da alteração</span><span class="sxs-lookup"><span data-stu-id="cb5b0-113">Indicates the Policy Name that changed or was targetted for change</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb5b0-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb5b0-114">JSON representation</span></span>

<span data-ttu-id="cb5b0-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cb5b0-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourcePolicy"
}-->

```json
{
  "policyType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourcePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->