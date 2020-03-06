---
title: tipo de recurso office365ActivationsUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 78c21f33352e5f6357638de8dacc4b628b6ef93b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522481"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="3955c-103">tipo de recurso office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="3955c-103">office365ActivationsUserCounts resource type</span></span>

<span data-ttu-id="3955c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3955c-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="3955c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3955c-105">Properties</span></span>

| <span data-ttu-id="3955c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3955c-106">Property</span></span>                 | <span data-ttu-id="3955c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3955c-107">Type</span></span>   | <span data-ttu-id="3955c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3955c-108">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="3955c-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3955c-109">reportRefreshDate</span></span>        | <span data-ttu-id="3955c-110">Data</span><span class="sxs-lookup"><span data-stu-id="3955c-110">Date</span></span>   | <span data-ttu-id="3955c-111">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="3955c-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="3955c-112">ProductType</span><span class="sxs-lookup"><span data-stu-id="3955c-112">productType</span></span>              | <span data-ttu-id="3955c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3955c-113">String</span></span> | <span data-ttu-id="3955c-114">O tipo de produto como "Office 365 ProPlus", "Project Client" ou "Visio Pro for Office 365".</span><span class="sxs-lookup"><span data-stu-id="3955c-114">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="3955c-115">atribuí</span><span class="sxs-lookup"><span data-stu-id="3955c-115">assigned</span></span>                 | <span data-ttu-id="3955c-116">Int64</span><span class="sxs-lookup"><span data-stu-id="3955c-116">Int64</span></span>  | <span data-ttu-id="3955c-117">O número de usuários foi atribuído para a licença de produto.</span><span class="sxs-lookup"><span data-stu-id="3955c-117">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="3955c-118">ativado</span><span class="sxs-lookup"><span data-stu-id="3955c-118">activated</span></span>                | <span data-ttu-id="3955c-119">Int64</span><span class="sxs-lookup"><span data-stu-id="3955c-119">Int64</span></span>  | <span data-ttu-id="3955c-120">O número de usuários que ativaram o produto.</span><span class="sxs-lookup"><span data-stu-id="3955c-120">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="3955c-121">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="3955c-121">sharedComputerActivation</span></span> | <span data-ttu-id="3955c-122">Int64</span><span class="sxs-lookup"><span data-stu-id="3955c-122">Int64</span></span>  | <span data-ttu-id="3955c-123">O número de usuários que usaram o produto em um computador compartilhado.</span><span class="sxs-lookup"><span data-stu-id="3955c-123">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3955c-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3955c-124">JSON representation</span></span>

<span data-ttu-id="3955c-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3955c-125">The following is a JSON representation of the resource.</span></span>

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
