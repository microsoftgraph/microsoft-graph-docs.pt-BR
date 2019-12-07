---
title: tipo de recurso openShift
description: Representa um turno aberto não atribuído em um cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3eff83475c4a36ec1c294c62b9e1b87673926d8d
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895570"
---
# <a name="openshift-resource-type"></a><span data-ttu-id="eb844-103">tipo de recurso openShift</span><span class="sxs-lookup"><span data-stu-id="eb844-103">openShift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb844-104">Representa um turno não atribuído e aberto em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="eb844-104">Represents an unassigned, open shift in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="eb844-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="eb844-105">Methods</span></span>

| <span data-ttu-id="eb844-106">Método</span><span class="sxs-lookup"><span data-stu-id="eb844-106">Method</span></span>       | <span data-ttu-id="eb844-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eb844-107">Return Type</span></span> | <span data-ttu-id="eb844-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb844-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="eb844-109">Get</span><span class="sxs-lookup"><span data-stu-id="eb844-109">Get</span></span>](../api/openshift-get.md) | [<span data-ttu-id="eb844-110">openShift</span><span class="sxs-lookup"><span data-stu-id="eb844-110">openShift</span></span>](openshift.md) | <span data-ttu-id="eb844-111">Leia as propriedades e os relacionamentos do objeto openShift.</span><span class="sxs-lookup"><span data-stu-id="eb844-111">Read properties and relationships of openShift object.</span></span> |
| [<span data-ttu-id="eb844-112">Update</span><span class="sxs-lookup"><span data-stu-id="eb844-112">Update</span></span>](../api/openshift-update.md) | [<span data-ttu-id="eb844-113">openShift</span><span class="sxs-lookup"><span data-stu-id="eb844-113">openShift</span></span>](openshift.md) | <span data-ttu-id="eb844-114">Atualize o objeto openShift.</span><span class="sxs-lookup"><span data-stu-id="eb844-114">Update openShift object.</span></span> |
| [<span data-ttu-id="eb844-115">Delete</span><span class="sxs-lookup"><span data-stu-id="eb844-115">Delete</span></span>](../api/openshift-delete.md) | <span data-ttu-id="eb844-116">None</span><span class="sxs-lookup"><span data-stu-id="eb844-116">None</span></span> | <span data-ttu-id="eb844-117">Exclua o objeto openShift.</span><span class="sxs-lookup"><span data-stu-id="eb844-117">Delete openShift object.</span></span> |

## <a name="properties"></a><span data-ttu-id="eb844-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb844-118">Properties</span></span>

| <span data-ttu-id="eb844-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb844-119">Property</span></span>     | <span data-ttu-id="eb844-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb844-120">Type</span></span>        | <span data-ttu-id="eb844-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb844-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eb844-122">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="eb844-122">draftOpenShift</span></span>|[<span data-ttu-id="eb844-123">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="eb844-123">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="eb844-124">Um turno aberto não publicado.</span><span class="sxs-lookup"><span data-stu-id="eb844-124">An unpublished open shift.</span></span>|
|<span data-ttu-id="eb844-125">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="eb844-125">schedulingGroupId</span></span>|<span data-ttu-id="eb844-126">String</span><span class="sxs-lookup"><span data-stu-id="eb844-126">String</span></span>|<span data-ttu-id="eb844-127">ID do grupo de agendamento ao qual o turno aberto pertence.</span><span class="sxs-lookup"><span data-stu-id="eb844-127">ID for the scheduling group that the open shift belongs to.</span></span>|
|<span data-ttu-id="eb844-128">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="eb844-128">sharedOpenShift</span></span>|[<span data-ttu-id="eb844-129">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="eb844-129">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="eb844-130">Um turno aberto publicado.</span><span class="sxs-lookup"><span data-stu-id="eb844-130">A published open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb844-131">Relações</span><span class="sxs-lookup"><span data-stu-id="eb844-131">Relationships</span></span>

<span data-ttu-id="eb844-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb844-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb844-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb844-133">JSON representation</span></span>

<span data-ttu-id="eb844-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb844-134">The following is a JSON representation of the resource.</span></span>

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
