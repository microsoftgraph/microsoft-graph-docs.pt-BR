---
title: tipo de recurso office365ActivationCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7bc21be693a5c68ecd5c6a1e4e44d53c9261acdb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505463"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="a4bb5-103">tipo de recurso office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="a4bb5-103">office365ActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a4bb5-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a4bb5-104">Properties</span></span>

| <span data-ttu-id="a4bb5-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4bb5-105">Property</span></span>          | <span data-ttu-id="a4bb5-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4bb5-106">Type</span></span>   | <span data-ttu-id="a4bb5-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4bb5-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="a4bb5-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a4bb5-108">reportRefreshDate</span></span> | <span data-ttu-id="a4bb5-109">Data</span><span class="sxs-lookup"><span data-stu-id="a4bb5-109">Date</span></span>   | <span data-ttu-id="a4bb5-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="a4bb5-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="a4bb5-111">ProductType</span><span class="sxs-lookup"><span data-stu-id="a4bb5-111">productType</span></span>       | <span data-ttu-id="a4bb5-112">String</span><span class="sxs-lookup"><span data-stu-id="a4bb5-112">String</span></span> | <span data-ttu-id="a4bb5-113">O tipo de produto, como "Office 365 proPlus", "Project Client" ou "Visio Pro for Office 365".</span><span class="sxs-lookup"><span data-stu-id="a4bb5-113">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="a4bb5-114">Windows</span><span class="sxs-lookup"><span data-stu-id="a4bb5-114">windows</span></span>           | <span data-ttu-id="a4bb5-115">Int64</span><span class="sxs-lookup"><span data-stu-id="a4bb5-115">Int64</span></span>  | <span data-ttu-id="a4bb5-116">A contagem de ativação no Windows.</span><span class="sxs-lookup"><span data-stu-id="a4bb5-116">The activation count on Windows.</span></span> <span data-ttu-id="a4bb5-117">Esse número inclui todas as ativações em qualquer computador Windows.</span><span class="sxs-lookup"><span data-stu-id="a4bb5-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="a4bb5-118">mac</span><span class="sxs-lookup"><span data-stu-id="a4bb5-118">mac</span></span>               | <span data-ttu-id="a4bb5-119">Int64</span><span class="sxs-lookup"><span data-stu-id="a4bb5-119">Int64</span></span>  | <span data-ttu-id="a4bb5-120">A contagem de ativação no Mac OS.</span><span class="sxs-lookup"><span data-stu-id="a4bb5-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="a4bb5-121">Android</span><span class="sxs-lookup"><span data-stu-id="a4bb5-121">android</span></span>           | <span data-ttu-id="a4bb5-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a4bb5-122">Int64</span></span>  | <span data-ttu-id="a4bb5-123">A contagem de ativação em um dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="a4bb5-123">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="a4bb5-124">emiti</span><span class="sxs-lookup"><span data-stu-id="a4bb5-124">ios</span></span>               | <span data-ttu-id="a4bb5-125">Int64</span><span class="sxs-lookup"><span data-stu-id="a4bb5-125">Int64</span></span>  | <span data-ttu-id="a4bb5-126">A contagem de ativação no iOS.</span><span class="sxs-lookup"><span data-stu-id="a4bb5-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="a4bb5-127">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="a4bb5-127">windows10Mobile</span></span>   | <span data-ttu-id="a4bb5-128">Int64</span><span class="sxs-lookup"><span data-stu-id="a4bb5-128">Int64</span></span>  | <span data-ttu-id="a4bb5-129">A contagem de ativação no Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="a4bb5-129">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a4bb5-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a4bb5-130">JSON representation</span></span>

<span data-ttu-id="a4bb5-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a4bb5-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "windows": 1024, 
  "mac": 1024, 
  "android": 1024, 
  "ios": 1024, 
  "windows10Mobile": 1024
}
```
