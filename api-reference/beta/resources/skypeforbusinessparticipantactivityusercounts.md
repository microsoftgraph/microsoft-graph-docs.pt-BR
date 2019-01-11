---
title: tipo de recurso de skypeForBusinessParticipantActivityUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 6579552ef3ca5e9fefe8690a161bef4752ad2492
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853001"
---
# <a name="skypeforbusinessparticipantactivityusercounts-resource-type"></a><span data-ttu-id="413bc-103">tipo de recurso de skypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="413bc-103">skypeForBusinessParticipantActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="413bc-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="413bc-104">Properties</span></span>

| <span data-ttu-id="413bc-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="413bc-105">Property</span></span>          | <span data-ttu-id="413bc-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="413bc-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="413bc-107">mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="413bc-107">im</span></span>                | <span data-ttu-id="413bc-108">Int64</span><span class="sxs-lookup"><span data-stu-id="413bc-108">Int64</span></span>  |
| <span data-ttu-id="413bc-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="413bc-109">audioVideo</span></span>        | <span data-ttu-id="413bc-110">Int64</span><span class="sxs-lookup"><span data-stu-id="413bc-110">Int64</span></span>  |
| <span data-ttu-id="413bc-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="413bc-111">appSharing</span></span>        | <span data-ttu-id="413bc-112">Int64</span><span class="sxs-lookup"><span data-stu-id="413bc-112">Int64</span></span>  |
| <span data-ttu-id="413bc-113">web</span><span class="sxs-lookup"><span data-stu-id="413bc-113">web</span></span>               | <span data-ttu-id="413bc-114">Int64</span><span class="sxs-lookup"><span data-stu-id="413bc-114">Int64</span></span>  |
| <span data-ttu-id="413bc-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="413bc-115">dialInOut3rdParty</span></span> | <span data-ttu-id="413bc-116">Int64</span><span class="sxs-lookup"><span data-stu-id="413bc-116">Int64</span></span>  |
| <span data-ttu-id="413bc-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="413bc-117">reportRefreshDate</span></span> | <span data-ttu-id="413bc-118">Data</span><span class="sxs-lookup"><span data-stu-id="413bc-118">Date</span></span>   |
| <span data-ttu-id="413bc-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="413bc-119">reportDate</span></span>        | <span data-ttu-id="413bc-120">Data</span><span class="sxs-lookup"><span data-stu-id="413bc-120">Date</span></span>   |
| <span data-ttu-id="413bc-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="413bc-121">reportPeriod</span></span>      | <span data-ttu-id="413bc-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="413bc-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="413bc-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="413bc-123">JSON representation</span></span>

<span data-ttu-id="413bc-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="413bc-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityUserCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 196, 
  "appSharing": 196, 
  "web": 196, 
  "dialInOut3rdParty": 196, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
