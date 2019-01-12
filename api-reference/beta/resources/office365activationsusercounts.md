---
title: tipo de recurso de office365ActivationsUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 3dc497e516f95f1e05167703f2b9f8aea6363a64
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917717"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="ef5e2-103">tipo de recurso de office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="ef5e2-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ef5e2-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ef5e2-104">Properties</span></span>

| <span data-ttu-id="ef5e2-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef5e2-105">Property</span></span>                 | <span data-ttu-id="ef5e2-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef5e2-106">Type</span></span>   | <span data-ttu-id="ef5e2-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef5e2-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="ef5e2-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ef5e2-108">reportRefreshDate</span></span>        | <span data-ttu-id="ef5e2-109">Data</span><span class="sxs-lookup"><span data-stu-id="ef5e2-109">Date</span></span>   | <span data-ttu-id="ef5e2-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ef5e2-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="ef5e2-111">productType</span><span class="sxs-lookup"><span data-stu-id="ef5e2-111">productType</span></span>              | <span data-ttu-id="ef5e2-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef5e2-112">String</span></span> | <span data-ttu-id="ef5e2-113">O tipo de produto, como "Office 365 ProPlus", "Cliente do projeto," ou "Visio Pro para Office 365".</span><span class="sxs-lookup"><span data-stu-id="ef5e2-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="ef5e2-114">atribuído</span><span class="sxs-lookup"><span data-stu-id="ef5e2-114">assigned</span></span>                 | <span data-ttu-id="ef5e2-115">Int64</span><span class="sxs-lookup"><span data-stu-id="ef5e2-115">Int64</span></span>  | <span data-ttu-id="ef5e2-116">O número de usuários foram atribuído para a licença do produto.</span><span class="sxs-lookup"><span data-stu-id="ef5e2-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="ef5e2-117">ativado</span><span class="sxs-lookup"><span data-stu-id="ef5e2-117">activated</span></span>                | <span data-ttu-id="ef5e2-118">Int64</span><span class="sxs-lookup"><span data-stu-id="ef5e2-118">Int64</span></span>  | <span data-ttu-id="ef5e2-119">O número de usuários que ativou o produto.</span><span class="sxs-lookup"><span data-stu-id="ef5e2-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="ef5e2-120">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="ef5e2-120">sharedComputerActivation</span></span> | <span data-ttu-id="ef5e2-121">Int64</span><span class="sxs-lookup"><span data-stu-id="ef5e2-121">Int64</span></span>  | <span data-ttu-id="ef5e2-122">O número de usuários que usaram o produto em um computador compartilhado.</span><span class="sxs-lookup"><span data-stu-id="ef5e2-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ef5e2-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ef5e2-123">JSON representation</span></span>

<span data-ttu-id="ef5e2-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ef5e2-124">The following is a JSON representation of the resource.</span></span>

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
