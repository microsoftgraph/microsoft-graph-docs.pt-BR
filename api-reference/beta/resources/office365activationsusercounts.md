---
title: tipo de recurso de office365ActivationsUserCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 90d9d2d8616f166eb9d8b87967898daa0468db54
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039736"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="26678-103">tipo de recurso de office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="26678-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="26678-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="26678-104">Properties</span></span>

| <span data-ttu-id="26678-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26678-105">Property</span></span>                 | <span data-ttu-id="26678-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="26678-106">Type</span></span>   | <span data-ttu-id="26678-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="26678-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="26678-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="26678-108">reportRefreshDate</span></span>        | <span data-ttu-id="26678-109">Data</span><span class="sxs-lookup"><span data-stu-id="26678-109">Date</span></span>   | <span data-ttu-id="26678-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="26678-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="26678-111">productType</span><span class="sxs-lookup"><span data-stu-id="26678-111">productType</span></span>              | <span data-ttu-id="26678-112">String</span><span class="sxs-lookup"><span data-stu-id="26678-112">String</span></span> | <span data-ttu-id="26678-113">O tipo de produto, como "Office 365 ProPlus", "Cliente do projeto," ou "Visio Pro para Office 365".</span><span class="sxs-lookup"><span data-stu-id="26678-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="26678-114">atribuído</span><span class="sxs-lookup"><span data-stu-id="26678-114">assigned</span></span>                 | <span data-ttu-id="26678-115">Int64</span><span class="sxs-lookup"><span data-stu-id="26678-115">Int64</span></span>  | <span data-ttu-id="26678-116">O número de usuários foram atribuído para a licença do produto.</span><span class="sxs-lookup"><span data-stu-id="26678-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="26678-117">ativado</span><span class="sxs-lookup"><span data-stu-id="26678-117">activated</span></span>                | <span data-ttu-id="26678-118">Int64</span><span class="sxs-lookup"><span data-stu-id="26678-118">Int64</span></span>  | <span data-ttu-id="26678-119">O número de usuários que ativou o produto.</span><span class="sxs-lookup"><span data-stu-id="26678-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="26678-120">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="26678-120">sharedComputerActivation</span></span> | <span data-ttu-id="26678-121">Int64</span><span class="sxs-lookup"><span data-stu-id="26678-121">Int64</span></span>  | <span data-ttu-id="26678-122">O número de usuários que usaram o produto em um computador compartilhado.</span><span class="sxs-lookup"><span data-stu-id="26678-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="26678-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="26678-123">JSON representation</span></span>

<span data-ttu-id="26678-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="26678-124">The following is a JSON representation of the resource.</span></span>

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
