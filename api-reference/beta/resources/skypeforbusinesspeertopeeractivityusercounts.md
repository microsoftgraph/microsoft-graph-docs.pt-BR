---
title: tipo de recurso skypeForBusinessPeerToPeerActivityUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 619e581fcdd25dda10be7210aefe5db8e4dcd8b7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503881"
---
# <a name="skypeforbusinesspeertopeeractivityusercounts-resource-type"></a><span data-ttu-id="6d060-103">tipo de recurso skypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="6d060-103">skypeForBusinessPeerToPeerActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6d060-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d060-104">Properties</span></span>

| <span data-ttu-id="6d060-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d060-105">Property</span></span>          | <span data-ttu-id="6d060-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d060-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="6d060-107">respectiva</span><span class="sxs-lookup"><span data-stu-id="6d060-107">im</span></span>                | <span data-ttu-id="6d060-108">Int64</span><span class="sxs-lookup"><span data-stu-id="6d060-108">Int64</span></span>  |
| <span data-ttu-id="6d060-109">audio</span><span class="sxs-lookup"><span data-stu-id="6d060-109">audio</span></span>             | <span data-ttu-id="6d060-110">Int64</span><span class="sxs-lookup"><span data-stu-id="6d060-110">Int64</span></span>  |
| <span data-ttu-id="6d060-111">video</span><span class="sxs-lookup"><span data-stu-id="6d060-111">video</span></span>             | <span data-ttu-id="6d060-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6d060-112">Int64</span></span>  |
| <span data-ttu-id="6d060-113">appSharing</span><span class="sxs-lookup"><span data-stu-id="6d060-113">appSharing</span></span>        | <span data-ttu-id="6d060-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6d060-114">Int64</span></span>  |
| <span data-ttu-id="6d060-115">transferência de</span><span class="sxs-lookup"><span data-stu-id="6d060-115">fileTransfer</span></span>      | <span data-ttu-id="6d060-116">Int64</span><span class="sxs-lookup"><span data-stu-id="6d060-116">Int64</span></span>  |
| <span data-ttu-id="6d060-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6d060-117">reportRefreshDate</span></span> | <span data-ttu-id="6d060-118">Data</span><span class="sxs-lookup"><span data-stu-id="6d060-118">Date</span></span>   |
| <span data-ttu-id="6d060-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="6d060-119">reportDate</span></span>        | <span data-ttu-id="6d060-120">Data</span><span class="sxs-lookup"><span data-stu-id="6d060-120">Date</span></span>   |
| <span data-ttu-id="6d060-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6d060-121">reportPeriod</span></span>      | <span data-ttu-id="6d060-122">String</span><span class="sxs-lookup"><span data-stu-id="6d060-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6d060-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d060-123">JSON representation</span></span>

<span data-ttu-id="6d060-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d060-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts"
} -->

```json
{
  "im": 1024, 
  "audio": 1024, 
  "video": 1024, 
  "appSharing": 1024, 
  "fileTransfer": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
