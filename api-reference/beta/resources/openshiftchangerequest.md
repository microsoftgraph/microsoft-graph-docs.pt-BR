---
title: Tipo de recurso openShiftChangeRequest
description: Representa um tipo de solicitação de turno para reivindicar um turno aberto em um cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e141dcb6657c9efc7d751b1713aa8b53d79c9264
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161415"
---
# <a name="openshiftchangerequest-resource-type"></a><span data-ttu-id="2ac23-103">Tipo de recurso openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="2ac23-103">openShiftChangeRequest resource type</span></span>

<span data-ttu-id="2ac23-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ac23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ac23-105">Representa um tipo de solicitação de turno para [reivindicar uma abertura](../resources/openshift.md) em um [cronograma.](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="2ac23-105">Represents a type of shift request to claim an [openshift](../resources/openshift.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2ac23-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="2ac23-106">Methods</span></span>

| <span data-ttu-id="2ac23-107">Método</span><span class="sxs-lookup"><span data-stu-id="2ac23-107">Method</span></span>       | <span data-ttu-id="2ac23-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2ac23-108">Return Type</span></span> | <span data-ttu-id="2ac23-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ac23-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2ac23-110">Criar</span><span class="sxs-lookup"><span data-stu-id="2ac23-110">Create</span></span>](../api/openshiftchangerequest-post.md) | [<span data-ttu-id="2ac23-111">openshiftchangerequest</span><span class="sxs-lookup"><span data-stu-id="2ac23-111">openshiftchangerequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="2ac23-112">Crie uma instância de um objeto openshiftchangerequest.</span><span class="sxs-lookup"><span data-stu-id="2ac23-112">Create an instance of an openshiftchangerequest object.</span></span> |
| [<span data-ttu-id="2ac23-113">Lista</span><span class="sxs-lookup"><span data-stu-id="2ac23-113">List</span></span>](../api/openshiftchangerequest-list.md) | <span data-ttu-id="2ac23-114">Coleção de [openshiftchangerequest](openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="2ac23-114">Collection of [openshiftchangerequest](openshiftchangerequest.md)</span></span> | <span data-ttu-id="2ac23-115">Listar as propriedades e os relacionamentos dos **objetos openShiftChangeRequest** em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="2ac23-115">List the properties and relationships of **openShiftChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="2ac23-116">Get</span><span class="sxs-lookup"><span data-stu-id="2ac23-116">Get</span></span>](../api/openshiftchangerequest-get.md) | [<span data-ttu-id="2ac23-117">openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="2ac23-117">openShiftChangeRequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="2ac23-118">Leia as propriedades e os relacionamentos de um **objeto openShiftChangeRequest.**</span><span class="sxs-lookup"><span data-stu-id="2ac23-118">Read the properties and relationships of an **openShiftChangeRequest** object.</span></span> |
|[<span data-ttu-id="2ac23-119">Aprovar</span><span class="sxs-lookup"><span data-stu-id="2ac23-119">Approve</span></span>](../api/openshiftchangerequest-approve.md)|<span data-ttu-id="2ac23-120">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="2ac23-120">None</span></span>|<span data-ttu-id="2ac23-121">Aprovar uma solicitação de alteração de turno aberto.</span><span class="sxs-lookup"><span data-stu-id="2ac23-121">Approve an open shift change request.</span></span>|
|[<span data-ttu-id="2ac23-122">Recusar</span><span class="sxs-lookup"><span data-stu-id="2ac23-122">Decline</span></span>](../api/openshiftchangerequest-decline.md)|<span data-ttu-id="2ac23-123">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="2ac23-123">None</span></span>| <span data-ttu-id="2ac23-124">Recusar uma solicitação de alteração de turno aberto.</span><span class="sxs-lookup"><span data-stu-id="2ac23-124">Decline an open shift change request.</span></span>|

## <a name="properties"></a><span data-ttu-id="2ac23-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ac23-125">Properties</span></span>

| <span data-ttu-id="2ac23-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ac23-126">Property</span></span>     | <span data-ttu-id="2ac23-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ac23-127">Type</span></span>        | <span data-ttu-id="2ac23-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ac23-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2ac23-129">openShiftId</span><span class="sxs-lookup"><span data-stu-id="2ac23-129">openShiftId</span></span>|<span data-ttu-id="2ac23-130">String</span><span class="sxs-lookup"><span data-stu-id="2ac23-130">String</span></span>| <span data-ttu-id="2ac23-131">ID do turno aberto.</span><span class="sxs-lookup"><span data-stu-id="2ac23-131">ID for the open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ac23-132">Relações</span><span class="sxs-lookup"><span data-stu-id="2ac23-132">Relationships</span></span>

<span data-ttu-id="2ac23-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ac23-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ac23-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ac23-134">JSON representation</span></span>

<span data-ttu-id="2ac23-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ac23-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShiftChangeRequest"
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


