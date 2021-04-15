---
title: Tipo de recurso teamsDeviceUsageUserCounts
description: Representa o número de usuários diários por tipo de dispositivo.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9d7b813727a5ac9b2f7547e108bad8ee455d206b
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766571"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="34502-103">Tipo de recurso teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="34502-103">teamsDeviceUsageUserCounts resource type</span></span>

<span data-ttu-id="34502-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34502-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34502-105">Representa o número de usuários diários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34502-105">Represents number of daily users by device type.</span></span>

## <a name="properties"></a><span data-ttu-id="34502-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34502-106">Properties</span></span>

| <span data-ttu-id="34502-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34502-107">Property</span></span>          | <span data-ttu-id="34502-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="34502-108">Type</span></span>   | <span data-ttu-id="34502-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="34502-109">Description</span></span>                                                  |
| :---------------- | :----- | ------------------------------------------------------------ |
| <span data-ttu-id="34502-110">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="34502-110">reportRefreshDate</span></span> | <span data-ttu-id="34502-111">Data</span><span class="sxs-lookup"><span data-stu-id="34502-111">Date</span></span>   | <span data-ttu-id="34502-112">A data mais recente do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="34502-112">The latest date of the content.</span></span>                              |
| <span data-ttu-id="34502-113">web</span><span class="sxs-lookup"><span data-stu-id="34502-113">web</span></span>               | <span data-ttu-id="34502-114">Int64</span><span class="sxs-lookup"><span data-stu-id="34502-114">Int64</span></span>  | <span data-ttu-id="34502-115">O número de usuários que estavam ativos no cliente Web do Teams em dispositivos.</span><span class="sxs-lookup"><span data-stu-id="34502-115">The number of users who were active in the Teams web client on devices.</span></span> |
| <span data-ttu-id="34502-116">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="34502-116">windowsPhone</span></span>      | <span data-ttu-id="34502-117">Int64</span><span class="sxs-lookup"><span data-stu-id="34502-117">Int64</span></span>  | <span data-ttu-id="34502-118">O número de usuários que estavam ativos no cliente móvel do Teams para windows phone.</span><span class="sxs-lookup"><span data-stu-id="34502-118">The number of users who were active on the Teams mobile client for Windows phone.</span></span> |
| <span data-ttu-id="34502-119">androidPhone</span><span class="sxs-lookup"><span data-stu-id="34502-119">androidPhone</span></span>      | <span data-ttu-id="34502-120">Int64</span><span class="sxs-lookup"><span data-stu-id="34502-120">Int64</span></span>  | <span data-ttu-id="34502-121">O número de usuários que estavam ativos no cliente móvel do Teams para Android.</span><span class="sxs-lookup"><span data-stu-id="34502-121">The number of users who were active on the Teams mobile client for Android.</span></span> |
| <span data-ttu-id="34502-122">ios</span><span class="sxs-lookup"><span data-stu-id="34502-122">ios</span></span>               | <span data-ttu-id="34502-123">Int64</span><span class="sxs-lookup"><span data-stu-id="34502-123">Int64</span></span>  | <span data-ttu-id="34502-124">O número de usuários que estavam ativos no cliente móvel do Teams para iOS.</span><span class="sxs-lookup"><span data-stu-id="34502-124">The number of users who were active on the Teams mobile client for iOS.</span></span> |
| <span data-ttu-id="34502-125">mac</span><span class="sxs-lookup"><span data-stu-id="34502-125">mac</span></span>               | <span data-ttu-id="34502-126">Int64</span><span class="sxs-lookup"><span data-stu-id="34502-126">Int64</span></span>  | <span data-ttu-id="34502-127">O número de usuários que estavam ativos no cliente de área de trabalho do Teams em um computador macOS.</span><span class="sxs-lookup"><span data-stu-id="34502-127">The number of users who were active in the Teams desktop client on a macOS computer.</span></span> |
| <span data-ttu-id="34502-128">windows</span><span class="sxs-lookup"><span data-stu-id="34502-128">windows</span></span>           | <span data-ttu-id="34502-129">Int64</span><span class="sxs-lookup"><span data-stu-id="34502-129">Int64</span></span>  | <span data-ttu-id="34502-130">O número de usuários que estavam ativos no cliente de área de trabalho do Teams em um computador baseado no Windows.</span><span class="sxs-lookup"><span data-stu-id="34502-130">The number of users who were active in the Teams desktop client on a Windows-based computer.</span></span> |
| <span data-ttu-id="34502-131">chromeOS</span><span class="sxs-lookup"><span data-stu-id="34502-131">chromeOS</span></span>          | <span data-ttu-id="34502-132">Int64</span><span class="sxs-lookup"><span data-stu-id="34502-132">Int64</span></span>  | <span data-ttu-id="34502-133">O número de usuários que estavam ativos no cliente de área de trabalho do Teams em um computador ChromeOS.</span><span class="sxs-lookup"><span data-stu-id="34502-133">The number of users who were active in the Teams desktop client on a ChromeOS computer.</span></span> |
| <span data-ttu-id="34502-134">linux</span><span class="sxs-lookup"><span data-stu-id="34502-134">linux</span></span>             | <span data-ttu-id="34502-135">Int64</span><span class="sxs-lookup"><span data-stu-id="34502-135">Int64</span></span>  | <span data-ttu-id="34502-136">O número de usuários que estavam ativos no cliente de área de trabalho do Teams em um computador Linux.</span><span class="sxs-lookup"><span data-stu-id="34502-136">The number of users who were active in the Teams desktop client on a Linux computer.</span></span> |
| <span data-ttu-id="34502-137">reportDate</span><span class="sxs-lookup"><span data-stu-id="34502-137">reportDate</span></span>        | <span data-ttu-id="34502-138">Data</span><span class="sxs-lookup"><span data-stu-id="34502-138">Date</span></span>   | <span data-ttu-id="34502-139">A data em que os usuários realizaram as atividades.</span><span class="sxs-lookup"><span data-stu-id="34502-139">The date on which the users performed the activities.</span></span>        |
| <span data-ttu-id="34502-140">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="34502-140">reportPeriod</span></span>      | <span data-ttu-id="34502-141">String</span><span class="sxs-lookup"><span data-stu-id="34502-141">String</span></span> | <span data-ttu-id="34502-142">O número de dias que o relatório aborda.</span><span class="sxs-lookup"><span data-stu-id="34502-142">The number of days the report covers.</span></span>                        |

## <a name="representation"></a><span data-ttu-id="34502-143">representation</span><span class="sxs-lookup"><span data-stu-id="34502-143">representation</span></span>

<span data-ttu-id="34502-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34502-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "chromeOS": 1024, 
  "linux": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


