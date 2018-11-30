---
title: tipo de recurso de targetResourceGroup
description: 'Indica o tipo de grupo que foi afetado devido a atividade de auditoria. Inclui valores como os grupos de unificado versus Azure AD. '
ms.openlocfilehash: 3427f2401a0e93767f0c563842be323f66d9f21b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036420"
---
# <a name="targetresourcegroup-resource-type"></a><span data-ttu-id="8223a-104">tipo de recurso de targetResourceGroup</span><span class="sxs-lookup"><span data-stu-id="8223a-104">targetResourceGroup resource type</span></span>
<span data-ttu-id="8223a-105">Indica o tipo de grupo que foi afetado devido a atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="8223a-105">Indicates the type of group that was impacted due to the audit activity.</span></span> <span data-ttu-id="8223a-106">Inclui valores como os grupos de unificado versus Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8223a-106">Includes values like unified groups versus Azure AD</span></span> 



## <a name="properties"></a><span data-ttu-id="8223a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8223a-107">Properties</span></span>
| <span data-ttu-id="8223a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8223a-108">Property</span></span>     | <span data-ttu-id="8223a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8223a-109">Type</span></span>   |<span data-ttu-id="8223a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8223a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8223a-111">groupType</span><span class="sxs-lookup"><span data-stu-id="8223a-111">groupType</span></span>|<span data-ttu-id="8223a-112">String</span><span class="sxs-lookup"><span data-stu-id="8223a-112">String</span></span>| <span data-ttu-id="8223a-113">Os valores possíveis são: `unifiedGroups`, `azureAD`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8223a-113">Possible values are: `unifiedGroups`, `azureAD`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8223a-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8223a-114">JSON representation</span></span>

<span data-ttu-id="8223a-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8223a-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceGroup"
}-->

```json
{
  "groupType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->