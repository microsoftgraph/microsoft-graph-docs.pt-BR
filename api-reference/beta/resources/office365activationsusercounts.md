---
title: Tipo de recurso office365ActivationsUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: a6b97aa8b74ad51158c151e9d3723ea5d1ef191b
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980749"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="34139-103">Tipo de recurso office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="34139-103">office365ActivationsUserCounts resource type</span></span>

<span data-ttu-id="34139-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34139-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="34139-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34139-105">Properties</span></span>

| <span data-ttu-id="34139-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34139-106">Property</span></span>                 | <span data-ttu-id="34139-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="34139-107">Type</span></span>   | <span data-ttu-id="34139-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="34139-108">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="34139-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="34139-109">reportRefreshDate</span></span>        | <span data-ttu-id="34139-110">Data</span><span class="sxs-lookup"><span data-stu-id="34139-110">Date</span></span>   | <span data-ttu-id="34139-111">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="34139-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="34139-112">productType</span><span class="sxs-lookup"><span data-stu-id="34139-112">productType</span></span>              | <span data-ttu-id="34139-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34139-113">String</span></span> | <span data-ttu-id="34139-114">O tipo de produto como "Microsoft 365 ProPlus" ou "Project Client".</span><span class="sxs-lookup"><span data-stu-id="34139-114">The product type such as "Microsoft 365 ProPlus" or "Project Client".</span></span> |
| <span data-ttu-id="34139-115">atribuído</span><span class="sxs-lookup"><span data-stu-id="34139-115">assigned</span></span>                 | <span data-ttu-id="34139-116">Int64</span><span class="sxs-lookup"><span data-stu-id="34139-116">Int64</span></span>  | <span data-ttu-id="34139-117">O número de usuários atribuídos à licença do produto.</span><span class="sxs-lookup"><span data-stu-id="34139-117">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="34139-118">ativado</span><span class="sxs-lookup"><span data-stu-id="34139-118">activated</span></span>                | <span data-ttu-id="34139-119">Int64</span><span class="sxs-lookup"><span data-stu-id="34139-119">Int64</span></span>  | <span data-ttu-id="34139-120">O número de usuários que ativaram o produto.</span><span class="sxs-lookup"><span data-stu-id="34139-120">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="34139-121">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="34139-121">sharedComputerActivation</span></span> | <span data-ttu-id="34139-122">Int64</span><span class="sxs-lookup"><span data-stu-id="34139-122">Int64</span></span>  | <span data-ttu-id="34139-123">O número de usuários que usaram o produto em um computador compartilhado.</span><span class="sxs-lookup"><span data-stu-id="34139-123">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="34139-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34139-124">JSON representation</span></span>

<span data-ttu-id="34139-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34139-125">The following is a JSON representation of the resource.</span></span>

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


