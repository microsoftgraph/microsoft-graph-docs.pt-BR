---
title: tipo de recurso openShiftChangeRequest
description: Representa um tipo de solicitação de mudança para declarar um turno aberto em um cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 400444ccccc13d103420cc95c522a6ed0aa1afa6
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895569"
---
# <a name="openshiftchangerequest-resource-type"></a><span data-ttu-id="949ed-103">tipo de recurso openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="949ed-103">openShiftChangeRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="949ed-104">Representa um tipo de solicitação de mudança para declarar um [openshift](../resources/openshift.md) em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="949ed-104">Represents a type of shift request to claim an [openshift](../resources/openshift.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="949ed-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="949ed-105">Methods</span></span>

| <span data-ttu-id="949ed-106">Método</span><span class="sxs-lookup"><span data-stu-id="949ed-106">Method</span></span>       | <span data-ttu-id="949ed-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="949ed-107">Return Type</span></span> | <span data-ttu-id="949ed-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="949ed-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="949ed-109">Get</span><span class="sxs-lookup"><span data-stu-id="949ed-109">Get</span></span>](../api/openshiftchangerequest-get.md) | [<span data-ttu-id="949ed-110">openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="949ed-110">openShiftChangeRequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="949ed-111">Leia as propriedades e os relacionamentos de um objeto **openShiftChangeRequest** .</span><span class="sxs-lookup"><span data-stu-id="949ed-111">Read the properties and relationships of an **openShiftChangeRequest** object.</span></span> |
| [<span data-ttu-id="949ed-112">Update</span><span class="sxs-lookup"><span data-stu-id="949ed-112">Update</span></span>](../api/openshiftchangerequest-update.md) | [<span data-ttu-id="949ed-113">openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="949ed-113">openShiftChangeRequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="949ed-114">Atualize um objeto **openShiftChangeRequest** .</span><span class="sxs-lookup"><span data-stu-id="949ed-114">Update an **openShiftChangeRequest** object.</span></span> |
| [<span data-ttu-id="949ed-115">Delete</span><span class="sxs-lookup"><span data-stu-id="949ed-115">Delete</span></span>](../api/openshiftchangerequest-delete.md) | <span data-ttu-id="949ed-116">None</span><span class="sxs-lookup"><span data-stu-id="949ed-116">None</span></span> | <span data-ttu-id="949ed-117">Excluir um objeto **openShiftChangeRequest** .</span><span class="sxs-lookup"><span data-stu-id="949ed-117">Delete an **openShiftChangeRequest** object.</span></span> |
|[<span data-ttu-id="949ed-118">Aprovar</span><span class="sxs-lookup"><span data-stu-id="949ed-118">Approve</span></span>](../api/openshiftchangerequest-approve.md)|<span data-ttu-id="949ed-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="949ed-119">None</span></span>|<span data-ttu-id="949ed-120">Aprovar uma solicitação de alteração de turno aberta.</span><span class="sxs-lookup"><span data-stu-id="949ed-120">Approve an open shift change request.</span></span>|
|[<span data-ttu-id="949ed-121">Aceito</span><span class="sxs-lookup"><span data-stu-id="949ed-121">Decline</span></span>](../api/openshiftchangerequest-decline.md)|<span data-ttu-id="949ed-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="949ed-122">None</span></span>| <span data-ttu-id="949ed-123">Recusar uma solicitação de alteração de turno aberto.</span><span class="sxs-lookup"><span data-stu-id="949ed-123">Decline an open shift change request.</span></span>|

## <a name="properties"></a><span data-ttu-id="949ed-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="949ed-124">Properties</span></span>

| <span data-ttu-id="949ed-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="949ed-125">Property</span></span>     | <span data-ttu-id="949ed-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="949ed-126">Type</span></span>        | <span data-ttu-id="949ed-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="949ed-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="949ed-128">openShiftId</span><span class="sxs-lookup"><span data-stu-id="949ed-128">openShiftId</span></span>|<span data-ttu-id="949ed-129">String</span><span class="sxs-lookup"><span data-stu-id="949ed-129">String</span></span>| <span data-ttu-id="949ed-130">ID para o turno aberto.</span><span class="sxs-lookup"><span data-stu-id="949ed-130">ID for the open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="949ed-131">Relações</span><span class="sxs-lookup"><span data-stu-id="949ed-131">Relationships</span></span>

<span data-ttu-id="949ed-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="949ed-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="949ed-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="949ed-133">JSON representation</span></span>

<span data-ttu-id="949ed-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="949ed-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShiftChangeRequest",
  "baseType": ""
}-->

```json
{
  "openShiftId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShiftChangeRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
