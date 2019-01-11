---
title: tipo de recurso de targetResourceServicePrincipal
description: Indica o ServicePrincipalId para o recurso que afetado a atividade de auditoria. Derivado do recurso targetResource.
localization_priority: Normal
ms.openlocfilehash: 37bd63851ca9169afb669c710ef4cb2c150ea615
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839596"
---
# <a name="targetresourceserviceprincipal-resource-type"></a><span data-ttu-id="e16ea-104">tipo de recurso de targetResourceServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="e16ea-104">targetResourceServicePrincipal resource type</span></span>
<span data-ttu-id="e16ea-105">Indica o ServicePrincipalId para o recurso que afetado a atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="e16ea-105">Indicates the ServicePrincipalId for the resource that impacted the audit activity.</span></span> <span data-ttu-id="e16ea-106">Derivado do recurso [targetResource](targetresource.md) .</span><span class="sxs-lookup"><span data-stu-id="e16ea-106">Derived from the [targetResource](targetresource.md) resource.</span></span>



## <a name="properties"></a><span data-ttu-id="e16ea-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e16ea-107">Properties</span></span>
| <span data-ttu-id="e16ea-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e16ea-108">Property</span></span>     | <span data-ttu-id="e16ea-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e16ea-109">Type</span></span>   |<span data-ttu-id="e16ea-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e16ea-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e16ea-111">appId</span><span class="sxs-lookup"><span data-stu-id="e16ea-111">appId</span></span>|<span data-ttu-id="e16ea-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e16ea-112">String</span></span>|<span data-ttu-id="e16ea-113">Indica a Id exclusiva do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e16ea-113">Indicates the Unique Id of the application.</span></span> <span data-ttu-id="e16ea-114">Se refere à Id de aplicativo para um aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="e16ea-114">Refers to App Id for a specfic app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e16ea-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e16ea-115">JSON representation</span></span>

<span data-ttu-id="e16ea-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e16ea-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceServicePrincipal"
}-->

```json
{
  "appId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
