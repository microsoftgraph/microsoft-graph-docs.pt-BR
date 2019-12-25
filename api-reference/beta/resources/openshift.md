---
title: tipo de recurso openShift
description: Representa um turno aberto não atribuído em um cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fa87acd2065a3a56f15016bb7708e73cebe63a31
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870156"
---
# <a name="openshift-resource-type"></a><span data-ttu-id="617b8-103">tipo de recurso openShift</span><span class="sxs-lookup"><span data-stu-id="617b8-103">openShift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="617b8-104">Representa um turno não atribuído e aberto em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="617b8-104">Represents an unassigned, open shift in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="617b8-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="617b8-105">Methods</span></span>

| <span data-ttu-id="617b8-106">Método</span><span class="sxs-lookup"><span data-stu-id="617b8-106">Method</span></span>       | <span data-ttu-id="617b8-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="617b8-107">Return Type</span></span> | <span data-ttu-id="617b8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="617b8-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="617b8-109">Get</span><span class="sxs-lookup"><span data-stu-id="617b8-109">Get</span></span>](../api/openshift-get.md) | [<span data-ttu-id="617b8-110">openShift</span><span class="sxs-lookup"><span data-stu-id="617b8-110">openShift</span></span>](openshift.md) | <span data-ttu-id="617b8-111">Leia as propriedades e os relacionamentos de um objeto **openShift** .</span><span class="sxs-lookup"><span data-stu-id="617b8-111">Read the properties and relationships of an **openShift** object.</span></span> |
| [<span data-ttu-id="617b8-112">Update</span><span class="sxs-lookup"><span data-stu-id="617b8-112">Update</span></span>](../api/openshift-update.md) | [<span data-ttu-id="617b8-113">openShift</span><span class="sxs-lookup"><span data-stu-id="617b8-113">openShift</span></span>](openshift.md) | <span data-ttu-id="617b8-114">Atualize um objeto **openShift** .</span><span class="sxs-lookup"><span data-stu-id="617b8-114">Update an **openShift** object.</span></span> |
| [<span data-ttu-id="617b8-115">Delete</span><span class="sxs-lookup"><span data-stu-id="617b8-115">Delete</span></span>](../api/openshift-delete.md) | <span data-ttu-id="617b8-116">None</span><span class="sxs-lookup"><span data-stu-id="617b8-116">None</span></span> | <span data-ttu-id="617b8-117">Excluir um objeto **openShift** .</span><span class="sxs-lookup"><span data-stu-id="617b8-117">Delete an **openShift** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="617b8-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="617b8-118">Properties</span></span>

| <span data-ttu-id="617b8-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="617b8-119">Property</span></span>     | <span data-ttu-id="617b8-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="617b8-120">Type</span></span>        | <span data-ttu-id="617b8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="617b8-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="617b8-122">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="617b8-122">draftOpenShift</span></span>|[<span data-ttu-id="617b8-123">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="617b8-123">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="617b8-124">Um turno aberto não publicado.</span><span class="sxs-lookup"><span data-stu-id="617b8-124">An unpublished open shift.</span></span>|
|<span data-ttu-id="617b8-125">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="617b8-125">schedulingGroupId</span></span>|<span data-ttu-id="617b8-126">String</span><span class="sxs-lookup"><span data-stu-id="617b8-126">String</span></span>|<span data-ttu-id="617b8-127">ID do grupo de agendamento ao qual o turno aberto pertence.</span><span class="sxs-lookup"><span data-stu-id="617b8-127">ID for the scheduling group that the open shift belongs to.</span></span>|
|<span data-ttu-id="617b8-128">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="617b8-128">sharedOpenShift</span></span>|[<span data-ttu-id="617b8-129">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="617b8-129">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="617b8-130">Um turno aberto publicado.</span><span class="sxs-lookup"><span data-stu-id="617b8-130">A published open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="617b8-131">Relações</span><span class="sxs-lookup"><span data-stu-id="617b8-131">Relationships</span></span>

<span data-ttu-id="617b8-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="617b8-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="617b8-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="617b8-133">JSON representation</span></span>

<span data-ttu-id="617b8-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="617b8-134">The following is a JSON representation of the resource.</span></span>

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
