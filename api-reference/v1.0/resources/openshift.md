---
title: tipo de recurso openShift
description: Representa um turno aberto não atribuído em um cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4a1a616cee4f61a93f8b3db379a0e5f39afc5f22
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003028"
---
# <a name="openshift-resource-type"></a><span data-ttu-id="37aab-103">tipo de recurso openShift</span><span class="sxs-lookup"><span data-stu-id="37aab-103">openShift resource type</span></span>

<span data-ttu-id="37aab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37aab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37aab-105">Representa um turno não atribuído e aberto em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="37aab-105">Represents an unassigned, open shift in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="37aab-106">Methods</span><span class="sxs-lookup"><span data-stu-id="37aab-106">Methods</span></span>

| <span data-ttu-id="37aab-107">Método</span><span class="sxs-lookup"><span data-stu-id="37aab-107">Method</span></span>       | <span data-ttu-id="37aab-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="37aab-108">Return Type</span></span> | <span data-ttu-id="37aab-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="37aab-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="37aab-110">List</span><span class="sxs-lookup"><span data-stu-id="37aab-110">List</span></span>](../api/openshift-list.md) | <span data-ttu-id="37aab-111">Coleção de [openShift](openshift.md)</span><span class="sxs-lookup"><span data-stu-id="37aab-111">Collection of [openShift](openshift.md)</span></span> | <span data-ttu-id="37aab-112">Listar as propriedades e os relacionamentos dos objetos **openShift** em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="37aab-112">List the properties and relationships of **openShift** objects in a team.</span></span>|
| [<span data-ttu-id="37aab-113">Create</span><span class="sxs-lookup"><span data-stu-id="37aab-113">Create</span></span>](../api/openshift-post.md) | [<span data-ttu-id="37aab-114">openShift</span><span class="sxs-lookup"><span data-stu-id="37aab-114">openShift</span></span>](openshift.md) | <span data-ttu-id="37aab-115">Criar uma instância de um objeto **openShift** .</span><span class="sxs-lookup"><span data-stu-id="37aab-115">Create an instance of an **openShift** object.</span></span> |
| [<span data-ttu-id="37aab-116">Get</span><span class="sxs-lookup"><span data-stu-id="37aab-116">Get</span></span>](../api/openshift-get.md) | [<span data-ttu-id="37aab-117">openShift</span><span class="sxs-lookup"><span data-stu-id="37aab-117">openShift</span></span>](openshift.md) | <span data-ttu-id="37aab-118">Leia as propriedades e os relacionamentos de um objeto **openShift** .</span><span class="sxs-lookup"><span data-stu-id="37aab-118">Read the properties and relationships of an **openShift** object.</span></span> |
| [<span data-ttu-id="37aab-119">Atualização</span><span class="sxs-lookup"><span data-stu-id="37aab-119">Update</span></span>](../api/openshift-update.md) | [<span data-ttu-id="37aab-120">openShift</span><span class="sxs-lookup"><span data-stu-id="37aab-120">openShift</span></span>](openshift.md) | <span data-ttu-id="37aab-121">Atualize um objeto **openShift** .</span><span class="sxs-lookup"><span data-stu-id="37aab-121">Update an **openShift** object.</span></span> |
| [<span data-ttu-id="37aab-122">Delete</span><span class="sxs-lookup"><span data-stu-id="37aab-122">Delete</span></span>](../api/openshift-delete.md) | <span data-ttu-id="37aab-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="37aab-123">None</span></span> | <span data-ttu-id="37aab-124">Excluir um objeto **openShift** .</span><span class="sxs-lookup"><span data-stu-id="37aab-124">Delete an **openShift** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="37aab-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37aab-125">Properties</span></span>

| <span data-ttu-id="37aab-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37aab-126">Property</span></span>     | <span data-ttu-id="37aab-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="37aab-127">Type</span></span>        | <span data-ttu-id="37aab-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="37aab-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="37aab-129">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="37aab-129">draftOpenShift</span></span>|[<span data-ttu-id="37aab-130">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="37aab-130">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="37aab-131">Um turno aberto não publicado.</span><span class="sxs-lookup"><span data-stu-id="37aab-131">An unpublished open shift.</span></span>|
|<span data-ttu-id="37aab-132">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="37aab-132">schedulingGroupId</span></span>|<span data-ttu-id="37aab-133">String</span><span class="sxs-lookup"><span data-stu-id="37aab-133">String</span></span>|<span data-ttu-id="37aab-134">ID do grupo de agendamento ao qual o turno aberto pertence.</span><span class="sxs-lookup"><span data-stu-id="37aab-134">ID for the scheduling group that the open shift belongs to.</span></span>|
|<span data-ttu-id="37aab-135">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="37aab-135">sharedOpenShift</span></span>|[<span data-ttu-id="37aab-136">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="37aab-136">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="37aab-137">Um turno aberto publicado.</span><span class="sxs-lookup"><span data-stu-id="37aab-137">A published open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37aab-138">Relações</span><span class="sxs-lookup"><span data-stu-id="37aab-138">Relationships</span></span>

<span data-ttu-id="37aab-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="37aab-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="37aab-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37aab-140">JSON representation</span></span>

<span data-ttu-id="37aab-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37aab-141">The following is a JSON representation of the resource.</span></span>

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

