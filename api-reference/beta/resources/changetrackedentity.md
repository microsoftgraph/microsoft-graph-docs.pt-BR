---
title: tipo de recurso changeTrackedEntity
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3815b22c7bd76a894df0e98415e0c30bb77decd1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974049"
---
# <a name="changetrackedentity-resource-type"></a><span data-ttu-id="201da-102">tipo de recurso changeTrackedEntity</span><span class="sxs-lookup"><span data-stu-id="201da-102">changeTrackedEntity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="201da-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="201da-103">Properties</span></span>
|<span data-ttu-id="201da-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="201da-104">Property</span></span>|<span data-ttu-id="201da-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="201da-105">Type</span></span>|<span data-ttu-id="201da-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="201da-106">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="201da-107">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="201da-107">createdDateTime</span></span>| <span data-ttu-id="201da-108">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="201da-108">DateTimeOffset</span></span>| |
|<span data-ttu-id="201da-109">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="201da-109">lastModifiedDateTime</span></span>| <span data-ttu-id="201da-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="201da-110">DateTimeOffset</span></span>| |
|<span data-ttu-id="201da-111">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="201da-111">lastModifiedBy</span></span>| [<span data-ttu-id="201da-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="201da-112">identitySet</span></span>](identityset.md) | |

## <a name="relationships"></a><span data-ttu-id="201da-113">Relações</span><span class="sxs-lookup"><span data-stu-id="201da-113">Relationships</span></span>
<span data-ttu-id="201da-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="201da-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="201da-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="201da-115">JSON Representation</span></span>
<span data-ttu-id="201da-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="201da-116">Here is a JSON representation of the resource.</span></span>
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



