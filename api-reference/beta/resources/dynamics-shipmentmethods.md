---
title: tipo de recurso shipmentMethods
description: Um método de remessa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 94ebd10ef87946b5333ec5a06d5edccadc298158
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503569"
---
# <a name="shipmentmethods-resource-type"></a><span data-ttu-id="866b3-103">tipo de recurso shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="866b3-103">shipmentMethods resource type</span></span>

<span data-ttu-id="866b3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="866b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="866b3-105">Representa um método de entrega no Dynamics 365 Business central, como no-break, FEDEX e DHL.</span><span class="sxs-lookup"><span data-stu-id="866b3-105">Represents a method of shipment in Dynamics 365 Business Central, such as UPS, Fedex, and DHL.</span></span>

## <a name="methods"></a><span data-ttu-id="866b3-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="866b3-106">Methods</span></span>

| <span data-ttu-id="866b3-107">Método</span><span class="sxs-lookup"><span data-stu-id="866b3-107">Method</span></span>       | <span data-ttu-id="866b3-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="866b3-108">Return Type</span></span>  |<span data-ttu-id="866b3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="866b3-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="866b3-110">Obter shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="866b3-110">Get shipmentMethods</span></span>](../api/dynamics-shipmentmethods-get.md)|<span data-ttu-id="866b3-111">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="866b3-111">shipmentMethods</span></span>|<span data-ttu-id="866b3-112">Obtém um método de remessa.</span><span class="sxs-lookup"><span data-stu-id="866b3-112">Gets a shipment method.</span></span>|
|[<span data-ttu-id="866b3-113">Postar shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="866b3-113">Post shipmentMethods</span></span>](../api/dynamics-create-shipmentmethods.md)|<span data-ttu-id="866b3-114">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="866b3-114">shipmentMethods</span></span>|<span data-ttu-id="866b3-115">Cria um método de remessa.</span><span class="sxs-lookup"><span data-stu-id="866b3-115">Creates a shipment method.</span></span>|
|[<span data-ttu-id="866b3-116">Patch shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="866b3-116">Patch shipmentMethods</span></span>](../api/dynamics-shipmentmethods-update.md)|<span data-ttu-id="866b3-117">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="866b3-117">shipmentMethods</span></span>|<span data-ttu-id="866b3-118">Atualiza um método de remessa.</span><span class="sxs-lookup"><span data-stu-id="866b3-118">Updates a shipment method.</span></span>|
|[<span data-ttu-id="866b3-119">Excluir shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="866b3-119">Delete shipmentMethods</span></span>](../api/dynamics-shipmentmethods-delete.md)|<span data-ttu-id="866b3-120">nenhuma</span><span class="sxs-lookup"><span data-stu-id="866b3-120">none</span></span>|<span data-ttu-id="866b3-121">Exclui um método de remessa.</span><span class="sxs-lookup"><span data-stu-id="866b3-121">Deletes a shipment method.</span></span>|

## <a name="properties"></a><span data-ttu-id="866b3-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="866b3-122">Properties</span></span>
| <span data-ttu-id="866b3-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="866b3-123">Property</span></span>     | <span data-ttu-id="866b3-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="866b3-124">Type</span></span>   |<span data-ttu-id="866b3-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="866b3-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="866b3-126">id</span><span class="sxs-lookup"><span data-stu-id="866b3-126">id</span></span>|<span data-ttu-id="866b3-127">GUID</span><span class="sxs-lookup"><span data-stu-id="866b3-127">GUID</span></span>|<span data-ttu-id="866b3-128">A ID exclusiva do shipmentMethod.</span><span class="sxs-lookup"><span data-stu-id="866b3-128">The unique ID of the shipmentMethod.</span></span> <span data-ttu-id="866b3-129">Não editável.</span><span class="sxs-lookup"><span data-stu-id="866b3-129">Non-editable.</span></span>|
|<span data-ttu-id="866b3-130">código</span><span class="sxs-lookup"><span data-stu-id="866b3-130">code</span></span>|<span data-ttu-id="866b3-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="866b3-131">string</span></span>|<span data-ttu-id="866b3-132">Especifica o código do método de remessa.</span><span class="sxs-lookup"><span data-stu-id="866b3-132">Specifies the shipment method code.</span></span>|
|<span data-ttu-id="866b3-133">displayName</span><span class="sxs-lookup"><span data-stu-id="866b3-133">displayName</span></span>|<span data-ttu-id="866b3-134">string</span><span class="sxs-lookup"><span data-stu-id="866b3-134">string</span></span>|<span data-ttu-id="866b3-135">Especifica o nome de exibição do método de remessa.</span><span class="sxs-lookup"><span data-stu-id="866b3-135">Specifies the shipment method display name.</span></span>|
|<span data-ttu-id="866b3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="866b3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="866b3-137">datetime</span><span class="sxs-lookup"><span data-stu-id="866b3-137">datetime</span></span>|<span data-ttu-id="866b3-138">O último DateTime que o método de remessa foi modificado.</span><span class="sxs-lookup"><span data-stu-id="866b3-138">The last datetime the shipment method was modified.</span></span> <span data-ttu-id="866b3-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="866b3-139">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="866b3-140">Relações</span><span class="sxs-lookup"><span data-stu-id="866b3-140">Relationships</span></span>
<span data-ttu-id="866b3-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="866b3-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="866b3-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="866b3-142">JSON representation</span></span>

<span data-ttu-id="866b3-143">Veja a seguir uma representação JSON do shipmentMethod.</span><span class="sxs-lookup"><span data-stu-id="866b3-143">Here is a JSON representation of the shipmentMethod.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```


