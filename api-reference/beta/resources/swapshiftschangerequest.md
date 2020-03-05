---
title: tipo de recurso swapShiftsChangeRequest
description: Representa o tipo de solicitação de turno para trocar uma mudança por outro usuário na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 96589309cbeb2880e533b5607dc05beec78894ed
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520265"
---
# <a name="swapshiftschangerequest-resource-type"></a><span data-ttu-id="57ba7-103">tipo de recurso swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="57ba7-103">swapShiftsChangeRequest resource type</span></span>

<span data-ttu-id="57ba7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="57ba7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57ba7-105">Representa um tipo de solicitação de mudança para trocar uma [mudança](../resources/shift.md) por outro usuário na [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="57ba7-105">Represents a type of shift request to swap a [shift](../resources/shift.md) with another user in the [team](../resources/team.md).</span></span>

## <a name="methods"></a><span data-ttu-id="57ba7-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="57ba7-106">Methods</span></span>

| <span data-ttu-id="57ba7-107">Método</span><span class="sxs-lookup"><span data-stu-id="57ba7-107">Method</span></span>       | <span data-ttu-id="57ba7-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="57ba7-108">Return Type</span></span> | <span data-ttu-id="57ba7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="57ba7-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="57ba7-110">List</span><span class="sxs-lookup"><span data-stu-id="57ba7-110">List</span></span>](../api/swapshiftschangerequest-list.md) | <span data-ttu-id="57ba7-111">Coleção de [swapShiftsChangeRequest](swapshiftschangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="57ba7-111">Collection of [swapShiftsChangeRequest](swapshiftschangerequest.md)</span></span> | <span data-ttu-id="57ba7-112">Listar as propriedades e os relacionamentos dos objetos **swapShiftsChangeRequest** em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="57ba7-112">List the properties and relationships of **swapShiftsChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="57ba7-113">Create</span><span class="sxs-lookup"><span data-stu-id="57ba7-113">Create</span></span>](../api/swapshiftschangerequest-post.md) | [<span data-ttu-id="57ba7-114">swapshiftschangerequest</span><span class="sxs-lookup"><span data-stu-id="57ba7-114">swapshiftschangerequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="57ba7-115">Criar uma instância de um objeto swapshiftschangerequest.</span><span class="sxs-lookup"><span data-stu-id="57ba7-115">Create an instance of an swapshiftschangerequest object.</span></span> |
| [<span data-ttu-id="57ba7-116">Get</span><span class="sxs-lookup"><span data-stu-id="57ba7-116">Get</span></span>](../api/swapshiftschangerequest-get.md) | [<span data-ttu-id="57ba7-117">swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="57ba7-117">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="57ba7-118">Leia as propriedades e os relacionamentos de um objeto **swapShiftsChangeRequest** .</span><span class="sxs-lookup"><span data-stu-id="57ba7-118">Read the properties and relationships of a **swapShiftsChangeRequest** object.</span></span> |
|[<span data-ttu-id="57ba7-119">Aprovar</span><span class="sxs-lookup"><span data-stu-id="57ba7-119">Approve</span></span>](../api/swapshiftschangerequest-approve.md)|<span data-ttu-id="57ba7-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="57ba7-120">None</span></span>|<span data-ttu-id="57ba7-121">Aprovar um **swapShiftsChangeRequest**.</span><span class="sxs-lookup"><span data-stu-id="57ba7-121">Approve a **swapShiftsChangeRequest**.</span></span> |
|[<span data-ttu-id="57ba7-122">Aceito</span><span class="sxs-lookup"><span data-stu-id="57ba7-122">Decline</span></span>](../api/swapshiftschangerequest-decline.md)|<span data-ttu-id="57ba7-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="57ba7-123">None</span></span>|<span data-ttu-id="57ba7-124">Recusar um **swapShiftsChangeRequest**.</span><span class="sxs-lookup"><span data-stu-id="57ba7-124">Decline a **swapShiftsChangeRequest**.</span></span>|

## <a name="properties"></a><span data-ttu-id="57ba7-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57ba7-125">Properties</span></span>

| <span data-ttu-id="57ba7-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57ba7-126">Property</span></span>     | <span data-ttu-id="57ba7-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="57ba7-127">Type</span></span>        | <span data-ttu-id="57ba7-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="57ba7-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="57ba7-129">recipientShiftId</span><span class="sxs-lookup"><span data-stu-id="57ba7-129">recipientShiftId</span></span>|<span data-ttu-id="57ba7-130">String</span><span class="sxs-lookup"><span data-stu-id="57ba7-130">String</span></span>|<span data-ttu-id="57ba7-131">ID do destinatário da solicitação de troca.</span><span class="sxs-lookup"><span data-stu-id="57ba7-131">ID of the recipient of the swap request.</span></span> <span data-ttu-id="57ba7-132">Esse é o usuário com o qual a solicitação deve ser trocada.</span><span class="sxs-lookup"><span data-stu-id="57ba7-132">This is the user with whom the request is to swap.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57ba7-133">Relações</span><span class="sxs-lookup"><span data-stu-id="57ba7-133">Relationships</span></span>

<span data-ttu-id="57ba7-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="57ba7-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="57ba7-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57ba7-135">JSON representation</span></span>

<span data-ttu-id="57ba7-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57ba7-136">The following is a JSON representation of the resource.</span></span>

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
