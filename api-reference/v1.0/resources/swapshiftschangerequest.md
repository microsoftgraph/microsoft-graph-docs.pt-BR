---
title: tipo de recurso swapShiftsChangeRequest
description: Representa o tipo de solicitação de turno para trocar uma mudança por outro usuário na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5a3902669028a26abdb8d88e09334ccefe414d42
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154967"
---
# <a name="swapshiftschangerequest-resource-type"></a><span data-ttu-id="f7046-103">tipo de recurso swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="f7046-103">swapShiftsChangeRequest resource type</span></span>

<span data-ttu-id="f7046-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7046-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f7046-105">Representa um tipo de solicitação de mudança para trocar uma [mudança](../resources/shift.md) por outro usuário na [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="f7046-105">Represents a type of shift request to swap a [shift](../resources/shift.md) with another user in the [team](../resources/team.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f7046-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f7046-106">Methods</span></span>

| <span data-ttu-id="f7046-107">Método</span><span class="sxs-lookup"><span data-stu-id="f7046-107">Method</span></span>       | <span data-ttu-id="f7046-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f7046-108">Return Type</span></span> | <span data-ttu-id="f7046-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7046-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f7046-110">List</span><span class="sxs-lookup"><span data-stu-id="f7046-110">List</span></span>](../api/swapshiftschangerequest-list.md) | <span data-ttu-id="f7046-111">Coleção de [swapShiftsChangeRequest](swapshiftschangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="f7046-111">Collection of [swapShiftsChangeRequest](swapshiftschangerequest.md)</span></span> | <span data-ttu-id="f7046-112">Listar as propriedades e os relacionamentos dos objetos **swapShiftsChangeRequest** em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="f7046-112">List the properties and relationships of **swapShiftsChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="f7046-113">Create</span><span class="sxs-lookup"><span data-stu-id="f7046-113">Create</span></span>](../api/swapshiftschangerequest-post.md) | [<span data-ttu-id="f7046-114">swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="f7046-114">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="f7046-115">Criar uma instância de um objeto **swapShiftsChangeRequest** .</span><span class="sxs-lookup"><span data-stu-id="f7046-115">Create an instance of a **swapShiftsChangeRequest** object.</span></span> |
| [<span data-ttu-id="f7046-116">Get</span><span class="sxs-lookup"><span data-stu-id="f7046-116">Get</span></span>](../api/swapshiftschangerequest-get.md) | [<span data-ttu-id="f7046-117">swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="f7046-117">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="f7046-118">Leia as propriedades e os relacionamentos de um objeto **swapShiftsChangeRequest** .</span><span class="sxs-lookup"><span data-stu-id="f7046-118">Read the properties and relationships of a **swapShiftsChangeRequest** object.</span></span> |
|[<span data-ttu-id="f7046-119">Aprovar</span><span class="sxs-lookup"><span data-stu-id="f7046-119">Approve</span></span>](../api/swapshiftschangerequest-approve.md)|<span data-ttu-id="f7046-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f7046-120">None</span></span>|<span data-ttu-id="f7046-121">Aprovar um **swapShiftsChangeRequest**.</span><span class="sxs-lookup"><span data-stu-id="f7046-121">Approve a **swapShiftsChangeRequest**.</span></span> |
|[<span data-ttu-id="f7046-122">Aceito</span><span class="sxs-lookup"><span data-stu-id="f7046-122">Decline</span></span>](../api/swapshiftschangerequest-decline.md)|<span data-ttu-id="f7046-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f7046-123">None</span></span>|<span data-ttu-id="f7046-124">Recusar um **swapShiftsChangeRequest**.</span><span class="sxs-lookup"><span data-stu-id="f7046-124">Decline a **swapShiftsChangeRequest**.</span></span>|

## <a name="properties"></a><span data-ttu-id="f7046-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f7046-125">Properties</span></span>

| <span data-ttu-id="f7046-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7046-126">Property</span></span>     | <span data-ttu-id="f7046-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7046-127">Type</span></span>        | <span data-ttu-id="f7046-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7046-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f7046-129">recipientShiftId</span><span class="sxs-lookup"><span data-stu-id="f7046-129">recipientShiftId</span></span>|<span data-ttu-id="f7046-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7046-130">String</span></span>|<span data-ttu-id="f7046-131">ShiftID do usuário do destinatário com o qual a solicitação deve ser trocada.</span><span class="sxs-lookup"><span data-stu-id="f7046-131">ShiftId for the recipient user with whom the request is to swap.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7046-132">Relações</span><span class="sxs-lookup"><span data-stu-id="f7046-132">Relationships</span></span>

<span data-ttu-id="f7046-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f7046-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7046-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f7046-134">JSON representation</span></span>

<span data-ttu-id="f7046-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f7046-135">The following is a JSON representation of the resource.</span></span>

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
