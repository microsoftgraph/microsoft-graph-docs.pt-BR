---
title: tipo de recurso riskyUserHistoryItem
description: ''
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7143fffecee52747109674e81e5bfbd9860df7f9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563030"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="8db20-102">tipo de recurso riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="8db20-102">riskyUserHistoryItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="8db20-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8db20-103">Properties</span></span>

| <span data-ttu-id="8db20-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8db20-104">Property</span></span>       | <span data-ttu-id="8db20-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="8db20-105">Type</span></span>    | <span data-ttu-id="8db20-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="8db20-106">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="8db20-107">userId</span><span class="sxs-lookup"><span data-stu-id="8db20-107">userId</span></span>         | <span data-ttu-id="8db20-108">string</span><span class="sxs-lookup"><span data-stu-id="8db20-108">string</span></span>  |             |
| <span data-ttu-id="8db20-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="8db20-109">initiatedBy</span></span>    | <span data-ttu-id="8db20-110">bool</span><span class="sxs-lookup"><span data-stu-id="8db20-110">bool</span></span>    |             |
| <span data-ttu-id="8db20-111">atividade</span><span class="sxs-lookup"><span data-stu-id="8db20-111">activity</span></span>       | [<span data-ttu-id="8db20-112">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="8db20-112">riskUserActivity</span></span>](riskuseractivity.md)| |

## <a name="json-representation"></a><span data-ttu-id="8db20-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8db20-113">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser"
}-->

```json
{
    "userId": "string",
    "initiatedBy": "bool",
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"}
}
```


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
   
  ]
}
-->
