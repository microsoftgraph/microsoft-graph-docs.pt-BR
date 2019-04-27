---
title: tipo de recurso changeTrackedEntity
description: ''
localization_priority: Normal
ms.openlocfilehash: 838aeca84b6928c709a3c4775c95ab3ef8fd7692
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33347936"
---
# <a name="changetrackedentity-resource-type"></a><span data-ttu-id="6bc73-102">tipo de recurso changeTrackedEntity</span><span class="sxs-lookup"><span data-stu-id="6bc73-102">changeTrackedEntity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="6bc73-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6bc73-103">Properties</span></span>
|<span data-ttu-id="6bc73-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6bc73-104">Property</span></span>|<span data-ttu-id="6bc73-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bc73-105">Type</span></span>|<span data-ttu-id="6bc73-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bc73-106">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bc73-107">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6bc73-107">createdDateTime</span></span>| <span data-ttu-id="6bc73-108">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bc73-108">DateTimeOffset</span></span>| |
|<span data-ttu-id="6bc73-109">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6bc73-109">lastModifiedDateTime</span></span>| <span data-ttu-id="6bc73-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bc73-110">DateTimeOffset</span></span>| |
|<span data-ttu-id="6bc73-111">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6bc73-111">lastModifiedBy</span></span>| [<span data-ttu-id="6bc73-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="6bc73-112">identitySet</span></span>](identityset.md) | |

## <a name="relationships"></a><span data-ttu-id="6bc73-113">Relações</span><span class="sxs-lookup"><span data-stu-id="6bc73-113">Relationships</span></span>
<span data-ttu-id="6bc73-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6bc73-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6bc73-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6bc73-115">JSON Representation</span></span>
<span data-ttu-id="6bc73-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6bc73-116">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.changeTrackedEntity",
  "baseType":"microsoft.graph.entity",
  "abstract":true
}-->

``` json
{
    "createdDateTime":"String (timestamp)",
    "lastModifiedDateTime" :"String (timestamp)",
    "lastModifiedBy":{"@odata.type":"microsoft.graph.identitySet"}
}
```



