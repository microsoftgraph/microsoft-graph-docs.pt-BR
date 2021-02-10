---
title: Tipo de recurso swapShiftsChangeRequest
description: Representa o tipo de solicitação de turno para trocar de turno com outro usuário na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5f5d1bb7a520d5d7f64640725a846ef5bc76a0b2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154730"
---
# <a name="swapshiftschangerequest-resource-type"></a><span data-ttu-id="f7071-103">Tipo de recurso swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="f7071-103">swapShiftsChangeRequest resource type</span></span>

<span data-ttu-id="f7071-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7071-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f7071-105">Representa um tipo de solicitação de turno para trocar uma [mudança](../resources/shift.md) com outro usuário na [equipe.](../resources/team.md)</span><span class="sxs-lookup"><span data-stu-id="f7071-105">Represents a type of shift request to swap a [shift](../resources/shift.md) with another user in the [team](../resources/team.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f7071-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f7071-106">Methods</span></span>

| <span data-ttu-id="f7071-107">Método</span><span class="sxs-lookup"><span data-stu-id="f7071-107">Method</span></span>       | <span data-ttu-id="f7071-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f7071-108">Return Type</span></span> | <span data-ttu-id="f7071-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7071-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f7071-110">List</span><span class="sxs-lookup"><span data-stu-id="f7071-110">List</span></span>](../api/swapshiftschangerequest-list.md) | <span data-ttu-id="f7071-111">Coleção de [swapShiftsChangeRequest](swapshiftschangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="f7071-111">Collection of [swapShiftsChangeRequest](swapshiftschangerequest.md)</span></span> | <span data-ttu-id="f7071-112">Listar as propriedades e os relacionamentos dos **objetos swapShiftsChangeRequest** em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="f7071-112">List the properties and relationships of **swapShiftsChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="f7071-113">Criar</span><span class="sxs-lookup"><span data-stu-id="f7071-113">Create</span></span>](../api/swapshiftschangerequest-post.md) | [<span data-ttu-id="f7071-114">swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="f7071-114">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="f7071-115">Crie uma instância de um **objeto swapShiftsChangeRequest.**</span><span class="sxs-lookup"><span data-stu-id="f7071-115">Create an instance of a **swapShiftsChangeRequest** object.</span></span> |
| [<span data-ttu-id="f7071-116">Get</span><span class="sxs-lookup"><span data-stu-id="f7071-116">Get</span></span>](../api/swapshiftschangerequest-get.md) | [<span data-ttu-id="f7071-117">swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="f7071-117">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="f7071-118">Leia as propriedades e os relacionamentos de um **objeto swapShiftsChangeRequest.**</span><span class="sxs-lookup"><span data-stu-id="f7071-118">Read the properties and relationships of a **swapShiftsChangeRequest** object.</span></span> |
|[<span data-ttu-id="f7071-119">Aprovar</span><span class="sxs-lookup"><span data-stu-id="f7071-119">Approve</span></span>](../api/swapshiftschangerequest-approve.md)|<span data-ttu-id="f7071-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f7071-120">None</span></span>|<span data-ttu-id="f7071-121">Aprovar um **swapShiftsChangeRequest**.</span><span class="sxs-lookup"><span data-stu-id="f7071-121">Approve a **swapShiftsChangeRequest**.</span></span> |
|[<span data-ttu-id="f7071-122">Recusar</span><span class="sxs-lookup"><span data-stu-id="f7071-122">Decline</span></span>](../api/swapshiftschangerequest-decline.md)|<span data-ttu-id="f7071-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f7071-123">None</span></span>|<span data-ttu-id="f7071-124">Recusar um **swapShiftsChangeRequest**.</span><span class="sxs-lookup"><span data-stu-id="f7071-124">Decline a **swapShiftsChangeRequest**.</span></span>|

## <a name="properties"></a><span data-ttu-id="f7071-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f7071-125">Properties</span></span>

| <span data-ttu-id="f7071-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7071-126">Property</span></span>     | <span data-ttu-id="f7071-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7071-127">Type</span></span>        | <span data-ttu-id="f7071-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7071-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f7071-129">recipientShiftId</span><span class="sxs-lookup"><span data-stu-id="f7071-129">recipientShiftId</span></span>|<span data-ttu-id="f7071-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7071-130">String</span></span>|<span data-ttu-id="f7071-131">ShiftId para o usuário do destinatário com o qual a solicitação deve ser trocada.</span><span class="sxs-lookup"><span data-stu-id="f7071-131">ShiftId for the recipient user with whom the request is to swap.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7071-132">Relações</span><span class="sxs-lookup"><span data-stu-id="f7071-132">Relationships</span></span>

<span data-ttu-id="f7071-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f7071-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7071-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f7071-134">JSON representation</span></span>

<span data-ttu-id="f7071-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f7071-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
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

