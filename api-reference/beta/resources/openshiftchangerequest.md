---
title: tipo de recurso openShiftChangeRequest
description: Representa um tipo de solicitação de mudança para declarar um turno aberto em um cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 69663b876e98bfe9f5c633890d02a6abd3b72f32
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951927"
---
# <a name="openshiftchangerequest-resource-type"></a><span data-ttu-id="670bb-103">tipo de recurso openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="670bb-103">openShiftChangeRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="670bb-104">Representa um tipo de solicitação de mudança para declarar um [openshift](../resources/openshift.md) em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="670bb-104">Represents a type of shift request to claim an [openshift](../resources/openshift.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="670bb-105">Methods</span><span class="sxs-lookup"><span data-stu-id="670bb-105">Methods</span></span>

| <span data-ttu-id="670bb-106">Método</span><span class="sxs-lookup"><span data-stu-id="670bb-106">Method</span></span>       | <span data-ttu-id="670bb-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="670bb-107">Return Type</span></span> | <span data-ttu-id="670bb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="670bb-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="670bb-109">Criar</span><span class="sxs-lookup"><span data-stu-id="670bb-109">Create</span></span>](../api/openshiftchangerequest-post.md) | [<span data-ttu-id="670bb-110">openshiftchangerequest</span><span class="sxs-lookup"><span data-stu-id="670bb-110">openshiftchangerequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="670bb-111">Criar uma instância de um objeto openshiftchangerequest.</span><span class="sxs-lookup"><span data-stu-id="670bb-111">Create an instance of an openshiftchangerequest object.</span></span> |
| [<span data-ttu-id="670bb-112">List</span><span class="sxs-lookup"><span data-stu-id="670bb-112">List</span></span>](../api/openshiftchangerequest-list.md) | <span data-ttu-id="670bb-113">Coleção de [openshiftchangerequest](openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="670bb-113">Collection of [openshiftchangerequest](openshiftchangerequest.md)</span></span> | <span data-ttu-id="670bb-114">Listar as propriedades e os relacionamentos dos objetos **openShiftChangeRequest** em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="670bb-114">List the properties and relationships of **openShiftChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="670bb-115">Get</span><span class="sxs-lookup"><span data-stu-id="670bb-115">Get</span></span>](../api/openshiftchangerequest-get.md) | [<span data-ttu-id="670bb-116">openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="670bb-116">openShiftChangeRequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="670bb-117">Leia as propriedades e os relacionamentos de um objeto **openShiftChangeRequest** .</span><span class="sxs-lookup"><span data-stu-id="670bb-117">Read the properties and relationships of an **openShiftChangeRequest** object.</span></span> |
|[<span data-ttu-id="670bb-118">Aprovar</span><span class="sxs-lookup"><span data-stu-id="670bb-118">Approve</span></span>](../api/openshiftchangerequest-approve.md)|<span data-ttu-id="670bb-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="670bb-119">None</span></span>|<span data-ttu-id="670bb-120">Aprovar uma solicitação de alteração de turno aberta.</span><span class="sxs-lookup"><span data-stu-id="670bb-120">Approve an open shift change request.</span></span>|
|[<span data-ttu-id="670bb-121">Aceito</span><span class="sxs-lookup"><span data-stu-id="670bb-121">Decline</span></span>](../api/openshiftchangerequest-decline.md)|<span data-ttu-id="670bb-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="670bb-122">None</span></span>| <span data-ttu-id="670bb-123">Recusar uma solicitação de alteração de turno aberto.</span><span class="sxs-lookup"><span data-stu-id="670bb-123">Decline an open shift change request.</span></span>|

## <a name="properties"></a><span data-ttu-id="670bb-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="670bb-124">Properties</span></span>

| <span data-ttu-id="670bb-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="670bb-125">Property</span></span>     | <span data-ttu-id="670bb-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="670bb-126">Type</span></span>        | <span data-ttu-id="670bb-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="670bb-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="670bb-128">openShiftId</span><span class="sxs-lookup"><span data-stu-id="670bb-128">openShiftId</span></span>|<span data-ttu-id="670bb-129">String</span><span class="sxs-lookup"><span data-stu-id="670bb-129">String</span></span>| <span data-ttu-id="670bb-130">ID para o turno aberto.</span><span class="sxs-lookup"><span data-stu-id="670bb-130">ID for the open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="670bb-131">Relações</span><span class="sxs-lookup"><span data-stu-id="670bb-131">Relationships</span></span>

<span data-ttu-id="670bb-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="670bb-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="670bb-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="670bb-133">JSON representation</span></span>

<span data-ttu-id="670bb-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="670bb-134">The following is a JSON representation of the resource.</span></span>

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
