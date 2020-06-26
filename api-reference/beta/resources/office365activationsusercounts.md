---
title: tipo de recurso office365ActivationsUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: b8746d58b03b15a3118e8fc51a42e61e3c22cb78
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896802"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="fe948-103">tipo de recurso office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="fe948-103">office365ActivationsUserCounts resource type</span></span>

<span data-ttu-id="fe948-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe948-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="fe948-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe948-105">Properties</span></span>

| <span data-ttu-id="fe948-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe948-106">Property</span></span>                 | <span data-ttu-id="fe948-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe948-107">Type</span></span>   | <span data-ttu-id="fe948-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe948-108">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="fe948-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fe948-109">reportRefreshDate</span></span>        | <span data-ttu-id="fe948-110">Data</span><span class="sxs-lookup"><span data-stu-id="fe948-110">Date</span></span>   | <span data-ttu-id="fe948-111">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="fe948-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="fe948-112">ProductType</span><span class="sxs-lookup"><span data-stu-id="fe948-112">productType</span></span>              | <span data-ttu-id="fe948-113">String</span><span class="sxs-lookup"><span data-stu-id="fe948-113">String</span></span> | <span data-ttu-id="fe948-114">O tipo de produto como "Microsoft 365 ProPlus" ou "Project Client".</span><span class="sxs-lookup"><span data-stu-id="fe948-114">The product type such as "Microsoft 365 ProPlus" or "Project Client".</span></span> |
| <span data-ttu-id="fe948-115">atribuí</span><span class="sxs-lookup"><span data-stu-id="fe948-115">assigned</span></span>                 | <span data-ttu-id="fe948-116">Int64</span><span class="sxs-lookup"><span data-stu-id="fe948-116">Int64</span></span>  | <span data-ttu-id="fe948-117">O número de usuários foi atribuído para a licença de produto.</span><span class="sxs-lookup"><span data-stu-id="fe948-117">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="fe948-118">ativado</span><span class="sxs-lookup"><span data-stu-id="fe948-118">activated</span></span>                | <span data-ttu-id="fe948-119">Int64</span><span class="sxs-lookup"><span data-stu-id="fe948-119">Int64</span></span>  | <span data-ttu-id="fe948-120">O número de usuários que ativaram o produto.</span><span class="sxs-lookup"><span data-stu-id="fe948-120">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="fe948-121">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="fe948-121">sharedComputerActivation</span></span> | <span data-ttu-id="fe948-122">Int64</span><span class="sxs-lookup"><span data-stu-id="fe948-122">Int64</span></span>  | <span data-ttu-id="fe948-123">O número de usuários que usaram o produto em um computador compartilhado.</span><span class="sxs-lookup"><span data-stu-id="fe948-123">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fe948-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe948-124">JSON representation</span></span>

<span data-ttu-id="fe948-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe948-125">The following is a JSON representation of the resource.</span></span>

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
