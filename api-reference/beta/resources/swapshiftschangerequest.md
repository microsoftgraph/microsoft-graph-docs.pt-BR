---
title: tipo de recurso swapShiftsChangeRequest
description: Representa o tipo de solicitação de turno para trocar uma mudança por outro usuário na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b0fbc0f392a6efa1b0a0ba5f1568451a6fe7d1cf
ms.sourcegitcommit: 31a9b4cb3d0f905f123475a4c1a86f5b1e59b935
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2020
ms.locfileid: "42219752"
---
# <a name="swapshiftschangerequest-resource-type"></a><span data-ttu-id="f5c48-103">tipo de recurso swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="f5c48-103">swapShiftsChangeRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5c48-104">Representa um tipo de solicitação de mudança para trocar uma [mudança](../resources/shift.md) por outro usuário na [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="f5c48-104">Represents a type of shift request to swap a [shift](../resources/shift.md) with another user in the [team](../resources/team.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f5c48-105">Methods</span><span class="sxs-lookup"><span data-stu-id="f5c48-105">Methods</span></span>

| <span data-ttu-id="f5c48-106">Método</span><span class="sxs-lookup"><span data-stu-id="f5c48-106">Method</span></span>       | <span data-ttu-id="f5c48-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f5c48-107">Return Type</span></span> | <span data-ttu-id="f5c48-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5c48-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f5c48-109">List</span><span class="sxs-lookup"><span data-stu-id="f5c48-109">List</span></span>](../api/swapshiftschangerequest-list.md) | <span data-ttu-id="f5c48-110">Coleção de [swapShiftsChangeRequest](swapshiftschangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="f5c48-110">Collection of [swapShiftsChangeRequest](swapshiftschangerequest.md)</span></span> | <span data-ttu-id="f5c48-111">Listar as propriedades e os relacionamentos dos objetos **swapShiftsChangeRequest** em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="f5c48-111">List the properties and relationships of **swapShiftsChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="f5c48-112">Create</span><span class="sxs-lookup"><span data-stu-id="f5c48-112">Create</span></span>](../api/swapshiftschangerequest-post.md) | [<span data-ttu-id="f5c48-113">swapshiftschangerequest</span><span class="sxs-lookup"><span data-stu-id="f5c48-113">swapshiftschangerequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="f5c48-114">Criar uma instância de um objeto swapshiftschangerequest.</span><span class="sxs-lookup"><span data-stu-id="f5c48-114">Create an instance of an swapshiftschangerequest object.</span></span> |
| [<span data-ttu-id="f5c48-115">Get</span><span class="sxs-lookup"><span data-stu-id="f5c48-115">Get</span></span>](../api/swapshiftschangerequest-get.md) | [<span data-ttu-id="f5c48-116">swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="f5c48-116">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="f5c48-117">Leia as propriedades e os relacionamentos de um objeto **swapShiftsChangeRequest** .</span><span class="sxs-lookup"><span data-stu-id="f5c48-117">Read the properties and relationships of a **swapShiftsChangeRequest** object.</span></span> |
|[<span data-ttu-id="f5c48-118">Aprovar</span><span class="sxs-lookup"><span data-stu-id="f5c48-118">Approve</span></span>](../api/swapshiftschangerequest-approve.md)|<span data-ttu-id="f5c48-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f5c48-119">None</span></span>|<span data-ttu-id="f5c48-120">Aprovar um **swapShiftsChangeRequest**.</span><span class="sxs-lookup"><span data-stu-id="f5c48-120">Approve a **swapShiftsChangeRequest**.</span></span> |
|[<span data-ttu-id="f5c48-121">Aceito</span><span class="sxs-lookup"><span data-stu-id="f5c48-121">Decline</span></span>](../api/swapshiftschangerequest-decline.md)|<span data-ttu-id="f5c48-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f5c48-122">None</span></span>|<span data-ttu-id="f5c48-123">Recusar um **swapShiftsChangeRequest**.</span><span class="sxs-lookup"><span data-stu-id="f5c48-123">Decline a **swapShiftsChangeRequest**.</span></span>|

## <a name="properties"></a><span data-ttu-id="f5c48-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5c48-124">Properties</span></span>

| <span data-ttu-id="f5c48-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5c48-125">Property</span></span>     | <span data-ttu-id="f5c48-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5c48-126">Type</span></span>        | <span data-ttu-id="f5c48-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5c48-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f5c48-128">recipientShiftId</span><span class="sxs-lookup"><span data-stu-id="f5c48-128">recipientShiftId</span></span>|<span data-ttu-id="f5c48-129">String</span><span class="sxs-lookup"><span data-stu-id="f5c48-129">String</span></span>|<span data-ttu-id="f5c48-130">ID do destinatário da solicitação de troca.</span><span class="sxs-lookup"><span data-stu-id="f5c48-130">ID of the recipient of the swap request.</span></span> <span data-ttu-id="f5c48-131">Esse é o usuário com o qual a solicitação deve ser trocada.</span><span class="sxs-lookup"><span data-stu-id="f5c48-131">This is the user with whom the request is to swap.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5c48-132">Relações</span><span class="sxs-lookup"><span data-stu-id="f5c48-132">Relationships</span></span>

<span data-ttu-id="f5c48-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f5c48-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5c48-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5c48-134">JSON representation</span></span>

<span data-ttu-id="f5c48-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f5c48-135">The following is a JSON representation of the resource.</span></span>

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
