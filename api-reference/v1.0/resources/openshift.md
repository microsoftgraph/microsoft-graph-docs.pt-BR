---
title: tipo de recurso openShift
description: Representa um turno aberto não atribuído em um cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2051dddb78121341d22dc9e3cd20b13178cb81c9
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154988"
---
# <a name="openshift-resource-type"></a><span data-ttu-id="947a6-103">tipo de recurso openShift</span><span class="sxs-lookup"><span data-stu-id="947a6-103">openShift resource type</span></span>

<span data-ttu-id="947a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="947a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="947a6-105">Representa um turno não atribuído e aberto em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="947a6-105">Represents an unassigned, open shift in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="947a6-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="947a6-106">Methods</span></span>

| <span data-ttu-id="947a6-107">Método</span><span class="sxs-lookup"><span data-stu-id="947a6-107">Method</span></span>       | <span data-ttu-id="947a6-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="947a6-108">Return Type</span></span> | <span data-ttu-id="947a6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="947a6-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="947a6-110">List</span><span class="sxs-lookup"><span data-stu-id="947a6-110">List</span></span>](../api/openshift-list.md) | <span data-ttu-id="947a6-111">Coleção de [openShift](openshift.md)</span><span class="sxs-lookup"><span data-stu-id="947a6-111">Collection of [openShift](openshift.md)</span></span> | <span data-ttu-id="947a6-112">Listar as propriedades e os relacionamentos dos objetos **openShift** em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="947a6-112">List the properties and relationships of **openShift** objects in a team.</span></span>|
| [<span data-ttu-id="947a6-113">Create</span><span class="sxs-lookup"><span data-stu-id="947a6-113">Create</span></span>](../api/openshift-post.md) | [<span data-ttu-id="947a6-114">openShift</span><span class="sxs-lookup"><span data-stu-id="947a6-114">openShift</span></span>](openshift.md) | <span data-ttu-id="947a6-115">Criar uma instância de um objeto **openShift** .</span><span class="sxs-lookup"><span data-stu-id="947a6-115">Create an instance of an **openShift** object.</span></span> |
| [<span data-ttu-id="947a6-116">Get</span><span class="sxs-lookup"><span data-stu-id="947a6-116">Get</span></span>](../api/openshift-get.md) | [<span data-ttu-id="947a6-117">openShift</span><span class="sxs-lookup"><span data-stu-id="947a6-117">openShift</span></span>](openshift.md) | <span data-ttu-id="947a6-118">Leia as propriedades e os relacionamentos de um objeto **openShift** .</span><span class="sxs-lookup"><span data-stu-id="947a6-118">Read the properties and relationships of an **openShift** object.</span></span> |
| [<span data-ttu-id="947a6-119">Update</span><span class="sxs-lookup"><span data-stu-id="947a6-119">Update</span></span>](../api/openshift-update.md) | [<span data-ttu-id="947a6-120">openShift</span><span class="sxs-lookup"><span data-stu-id="947a6-120">openShift</span></span>](openshift.md) | <span data-ttu-id="947a6-121">Atualize um objeto **openShift** .</span><span class="sxs-lookup"><span data-stu-id="947a6-121">Update an **openShift** object.</span></span> |
| [<span data-ttu-id="947a6-122">Delete</span><span class="sxs-lookup"><span data-stu-id="947a6-122">Delete</span></span>](../api/openshift-delete.md) | <span data-ttu-id="947a6-123">None</span><span class="sxs-lookup"><span data-stu-id="947a6-123">None</span></span> | <span data-ttu-id="947a6-124">Excluir um objeto **openShift** .</span><span class="sxs-lookup"><span data-stu-id="947a6-124">Delete an **openShift** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="947a6-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="947a6-125">Properties</span></span>

| <span data-ttu-id="947a6-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="947a6-126">Property</span></span>     | <span data-ttu-id="947a6-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="947a6-127">Type</span></span>        | <span data-ttu-id="947a6-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="947a6-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="947a6-129">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="947a6-129">draftOpenShift</span></span>|[<span data-ttu-id="947a6-130">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="947a6-130">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="947a6-131">Um turno aberto não publicado.</span><span class="sxs-lookup"><span data-stu-id="947a6-131">An unpublished open shift.</span></span>|
|<span data-ttu-id="947a6-132">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="947a6-132">schedulingGroupId</span></span>|<span data-ttu-id="947a6-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="947a6-133">String</span></span>|<span data-ttu-id="947a6-134">ID do grupo de agendamento ao qual o turno aberto pertence.</span><span class="sxs-lookup"><span data-stu-id="947a6-134">ID for the scheduling group that the open shift belongs to.</span></span>|
|<span data-ttu-id="947a6-135">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="947a6-135">sharedOpenShift</span></span>|[<span data-ttu-id="947a6-136">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="947a6-136">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="947a6-137">Um turno aberto publicado.</span><span class="sxs-lookup"><span data-stu-id="947a6-137">A published open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="947a6-138">Relações</span><span class="sxs-lookup"><span data-stu-id="947a6-138">Relationships</span></span>

<span data-ttu-id="947a6-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="947a6-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="947a6-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="947a6-140">JSON representation</span></span>

<span data-ttu-id="947a6-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="947a6-141">The following is a JSON representation of the resource.</span></span>

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
