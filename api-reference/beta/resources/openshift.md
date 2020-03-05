---
title: tipo de recurso openShift
description: Representa um turno aberto não atribuído em um cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e544f54c7fbf015ed1050ab23d76217b311bdeaf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522190"
---
# <a name="openshift-resource-type"></a><span data-ttu-id="617ce-103">tipo de recurso openShift</span><span class="sxs-lookup"><span data-stu-id="617ce-103">openShift resource type</span></span>

<span data-ttu-id="617ce-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="617ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="617ce-105">Representa um turno não atribuído e aberto em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="617ce-105">Represents an unassigned, open shift in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="617ce-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="617ce-106">Methods</span></span>

| <span data-ttu-id="617ce-107">Método</span><span class="sxs-lookup"><span data-stu-id="617ce-107">Method</span></span>       | <span data-ttu-id="617ce-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="617ce-108">Return Type</span></span> | <span data-ttu-id="617ce-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="617ce-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="617ce-110">Criar</span><span class="sxs-lookup"><span data-stu-id="617ce-110">Create</span></span>](../api/openshift-post.md) | [<span data-ttu-id="617ce-111">openShift</span><span class="sxs-lookup"><span data-stu-id="617ce-111">openShift</span></span>](openshift.md) | <span data-ttu-id="617ce-112">Criar uma instância de um objeto **openShift** .</span><span class="sxs-lookup"><span data-stu-id="617ce-112">Create an instance of an **openShift** object.</span></span> |
| [<span data-ttu-id="617ce-113">List</span><span class="sxs-lookup"><span data-stu-id="617ce-113">List</span></span>](../api/openshift-list.md) | <span data-ttu-id="617ce-114">Coleção de [openShift](openshift.md)</span><span class="sxs-lookup"><span data-stu-id="617ce-114">Collection of [openShift](openshift.md)</span></span> | <span data-ttu-id="617ce-115">Listar as propriedades e os relacionamentos dos objetos **openShift** em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="617ce-115">List the properties and relationships of **openShift** objects in a team.</span></span>|
| [<span data-ttu-id="617ce-116">Get</span><span class="sxs-lookup"><span data-stu-id="617ce-116">Get</span></span>](../api/openshift-get.md) | [<span data-ttu-id="617ce-117">openShift</span><span class="sxs-lookup"><span data-stu-id="617ce-117">openShift</span></span>](openshift.md) | <span data-ttu-id="617ce-118">Leia as propriedades e os relacionamentos de um objeto **openShift** .</span><span class="sxs-lookup"><span data-stu-id="617ce-118">Read the properties and relationships of an **openShift** object.</span></span> |
| [<span data-ttu-id="617ce-119">Update</span><span class="sxs-lookup"><span data-stu-id="617ce-119">Update</span></span>](../api/openshift-update.md) | [<span data-ttu-id="617ce-120">openShift</span><span class="sxs-lookup"><span data-stu-id="617ce-120">openShift</span></span>](openshift.md) | <span data-ttu-id="617ce-121">Atualize um objeto **openShift** .</span><span class="sxs-lookup"><span data-stu-id="617ce-121">Update an **openShift** object.</span></span> |
| [<span data-ttu-id="617ce-122">Delete</span><span class="sxs-lookup"><span data-stu-id="617ce-122">Delete</span></span>](../api/openshift-delete.md) | <span data-ttu-id="617ce-123">None</span><span class="sxs-lookup"><span data-stu-id="617ce-123">None</span></span> | <span data-ttu-id="617ce-124">Excluir um objeto **openShift** .</span><span class="sxs-lookup"><span data-stu-id="617ce-124">Delete an **openShift** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="617ce-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="617ce-125">Properties</span></span>

| <span data-ttu-id="617ce-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="617ce-126">Property</span></span>     | <span data-ttu-id="617ce-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="617ce-127">Type</span></span>        | <span data-ttu-id="617ce-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="617ce-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="617ce-129">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="617ce-129">draftOpenShift</span></span>|[<span data-ttu-id="617ce-130">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="617ce-130">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="617ce-131">Um turno aberto não publicado.</span><span class="sxs-lookup"><span data-stu-id="617ce-131">An unpublished open shift.</span></span>|
|<span data-ttu-id="617ce-132">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="617ce-132">schedulingGroupId</span></span>|<span data-ttu-id="617ce-133">String</span><span class="sxs-lookup"><span data-stu-id="617ce-133">String</span></span>|<span data-ttu-id="617ce-134">ID do grupo de agendamento ao qual o turno aberto pertence.</span><span class="sxs-lookup"><span data-stu-id="617ce-134">ID for the scheduling group that the open shift belongs to.</span></span>|
|<span data-ttu-id="617ce-135">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="617ce-135">sharedOpenShift</span></span>|[<span data-ttu-id="617ce-136">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="617ce-136">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="617ce-137">Um turno aberto publicado.</span><span class="sxs-lookup"><span data-stu-id="617ce-137">A published open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="617ce-138">Relações</span><span class="sxs-lookup"><span data-stu-id="617ce-138">Relationships</span></span>

<span data-ttu-id="617ce-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="617ce-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="617ce-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="617ce-140">JSON representation</span></span>

<span data-ttu-id="617ce-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="617ce-141">The following is a JSON representation of the resource.</span></span>

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
