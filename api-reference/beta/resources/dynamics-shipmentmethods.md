---
title: tipo de recurso shipmentMethods
description: Um método de remessa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 2f7ef9611fc85c13ac24c79b292e06a6bdc5d587
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365497"
---
# <a name="shipmentmethods-resource-type"></a><span data-ttu-id="353f9-103">tipo de recurso shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="353f9-103">shipmentMethods resource type</span></span>
<span data-ttu-id="353f9-104">Representa um método de entrega no Dynamics 365 Business central, como no-break, FEDEX e DHL.</span><span class="sxs-lookup"><span data-stu-id="353f9-104">Represents a method of shipment in Dynamics 365 Business Central, such as UPS, Fedex, and DHL.</span></span>

## <a name="methods"></a><span data-ttu-id="353f9-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="353f9-105">Methods</span></span>

| <span data-ttu-id="353f9-106">Método</span><span class="sxs-lookup"><span data-stu-id="353f9-106">Method</span></span>       | <span data-ttu-id="353f9-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="353f9-107">Return Type</span></span>  |<span data-ttu-id="353f9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="353f9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="353f9-109">Obter shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="353f9-109">Get shipmentMethods</span></span>](../api/dynamics-shipmentmethods-get.md)|<span data-ttu-id="353f9-110">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="353f9-110">shipmentMethods</span></span>|<span data-ttu-id="353f9-111">Obtém um método de remessa.</span><span class="sxs-lookup"><span data-stu-id="353f9-111">Gets a shipment method.</span></span>|
|[<span data-ttu-id="353f9-112">Postar shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="353f9-112">Post shipmentMethods</span></span>](../api/dynamics-create-shipmentmethods.md)|<span data-ttu-id="353f9-113">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="353f9-113">shipmentMethods</span></span>|<span data-ttu-id="353f9-114">Cria um método de remessa.</span><span class="sxs-lookup"><span data-stu-id="353f9-114">Creates a shipment method.</span></span>|
|[<span data-ttu-id="353f9-115">Patch shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="353f9-115">Patch shipmentMethods</span></span>](../api/dynamics-shipmentmethods-update.md)|<span data-ttu-id="353f9-116">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="353f9-116">shipmentMethods</span></span>|<span data-ttu-id="353f9-117">Atualiza um método de remessa.</span><span class="sxs-lookup"><span data-stu-id="353f9-117">Updates a shipment method.</span></span>|
|[<span data-ttu-id="353f9-118">Excluir shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="353f9-118">Delete shipmentMethods</span></span>](../api/dynamics-shipmentmethods-delete.md)|<span data-ttu-id="353f9-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="353f9-119">none</span></span>|<span data-ttu-id="353f9-120">Exclui um método de remessa.</span><span class="sxs-lookup"><span data-stu-id="353f9-120">Deletes a shipment method.</span></span>|

## <a name="properties"></a><span data-ttu-id="353f9-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="353f9-121">Properties</span></span>
| <span data-ttu-id="353f9-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="353f9-122">Property</span></span>     | <span data-ttu-id="353f9-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="353f9-123">Type</span></span>   |<span data-ttu-id="353f9-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="353f9-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="353f9-125">id</span><span class="sxs-lookup"><span data-stu-id="353f9-125">id</span></span>|<span data-ttu-id="353f9-126">GUID</span><span class="sxs-lookup"><span data-stu-id="353f9-126">GUID</span></span>|<span data-ttu-id="353f9-127">A ID exclusiva do shipmentMethod.</span><span class="sxs-lookup"><span data-stu-id="353f9-127">The unique ID of the shipmentMethod.</span></span> <span data-ttu-id="353f9-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="353f9-128">Non-editable.</span></span>|
|<span data-ttu-id="353f9-129">código</span><span class="sxs-lookup"><span data-stu-id="353f9-129">code</span></span>|<span data-ttu-id="353f9-130">string</span><span class="sxs-lookup"><span data-stu-id="353f9-130">string</span></span>|<span data-ttu-id="353f9-131">Especifica o código do método de remessa.</span><span class="sxs-lookup"><span data-stu-id="353f9-131">Specifies the shipment method code.</span></span>|
|<span data-ttu-id="353f9-132">displayName</span><span class="sxs-lookup"><span data-stu-id="353f9-132">displayName</span></span>|<span data-ttu-id="353f9-133">string</span><span class="sxs-lookup"><span data-stu-id="353f9-133">string</span></span>|<span data-ttu-id="353f9-134">Especifica o nome de exibição do método de remessa.</span><span class="sxs-lookup"><span data-stu-id="353f9-134">Specifies the shipment method display name.</span></span>|
|<span data-ttu-id="353f9-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="353f9-135">lastModifiedDateTime</span></span>|<span data-ttu-id="353f9-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="353f9-136">datetime</span></span>|<span data-ttu-id="353f9-137">O último DateTime que o método de remessa foi modificado.</span><span class="sxs-lookup"><span data-stu-id="353f9-137">The last datetime the shipment method was modified.</span></span> <span data-ttu-id="353f9-138">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="353f9-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="353f9-139">Relações</span><span class="sxs-lookup"><span data-stu-id="353f9-139">Relationships</span></span>
<span data-ttu-id="353f9-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="353f9-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="353f9-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="353f9-141">JSON representation</span></span>

<span data-ttu-id="353f9-142">Veja a seguir uma representação JSON do shipmentMethod.</span><span class="sxs-lookup"><span data-stu-id="353f9-142">Here is a JSON representation of the shipmentMethod.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```


