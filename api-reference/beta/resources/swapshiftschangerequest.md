---
title: tipo de recurso swapShiftsChangeRequest
description: Representa o tipo de solicitação de turno para trocar uma mudança por outro usuário na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 80149a37dfb4d8d900066d11c315d125ff7fd670
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895565"
---
# <a name="swapshiftschangerequest-resource-type"></a><span data-ttu-id="1e224-103">tipo de recurso swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="1e224-103">swapShiftsChangeRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e224-104">Representa um tipo de solicitação de mudança para trocar uma [mudança](../resources/shift.md) por outro usuário na [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="1e224-104">Represents a type of shift request to swap a [shift](../resources/shift.md) with another user in the [team](../resources/team.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1e224-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="1e224-105">Methods</span></span>

| <span data-ttu-id="1e224-106">Método</span><span class="sxs-lookup"><span data-stu-id="1e224-106">Method</span></span>       | <span data-ttu-id="1e224-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1e224-107">Return Type</span></span> | <span data-ttu-id="1e224-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e224-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1e224-109">Get</span><span class="sxs-lookup"><span data-stu-id="1e224-109">Get</span></span>](../api/swapshiftschangerequest-get.md) | [<span data-ttu-id="1e224-110">swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="1e224-110">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="1e224-111">Leia as propriedades e os relacionamentos de um objeto **swapShiftsChangeRequest** .</span><span class="sxs-lookup"><span data-stu-id="1e224-111">Read the properties and relationships of a **swapShiftsChangeRequest** object.</span></span> |
| [<span data-ttu-id="1e224-112">Update</span><span class="sxs-lookup"><span data-stu-id="1e224-112">Update</span></span>](../api/swapshiftschangerequest-update.md) | [<span data-ttu-id="1e224-113">swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="1e224-113">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="1e224-114">Atualizar um objeto **swapShiftsChangeRequest** .</span><span class="sxs-lookup"><span data-stu-id="1e224-114">Update a **swapShiftsChangeRequest** object.</span></span> |
| [<span data-ttu-id="1e224-115">Delete</span><span class="sxs-lookup"><span data-stu-id="1e224-115">Delete</span></span>](../api/swapshiftschangerequest-delete.md) | <span data-ttu-id="1e224-116">None</span><span class="sxs-lookup"><span data-stu-id="1e224-116">None</span></span> | <span data-ttu-id="1e224-117">Excluir um objeto **swapShiftsChangeRequest** .</span><span class="sxs-lookup"><span data-stu-id="1e224-117">Delete a **swapShiftsChangeRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1e224-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e224-118">Properties</span></span>

| <span data-ttu-id="1e224-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e224-119">Property</span></span>     | <span data-ttu-id="1e224-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e224-120">Type</span></span>        | <span data-ttu-id="1e224-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e224-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1e224-122">recipientShiftId</span><span class="sxs-lookup"><span data-stu-id="1e224-122">recipientShiftId</span></span>|<span data-ttu-id="1e224-123">String</span><span class="sxs-lookup"><span data-stu-id="1e224-123">String</span></span>|<span data-ttu-id="1e224-124">ID do destinatário da solicitação de troca.</span><span class="sxs-lookup"><span data-stu-id="1e224-124">ID of the recipient of the swap request.</span></span> <span data-ttu-id="1e224-125">Esse é o usuário com o qual a solicitação deve ser trocada.</span><span class="sxs-lookup"><span data-stu-id="1e224-125">This is the user with whom the request is to swap.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e224-126">Relações</span><span class="sxs-lookup"><span data-stu-id="1e224-126">Relationships</span></span>

<span data-ttu-id="1e224-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1e224-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e224-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e224-128">JSON representation</span></span>

<span data-ttu-id="1e224-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e224-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest",
  "baseType": ""
}-->

```json
{
  "recipientShiftId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "swapShiftsChangeRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
