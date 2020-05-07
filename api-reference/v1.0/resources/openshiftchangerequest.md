---
title: tipo de recurso openShiftChangeRequest
description: Representa uma solicitação para solicitar um turno aberto em um cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 47a2aa9eddc4e45d88c3768ded2b44e9d5952178
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154981"
---
# <a name="openshiftchangerequest-resource-type"></a><span data-ttu-id="76d7a-103">tipo de recurso openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="76d7a-103">openShiftChangeRequest resource type</span></span>

<span data-ttu-id="76d7a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76d7a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="76d7a-105">Representa a solicitação para solicitar um [openShift](../resources/openshift.md) em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="76d7a-105">Represents request to claim an [openShift](../resources/openshift.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="76d7a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="76d7a-106">Methods</span></span>

| <span data-ttu-id="76d7a-107">Método</span><span class="sxs-lookup"><span data-stu-id="76d7a-107">Method</span></span>       | <span data-ttu-id="76d7a-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="76d7a-108">Return Type</span></span> | <span data-ttu-id="76d7a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="76d7a-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="76d7a-110">List</span><span class="sxs-lookup"><span data-stu-id="76d7a-110">List</span></span>](../api/openshiftchangerequest-list.md) | <span data-ttu-id="76d7a-111">Coleção de [openShiftChangeRequest](openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="76d7a-111">Collection of [openShiftChangeRequest](openshiftchangerequest.md)</span></span> | <span data-ttu-id="76d7a-112">Listar as propriedades e os relacionamentos dos objetos **openShiftChangeRequest** em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="76d7a-112">List the properties and relationships of **openShiftChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="76d7a-113">Create</span><span class="sxs-lookup"><span data-stu-id="76d7a-113">Create</span></span>](../api/openshiftchangerequest-post.md) | [<span data-ttu-id="76d7a-114">openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="76d7a-114">openShiftChangeRequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="76d7a-115">Criar uma instância de um objeto **openShiftChangeRequest** .</span><span class="sxs-lookup"><span data-stu-id="76d7a-115">Create an instance of an **openShiftChangeRequest** object.</span></span> |
| [<span data-ttu-id="76d7a-116">Get</span><span class="sxs-lookup"><span data-stu-id="76d7a-116">Get</span></span>](../api/openshiftchangerequest-get.md) | [<span data-ttu-id="76d7a-117">openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="76d7a-117">openShiftChangeRequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="76d7a-118">Leia as propriedades e os relacionamentos de um objeto **openShiftChangeRequest** .</span><span class="sxs-lookup"><span data-stu-id="76d7a-118">Read the properties and relationships of an **openShiftChangeRequest** object.</span></span> |
|[<span data-ttu-id="76d7a-119">Aprovar</span><span class="sxs-lookup"><span data-stu-id="76d7a-119">Approve</span></span>](../api/openshiftchangerequest-approve.md)|<span data-ttu-id="76d7a-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="76d7a-120">None</span></span>|<span data-ttu-id="76d7a-121">Aprovar uma solicitação de alteração de turno aberta.</span><span class="sxs-lookup"><span data-stu-id="76d7a-121">Approve an open shift change request.</span></span>|
|[<span data-ttu-id="76d7a-122">Aceito</span><span class="sxs-lookup"><span data-stu-id="76d7a-122">Decline</span></span>](../api/openshiftchangerequest-decline.md)|<span data-ttu-id="76d7a-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="76d7a-123">None</span></span>| <span data-ttu-id="76d7a-124">Recusar uma solicitação de alteração de turno aberto.</span><span class="sxs-lookup"><span data-stu-id="76d7a-124">Decline an open shift change request.</span></span>|

## <a name="properties"></a><span data-ttu-id="76d7a-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="76d7a-125">Properties</span></span>

| <span data-ttu-id="76d7a-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76d7a-126">Property</span></span>     | <span data-ttu-id="76d7a-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="76d7a-127">Type</span></span>        | <span data-ttu-id="76d7a-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="76d7a-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="76d7a-129">openShiftId</span><span class="sxs-lookup"><span data-stu-id="76d7a-129">openShiftId</span></span>|<span data-ttu-id="76d7a-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76d7a-130">String</span></span>| <span data-ttu-id="76d7a-131">ID para o turno aberto.</span><span class="sxs-lookup"><span data-stu-id="76d7a-131">ID for the open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76d7a-132">Relações</span><span class="sxs-lookup"><span data-stu-id="76d7a-132">Relationships</span></span>

<span data-ttu-id="76d7a-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="76d7a-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="76d7a-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="76d7a-134">JSON representation</span></span>

<span data-ttu-id="76d7a-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="76d7a-135">The following is a JSON representation of the resource.</span></span>

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
