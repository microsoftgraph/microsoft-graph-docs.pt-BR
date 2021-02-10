---
title: Tipo de recurso openShiftChangeRequest
description: Representa uma solicitação para reivindicar um turno aberto em um cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b427d7914d95aaed794734bbbb39fa3eb139d06a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158678"
---
# <a name="openshiftchangerequest-resource-type"></a><span data-ttu-id="6268e-103">Tipo de recurso openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="6268e-103">openShiftChangeRequest resource type</span></span>

<span data-ttu-id="6268e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6268e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6268e-105">Representa a solicitação para [reivindicar um openShift](../resources/openshift.md) em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="6268e-105">Represents request to claim an [openShift](../resources/openshift.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6268e-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6268e-106">Methods</span></span>

| <span data-ttu-id="6268e-107">Método</span><span class="sxs-lookup"><span data-stu-id="6268e-107">Method</span></span>       | <span data-ttu-id="6268e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6268e-108">Return Type</span></span> | <span data-ttu-id="6268e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6268e-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6268e-110">List</span><span class="sxs-lookup"><span data-stu-id="6268e-110">List</span></span>](../api/openshiftchangerequest-list.md) | <span data-ttu-id="6268e-111">Coleção de [openShiftChangeRequest](openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="6268e-111">Collection of [openShiftChangeRequest](openshiftchangerequest.md)</span></span> | <span data-ttu-id="6268e-112">Listar as propriedades e os relacionamentos dos **objetos openShiftChangeRequest** em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="6268e-112">List the properties and relationships of **openShiftChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="6268e-113">Criar</span><span class="sxs-lookup"><span data-stu-id="6268e-113">Create</span></span>](../api/openshiftchangerequest-post.md) | [<span data-ttu-id="6268e-114">openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="6268e-114">openShiftChangeRequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="6268e-115">Crie uma instância de um **objeto openShiftChangeRequest.**</span><span class="sxs-lookup"><span data-stu-id="6268e-115">Create an instance of an **openShiftChangeRequest** object.</span></span> |
| [<span data-ttu-id="6268e-116">Get</span><span class="sxs-lookup"><span data-stu-id="6268e-116">Get</span></span>](../api/openshiftchangerequest-get.md) | [<span data-ttu-id="6268e-117">openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="6268e-117">openShiftChangeRequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="6268e-118">Leia as propriedades e os relacionamentos de um **objeto openShiftChangeRequest.**</span><span class="sxs-lookup"><span data-stu-id="6268e-118">Read the properties and relationships of an **openShiftChangeRequest** object.</span></span> |
|[<span data-ttu-id="6268e-119">Aprovar</span><span class="sxs-lookup"><span data-stu-id="6268e-119">Approve</span></span>](../api/openshiftchangerequest-approve.md)|<span data-ttu-id="6268e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6268e-120">None</span></span>|<span data-ttu-id="6268e-121">Aprovar uma solicitação de alteração de turno aberto.</span><span class="sxs-lookup"><span data-stu-id="6268e-121">Approve an open shift change request.</span></span>|
|[<span data-ttu-id="6268e-122">Recusar</span><span class="sxs-lookup"><span data-stu-id="6268e-122">Decline</span></span>](../api/openshiftchangerequest-decline.md)|<span data-ttu-id="6268e-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6268e-123">None</span></span>| <span data-ttu-id="6268e-124">Recusar uma solicitação de alteração de turno aberto.</span><span class="sxs-lookup"><span data-stu-id="6268e-124">Decline an open shift change request.</span></span>|

## <a name="properties"></a><span data-ttu-id="6268e-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6268e-125">Properties</span></span>

| <span data-ttu-id="6268e-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6268e-126">Property</span></span>     | <span data-ttu-id="6268e-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="6268e-127">Type</span></span>        | <span data-ttu-id="6268e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="6268e-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6268e-129">openShiftId</span><span class="sxs-lookup"><span data-stu-id="6268e-129">openShiftId</span></span>|<span data-ttu-id="6268e-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6268e-130">String</span></span>| <span data-ttu-id="6268e-131">ID do turno aberto.</span><span class="sxs-lookup"><span data-stu-id="6268e-131">ID for the open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6268e-132">Relações</span><span class="sxs-lookup"><span data-stu-id="6268e-132">Relationships</span></span>

<span data-ttu-id="6268e-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6268e-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6268e-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6268e-134">JSON representation</span></span>

<span data-ttu-id="6268e-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6268e-135">The following is a JSON representation of the resource.</span></span>

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

