---
title: tipo de recurso office365ActivationsUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 21e18b35dc4e4ff639087617d679ae1583516026
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021221"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="531b4-103">tipo de recurso office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="531b4-103">office365ActivationsUserCounts resource type</span></span>

<span data-ttu-id="531b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="531b4-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="531b4-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="531b4-105">Properties</span></span>

| <span data-ttu-id="531b4-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="531b4-106">Property</span></span>                 | <span data-ttu-id="531b4-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="531b4-107">Type</span></span>   | <span data-ttu-id="531b4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="531b4-108">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="531b4-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="531b4-109">reportRefreshDate</span></span>        | <span data-ttu-id="531b4-110">Data</span><span class="sxs-lookup"><span data-stu-id="531b4-110">Date</span></span>   | <span data-ttu-id="531b4-111">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="531b4-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="531b4-112">ProductType</span><span class="sxs-lookup"><span data-stu-id="531b4-112">productType</span></span>              | <span data-ttu-id="531b4-113">String</span><span class="sxs-lookup"><span data-stu-id="531b4-113">String</span></span> | <span data-ttu-id="531b4-114">O tipo de produto como "Microsoft 365 ProPlus" ou "Project Client".</span><span class="sxs-lookup"><span data-stu-id="531b4-114">The product type such as "Microsoft 365 ProPlus" or "Project Client".</span></span> |
| <span data-ttu-id="531b4-115">atribuí</span><span class="sxs-lookup"><span data-stu-id="531b4-115">assigned</span></span>                 | <span data-ttu-id="531b4-116">Int64</span><span class="sxs-lookup"><span data-stu-id="531b4-116">Int64</span></span>  | <span data-ttu-id="531b4-117">O número de usuários foi atribuído para a licença de produto.</span><span class="sxs-lookup"><span data-stu-id="531b4-117">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="531b4-118">ativado</span><span class="sxs-lookup"><span data-stu-id="531b4-118">activated</span></span>                | <span data-ttu-id="531b4-119">Int64</span><span class="sxs-lookup"><span data-stu-id="531b4-119">Int64</span></span>  | <span data-ttu-id="531b4-120">O número de usuários que ativaram o produto.</span><span class="sxs-lookup"><span data-stu-id="531b4-120">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="531b4-121">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="531b4-121">sharedComputerActivation</span></span> | <span data-ttu-id="531b4-122">Int64</span><span class="sxs-lookup"><span data-stu-id="531b4-122">Int64</span></span>  | <span data-ttu-id="531b4-123">O número de usuários que usaram o produto em um computador compartilhado.</span><span class="sxs-lookup"><span data-stu-id="531b4-123">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="531b4-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="531b4-124">JSON representation</span></span>

<span data-ttu-id="531b4-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="531b4-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "assigned": 1024, 
  "activated": 1024,
  "sharedComputerActivation": 1024
}
```


