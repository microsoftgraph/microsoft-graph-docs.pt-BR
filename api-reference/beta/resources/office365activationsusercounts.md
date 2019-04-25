---
title: tipo de recurso office365ActivationsUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0d5ed2af02f429f5fd4d6e92b408d2e8e420f4d0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581510"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="093dd-103">tipo de recurso office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="093dd-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="093dd-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="093dd-104">Properties</span></span>

| <span data-ttu-id="093dd-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="093dd-105">Property</span></span>                 | <span data-ttu-id="093dd-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="093dd-106">Type</span></span>   | <span data-ttu-id="093dd-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="093dd-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="093dd-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="093dd-108">reportRefreshDate</span></span>        | <span data-ttu-id="093dd-109">Data</span><span class="sxs-lookup"><span data-stu-id="093dd-109">Date</span></span>   | <span data-ttu-id="093dd-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="093dd-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="093dd-111">ProductType</span><span class="sxs-lookup"><span data-stu-id="093dd-111">productType</span></span>              | <span data-ttu-id="093dd-112">String</span><span class="sxs-lookup"><span data-stu-id="093dd-112">String</span></span> | <span data-ttu-id="093dd-113">O tipo de produto como "Office 365 proPlus", "Project Client" ou "Visio Pro for Office 365".</span><span class="sxs-lookup"><span data-stu-id="093dd-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="093dd-114">atribuí</span><span class="sxs-lookup"><span data-stu-id="093dd-114">assigned</span></span>                 | <span data-ttu-id="093dd-115">Int64</span><span class="sxs-lookup"><span data-stu-id="093dd-115">Int64</span></span>  | <span data-ttu-id="093dd-116">O número de usuários foi atribuído para a licença de produto.</span><span class="sxs-lookup"><span data-stu-id="093dd-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="093dd-117">ativado</span><span class="sxs-lookup"><span data-stu-id="093dd-117">activated</span></span>                | <span data-ttu-id="093dd-118">Int64</span><span class="sxs-lookup"><span data-stu-id="093dd-118">Int64</span></span>  | <span data-ttu-id="093dd-119">O número de usuários que ativaram o produto.</span><span class="sxs-lookup"><span data-stu-id="093dd-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="093dd-120">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="093dd-120">sharedComputerActivation</span></span> | <span data-ttu-id="093dd-121">Int64</span><span class="sxs-lookup"><span data-stu-id="093dd-121">Int64</span></span>  | <span data-ttu-id="093dd-122">O número de usuários que usaram o produto em um computador compartilhado.</span><span class="sxs-lookup"><span data-stu-id="093dd-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="093dd-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="093dd-123">JSON representation</span></span>

<span data-ttu-id="093dd-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="093dd-124">The following is a JSON representation of the resource.</span></span>

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
