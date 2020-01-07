---
title: tipo de recurso openShift
description: Representa um turno aberto não atribuído em um cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f3ce94c12328e9c05f899c5d2176339bbed93432
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951934"
---
# <a name="openshift-resource-type"></a><span data-ttu-id="a20df-103">tipo de recurso openShift</span><span class="sxs-lookup"><span data-stu-id="a20df-103">openShift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a20df-104">Representa um turno não atribuído e aberto em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="a20df-104">Represents an unassigned, open shift in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a20df-105">Methods</span><span class="sxs-lookup"><span data-stu-id="a20df-105">Methods</span></span>

| <span data-ttu-id="a20df-106">Método</span><span class="sxs-lookup"><span data-stu-id="a20df-106">Method</span></span>       | <span data-ttu-id="a20df-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a20df-107">Return Type</span></span> | <span data-ttu-id="a20df-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a20df-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a20df-109">Criar</span><span class="sxs-lookup"><span data-stu-id="a20df-109">Create</span></span>](../api/openshift-post.md) | [<span data-ttu-id="a20df-110">openShift</span><span class="sxs-lookup"><span data-stu-id="a20df-110">openShift</span></span>](openshift.md) | <span data-ttu-id="a20df-111">Criar uma instância de um objeto **openShift** .</span><span class="sxs-lookup"><span data-stu-id="a20df-111">Create an instance of an **openShift** object.</span></span> |
| [<span data-ttu-id="a20df-112">List</span><span class="sxs-lookup"><span data-stu-id="a20df-112">List</span></span>](../api/openshift-list.md) | <span data-ttu-id="a20df-113">Coleção de [openShift](openshift.md)</span><span class="sxs-lookup"><span data-stu-id="a20df-113">Collection of [openShift](openshift.md)</span></span> | <span data-ttu-id="a20df-114">Listar as propriedades e os relacionamentos dos objetos **openShift** em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="a20df-114">List the properties and relationships of **openShift** objects in a team.</span></span>|
| [<span data-ttu-id="a20df-115">Get</span><span class="sxs-lookup"><span data-stu-id="a20df-115">Get</span></span>](../api/openshift-get.md) | [<span data-ttu-id="a20df-116">openShift</span><span class="sxs-lookup"><span data-stu-id="a20df-116">openShift</span></span>](openshift.md) | <span data-ttu-id="a20df-117">Leia as propriedades e os relacionamentos de um objeto **openShift** .</span><span class="sxs-lookup"><span data-stu-id="a20df-117">Read the properties and relationships of an **openShift** object.</span></span> |
| [<span data-ttu-id="a20df-118">Update</span><span class="sxs-lookup"><span data-stu-id="a20df-118">Update</span></span>](../api/openshift-update.md) | [<span data-ttu-id="a20df-119">openShift</span><span class="sxs-lookup"><span data-stu-id="a20df-119">openShift</span></span>](openshift.md) | <span data-ttu-id="a20df-120">Atualize um objeto **openShift** .</span><span class="sxs-lookup"><span data-stu-id="a20df-120">Update an **openShift** object.</span></span> |
| [<span data-ttu-id="a20df-121">Delete</span><span class="sxs-lookup"><span data-stu-id="a20df-121">Delete</span></span>](../api/openshift-delete.md) | <span data-ttu-id="a20df-122">None</span><span class="sxs-lookup"><span data-stu-id="a20df-122">None</span></span> | <span data-ttu-id="a20df-123">Excluir um objeto **openShift** .</span><span class="sxs-lookup"><span data-stu-id="a20df-123">Delete an **openShift** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a20df-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a20df-124">Properties</span></span>

| <span data-ttu-id="a20df-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a20df-125">Property</span></span>     | <span data-ttu-id="a20df-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a20df-126">Type</span></span>        | <span data-ttu-id="a20df-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a20df-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a20df-128">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="a20df-128">draftOpenShift</span></span>|[<span data-ttu-id="a20df-129">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="a20df-129">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="a20df-130">Um turno aberto não publicado.</span><span class="sxs-lookup"><span data-stu-id="a20df-130">An unpublished open shift.</span></span>|
|<span data-ttu-id="a20df-131">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="a20df-131">schedulingGroupId</span></span>|<span data-ttu-id="a20df-132">String</span><span class="sxs-lookup"><span data-stu-id="a20df-132">String</span></span>|<span data-ttu-id="a20df-133">ID do grupo de agendamento ao qual o turno aberto pertence.</span><span class="sxs-lookup"><span data-stu-id="a20df-133">ID for the scheduling group that the open shift belongs to.</span></span>|
|<span data-ttu-id="a20df-134">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="a20df-134">sharedOpenShift</span></span>|[<span data-ttu-id="a20df-135">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="a20df-135">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="a20df-136">Um turno aberto publicado.</span><span class="sxs-lookup"><span data-stu-id="a20df-136">A published open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a20df-137">Relações</span><span class="sxs-lookup"><span data-stu-id="a20df-137">Relationships</span></span>

<span data-ttu-id="a20df-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a20df-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a20df-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a20df-139">JSON representation</span></span>

<span data-ttu-id="a20df-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a20df-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShift",
  "baseType": ""
}-->

```json
{
  "draftOpenShift": {"@odata.type": "microsoft.graph.openShiftItem"},
  "schedulingGroupId": "String",
  "sharedOpenShift": {"@odata.type": "microsoft.graph.openShiftItem"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShift resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
