---
title: Tipo de recurso teamsDeviceUsageDistributionUserCounts
description: Representa o número de usuários por tipo de dispositivo durante o período de tempo selecionado.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2d1c716a4be9ab6ffac7b37484d7cb8bc8f01ee9
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766564"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="8261c-103">Tipo de recurso teamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="8261c-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

<span data-ttu-id="8261c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8261c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8261c-105">Representa o número de usuários por tipo de dispositivo durante o período de tempo selecionado.</span><span class="sxs-lookup"><span data-stu-id="8261c-105">Represents number of users by device type over the selected time period.</span></span>

## <a name="properties"></a><span data-ttu-id="8261c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8261c-106">Properties</span></span>

| <span data-ttu-id="8261c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8261c-107">Property</span></span>          | <span data-ttu-id="8261c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8261c-108">Type</span></span>   | <span data-ttu-id="8261c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8261c-109">Description</span></span>                                                  |
| :---------------- | :----- | ------------------------------------------------------------ |
| <span data-ttu-id="8261c-110">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8261c-110">reportRefreshDate</span></span> | <span data-ttu-id="8261c-111">Data</span><span class="sxs-lookup"><span data-stu-id="8261c-111">Date</span></span>   | <span data-ttu-id="8261c-112">A data mais recente do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8261c-112">The latest date of the content.</span></span>                              |
| <span data-ttu-id="8261c-113">web</span><span class="sxs-lookup"><span data-stu-id="8261c-113">web</span></span>               | <span data-ttu-id="8261c-114">Int64</span><span class="sxs-lookup"><span data-stu-id="8261c-114">Int64</span></span>  | <span data-ttu-id="8261c-115">O número de usuários que estavam ativos no cliente Web do Teams em dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8261c-115">The number of users who were active in the Teams web client on devices.</span></span> |
| <span data-ttu-id="8261c-116">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="8261c-116">windowsPhone</span></span>      | <span data-ttu-id="8261c-117">Int64</span><span class="sxs-lookup"><span data-stu-id="8261c-117">Int64</span></span>  | <span data-ttu-id="8261c-118">O número de usuários que estavam ativos no cliente móvel do Teams para windows phone.</span><span class="sxs-lookup"><span data-stu-id="8261c-118">The number of users who were active on the Teams mobile client for Windows phone.</span></span> |
| <span data-ttu-id="8261c-119">androidPhone</span><span class="sxs-lookup"><span data-stu-id="8261c-119">androidPhone</span></span>      | <span data-ttu-id="8261c-120">Int64</span><span class="sxs-lookup"><span data-stu-id="8261c-120">Int64</span></span>  | <span data-ttu-id="8261c-121">O número de usuários que estavam ativos no cliente móvel do Teams para Android.</span><span class="sxs-lookup"><span data-stu-id="8261c-121">The number of users who were active on the Teams mobile client for Android.</span></span> |
| <span data-ttu-id="8261c-122">ios</span><span class="sxs-lookup"><span data-stu-id="8261c-122">ios</span></span>               | <span data-ttu-id="8261c-123">Int64</span><span class="sxs-lookup"><span data-stu-id="8261c-123">Int64</span></span>  | <span data-ttu-id="8261c-124">O número de usuários que estavam ativos no cliente móvel do Teams para iOS.</span><span class="sxs-lookup"><span data-stu-id="8261c-124">The number of users who were active on the Teams mobile client for iOS.</span></span> |
| <span data-ttu-id="8261c-125">mac</span><span class="sxs-lookup"><span data-stu-id="8261c-125">mac</span></span>               | <span data-ttu-id="8261c-126">Int64</span><span class="sxs-lookup"><span data-stu-id="8261c-126">Int64</span></span>  | <span data-ttu-id="8261c-127">O número de usuários que estavam ativos no cliente de área de trabalho do Teams em um computador macOS.</span><span class="sxs-lookup"><span data-stu-id="8261c-127">The number of users who were active in the Teams desktop client on a macOS computer.</span></span> |
| <span data-ttu-id="8261c-128">windows</span><span class="sxs-lookup"><span data-stu-id="8261c-128">windows</span></span>           | <span data-ttu-id="8261c-129">Int64</span><span class="sxs-lookup"><span data-stu-id="8261c-129">Int64</span></span>  | <span data-ttu-id="8261c-130">O número de usuários que estavam ativos no cliente de área de trabalho do Teams em um computador baseado no Windows.</span><span class="sxs-lookup"><span data-stu-id="8261c-130">The number of users who were active in the Teams desktop client on a Windows-based computer.</span></span> |
| <span data-ttu-id="8261c-131">chromeOS</span><span class="sxs-lookup"><span data-stu-id="8261c-131">chromeOS</span></span>          | <span data-ttu-id="8261c-132">Int64</span><span class="sxs-lookup"><span data-stu-id="8261c-132">Int64</span></span>  | <span data-ttu-id="8261c-133">O número de usuários que estavam ativos no cliente de área de trabalho do Teams em um computador ChromeOS.</span><span class="sxs-lookup"><span data-stu-id="8261c-133">The number of users who were active in the Teams desktop client on a ChromeOS computer.</span></span> |
| <span data-ttu-id="8261c-134">linux</span><span class="sxs-lookup"><span data-stu-id="8261c-134">linux</span></span>             | <span data-ttu-id="8261c-135">Int64</span><span class="sxs-lookup"><span data-stu-id="8261c-135">Int64</span></span>  | <span data-ttu-id="8261c-136">O número de usuários que estavam ativos no cliente de área de trabalho do Teams em um computador Linux.</span><span class="sxs-lookup"><span data-stu-id="8261c-136">The number of users who were active in the Teams desktop client on a Linux computer.</span></span> |
| <span data-ttu-id="8261c-137">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8261c-137">reportPeriod</span></span>      | <span data-ttu-id="8261c-138">String</span><span class="sxs-lookup"><span data-stu-id="8261c-138">String</span></span> | <span data-ttu-id="8261c-139">O número de dias que o relatório aborda.</span><span class="sxs-lookup"><span data-stu-id="8261c-139">The number of days the report covers.</span></span>                        |

## <a name="json-representation"></a><span data-ttu-id="8261c-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8261c-140">JSON representation</span></span>

<span data-ttu-id="8261c-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8261c-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
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
  "reportPeriod": "String"
}
```


