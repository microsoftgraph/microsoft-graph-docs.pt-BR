---
title: tipo de recurso de targetResourceGroup
description: 'Indica o tipo de grupo que foi afetado devido a atividade de auditoria. Inclui valores como os grupos de unificado versus Azure AD. '
localization_priority: Normal
ms.openlocfilehash: 2cc7e0adb1a93394b64375d05dfb6a6e349bac55
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851181"
---
# <a name="targetresourcegroup-resource-type"></a><span data-ttu-id="85b56-104">tipo de recurso de targetResourceGroup</span><span class="sxs-lookup"><span data-stu-id="85b56-104">targetResourceGroup resource type</span></span>
<span data-ttu-id="85b56-105">Indica o tipo de grupo que foi afetado devido a atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="85b56-105">Indicates the type of group that was impacted due to the audit activity.</span></span> <span data-ttu-id="85b56-106">Inclui valores como os grupos de unificado versus Azure AD.</span><span class="sxs-lookup"><span data-stu-id="85b56-106">Includes values like unified groups versus Azure AD</span></span> 



## <a name="properties"></a><span data-ttu-id="85b56-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="85b56-107">Properties</span></span>
| <span data-ttu-id="85b56-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85b56-108">Property</span></span>     | <span data-ttu-id="85b56-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="85b56-109">Type</span></span>   |<span data-ttu-id="85b56-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="85b56-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85b56-111">groupType</span><span class="sxs-lookup"><span data-stu-id="85b56-111">groupType</span></span>|<span data-ttu-id="85b56-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85b56-112">String</span></span>| <span data-ttu-id="85b56-113">Os valores possíveis são: `unifiedGroups`, `azureAD`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="85b56-113">Possible values are: `unifiedGroups`, `azureAD`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="85b56-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="85b56-114">JSON representation</span></span>

<span data-ttu-id="85b56-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="85b56-115">Here is a JSON representation of the resource.</span></span>

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
