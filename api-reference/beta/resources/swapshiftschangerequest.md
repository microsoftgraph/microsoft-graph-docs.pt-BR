---
title: tipo de recurso swapShiftsChangeRequest
description: Representa o tipo de solicitação de turno para trocar uma mudança por outro usuário na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a172737f40572b29358ecdc6fba804db2a8b80e5
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951955"
---
# <a name="swapshiftschangerequest-resource-type"></a><span data-ttu-id="4c1f2-103">tipo de recurso swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="4c1f2-103">swapShiftsChangeRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c1f2-104">Representa um tipo de solicitação de mudança para trocar uma [mudança](../resources/shift.md) por outro usuário na [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="4c1f2-104">Represents a type of shift request to swap a [shift](../resources/shift.md) with another user in the [team](../resources/team.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4c1f2-105">Methods</span><span class="sxs-lookup"><span data-stu-id="4c1f2-105">Methods</span></span>

| <span data-ttu-id="4c1f2-106">Método</span><span class="sxs-lookup"><span data-stu-id="4c1f2-106">Method</span></span>       | <span data-ttu-id="4c1f2-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4c1f2-107">Return Type</span></span> | <span data-ttu-id="4c1f2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c1f2-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4c1f2-109">List</span><span class="sxs-lookup"><span data-stu-id="4c1f2-109">List</span></span>](../api/swapshiftschangerequest-list.md) | <span data-ttu-id="4c1f2-110">Coleção de [swapShiftsChangeRequest](swapshiftschangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="4c1f2-110">Collection of [swapShiftsChangeRequest](swapshiftschangerequest.md)</span></span> | <span data-ttu-id="4c1f2-111">Listar as propriedades e os relacionamentos dos objetos **swapShiftsChangeRequest** em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="4c1f2-111">List the properties and relationships of **swapShiftsChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="4c1f2-112">Create</span><span class="sxs-lookup"><span data-stu-id="4c1f2-112">Create</span></span>](../api/swapshiftschangerequest-post.md) | [<span data-ttu-id="4c1f2-113">swapshiftschangerequest</span><span class="sxs-lookup"><span data-stu-id="4c1f2-113">swapshiftschangerequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="4c1f2-114">Criar uma instância de um objeto swapshiftschangerequest.</span><span class="sxs-lookup"><span data-stu-id="4c1f2-114">Create an instance of an swapshiftschangerequest object.</span></span> |
| [<span data-ttu-id="4c1f2-115">Get</span><span class="sxs-lookup"><span data-stu-id="4c1f2-115">Get</span></span>](../api/swapshiftschangerequest-get.md) | [<span data-ttu-id="4c1f2-116">swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="4c1f2-116">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="4c1f2-117">Leia as propriedades e os relacionamentos de um objeto **swapShiftsChangeRequest** .</span><span class="sxs-lookup"><span data-stu-id="4c1f2-117">Read the properties and relationships of a **swapShiftsChangeRequest** object.</span></span> |
|[<span data-ttu-id="4c1f2-118">Aprovar</span><span class="sxs-lookup"><span data-stu-id="4c1f2-118">Approve</span></span>](../api/swapshiftschangerequest-approve.md)|<span data-ttu-id="4c1f2-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4c1f2-119">None</span></span>|<span data-ttu-id="4c1f2-120">Aprovar um swapshiftschangerequest.</span><span class="sxs-lookup"><span data-stu-id="4c1f2-120">Approve an swapshiftschangerequest.</span></span> |

## <a name="properties"></a><span data-ttu-id="4c1f2-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4c1f2-121">Properties</span></span>

| <span data-ttu-id="4c1f2-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c1f2-122">Property</span></span>     | <span data-ttu-id="4c1f2-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c1f2-123">Type</span></span>        | <span data-ttu-id="4c1f2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c1f2-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4c1f2-125">recipientShiftId</span><span class="sxs-lookup"><span data-stu-id="4c1f2-125">recipientShiftId</span></span>|<span data-ttu-id="4c1f2-126">String</span><span class="sxs-lookup"><span data-stu-id="4c1f2-126">String</span></span>|<span data-ttu-id="4c1f2-127">ID do destinatário da solicitação de troca.</span><span class="sxs-lookup"><span data-stu-id="4c1f2-127">ID of the recipient of the swap request.</span></span> <span data-ttu-id="4c1f2-128">Esse é o usuário com o qual a solicitação deve ser trocada.</span><span class="sxs-lookup"><span data-stu-id="4c1f2-128">This is the user with whom the request is to swap.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c1f2-129">Relações</span><span class="sxs-lookup"><span data-stu-id="4c1f2-129">Relationships</span></span>

<span data-ttu-id="4c1f2-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4c1f2-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c1f2-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4c1f2-131">JSON representation</span></span>

<span data-ttu-id="4c1f2-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4c1f2-132">The following is a JSON representation of the resource.</span></span>

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
