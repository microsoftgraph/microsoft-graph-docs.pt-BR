---
title: tipo de recurso shipmentMethods
description: Um método de remessa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d45153a08572f32f29128fd4d3f51638d71c951b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027066"
---
# <a name="shipmentmethods-resource-type"></a><span data-ttu-id="a89cd-103">tipo de recurso shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="a89cd-103">shipmentMethods resource type</span></span>

<span data-ttu-id="a89cd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a89cd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a89cd-105">Representa um método de entrega no Dynamics 365 Business central, como no-break, FEDEX e DHL.</span><span class="sxs-lookup"><span data-stu-id="a89cd-105">Represents a method of shipment in Dynamics 365 Business Central, such as UPS, Fedex, and DHL.</span></span>

## <a name="methods"></a><span data-ttu-id="a89cd-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="a89cd-106">Methods</span></span>

| <span data-ttu-id="a89cd-107">Método</span><span class="sxs-lookup"><span data-stu-id="a89cd-107">Method</span></span>       | <span data-ttu-id="a89cd-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a89cd-108">Return Type</span></span>  |<span data-ttu-id="a89cd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a89cd-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a89cd-110">Obter shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="a89cd-110">Get shipmentMethods</span></span>](../api/dynamics-shipmentmethods-get.md)|<span data-ttu-id="a89cd-111">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="a89cd-111">shipmentMethods</span></span>|<span data-ttu-id="a89cd-112">Obtém um método de remessa.</span><span class="sxs-lookup"><span data-stu-id="a89cd-112">Gets a shipment method.</span></span>|
|[<span data-ttu-id="a89cd-113">Postar shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="a89cd-113">Post shipmentMethods</span></span>](../api/dynamics-create-shipmentmethods.md)|<span data-ttu-id="a89cd-114">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="a89cd-114">shipmentMethods</span></span>|<span data-ttu-id="a89cd-115">Cria um método de remessa.</span><span class="sxs-lookup"><span data-stu-id="a89cd-115">Creates a shipment method.</span></span>|
|[<span data-ttu-id="a89cd-116">Patch shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="a89cd-116">Patch shipmentMethods</span></span>](../api/dynamics-shipmentmethods-update.md)|<span data-ttu-id="a89cd-117">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="a89cd-117">shipmentMethods</span></span>|<span data-ttu-id="a89cd-118">Atualiza um método de remessa.</span><span class="sxs-lookup"><span data-stu-id="a89cd-118">Updates a shipment method.</span></span>|
|[<span data-ttu-id="a89cd-119">Excluir shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="a89cd-119">Delete shipmentMethods</span></span>](../api/dynamics-shipmentmethods-delete.md)|<span data-ttu-id="a89cd-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="a89cd-120">none</span></span>|<span data-ttu-id="a89cd-121">Exclui um método de remessa.</span><span class="sxs-lookup"><span data-stu-id="a89cd-121">Deletes a shipment method.</span></span>|

## <a name="properties"></a><span data-ttu-id="a89cd-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a89cd-122">Properties</span></span>
| <span data-ttu-id="a89cd-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a89cd-123">Property</span></span>     | <span data-ttu-id="a89cd-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="a89cd-124">Type</span></span>   |<span data-ttu-id="a89cd-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="a89cd-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a89cd-126">id</span><span class="sxs-lookup"><span data-stu-id="a89cd-126">id</span></span>|<span data-ttu-id="a89cd-127">GUID</span><span class="sxs-lookup"><span data-stu-id="a89cd-127">GUID</span></span>|<span data-ttu-id="a89cd-128">A ID exclusiva do shipmentMethod.</span><span class="sxs-lookup"><span data-stu-id="a89cd-128">The unique ID of the shipmentMethod.</span></span> <span data-ttu-id="a89cd-129">Não editável.</span><span class="sxs-lookup"><span data-stu-id="a89cd-129">Non-editable.</span></span>|
|<span data-ttu-id="a89cd-130">código</span><span class="sxs-lookup"><span data-stu-id="a89cd-130">code</span></span>|<span data-ttu-id="a89cd-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a89cd-131">string</span></span>|<span data-ttu-id="a89cd-132">Especifica o código do método de remessa.</span><span class="sxs-lookup"><span data-stu-id="a89cd-132">Specifies the shipment method code.</span></span>|
|<span data-ttu-id="a89cd-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a89cd-133">displayName</span></span>|<span data-ttu-id="a89cd-134">string</span><span class="sxs-lookup"><span data-stu-id="a89cd-134">string</span></span>|<span data-ttu-id="a89cd-135">Especifica o nome de exibição do método de remessa.</span><span class="sxs-lookup"><span data-stu-id="a89cd-135">Specifies the shipment method display name.</span></span>|
|<span data-ttu-id="a89cd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a89cd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a89cd-137">datetime</span><span class="sxs-lookup"><span data-stu-id="a89cd-137">datetime</span></span>|<span data-ttu-id="a89cd-138">O último DateTime que o método de remessa foi modificado.</span><span class="sxs-lookup"><span data-stu-id="a89cd-138">The last datetime the shipment method was modified.</span></span> <span data-ttu-id="a89cd-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a89cd-139">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="a89cd-140">Relações</span><span class="sxs-lookup"><span data-stu-id="a89cd-140">Relationships</span></span>
<span data-ttu-id="a89cd-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a89cd-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a89cd-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a89cd-142">JSON representation</span></span>

<span data-ttu-id="a89cd-143">Veja a seguir uma representação JSON do shipmentMethod.</span><span class="sxs-lookup"><span data-stu-id="a89cd-143">Here is a JSON representation of the shipmentMethod.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```




