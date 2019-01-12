---
title: tipo de recurso de mailboxUsageStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 44b97c7b18264e01c86b34bfd8265246f80ab031
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917864"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="df3ec-103">tipo de recurso de mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="df3ec-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="df3ec-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df3ec-104">Properties</span></span>

| <span data-ttu-id="df3ec-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df3ec-105">Property</span></span>           | <span data-ttu-id="df3ec-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="df3ec-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="df3ec-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="df3ec-107">reportRefreshDate</span></span>  | <span data-ttu-id="df3ec-108">Data</span><span class="sxs-lookup"><span data-stu-id="df3ec-108">Date</span></span>   |
| <span data-ttu-id="df3ec-109">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="df3ec-109">storageUsedInBytes</span></span> | <span data-ttu-id="df3ec-110">Int64</span><span class="sxs-lookup"><span data-stu-id="df3ec-110">Int64</span></span>  |
| <span data-ttu-id="df3ec-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="df3ec-111">reportDate</span></span>         | <span data-ttu-id="df3ec-112">Data</span><span class="sxs-lookup"><span data-stu-id="df3ec-112">Date</span></span>   |
| <span data-ttu-id="df3ec-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="df3ec-113">reportPeriod</span></span>       | <span data-ttu-id="df3ec-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df3ec-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="df3ec-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df3ec-115">JSON representation</span></span>

<span data-ttu-id="df3ec-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df3ec-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
