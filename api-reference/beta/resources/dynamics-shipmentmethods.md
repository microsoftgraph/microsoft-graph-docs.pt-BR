---
title: tipo de recurso shipmentMethods
description: Um método de remessa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 2f7ef9611fc85c13ac24c79b292e06a6bdc5d587
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543032"
---
# <a name="shipmentmethods-resource-type"></a><span data-ttu-id="b133d-103">tipo de recurso shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="b133d-103">shipmentMethods resource type</span></span>
<span data-ttu-id="b133d-104">Representa um método de entrega no Dynamics 365 Business central, como no-break, FEDEX e DHL.</span><span class="sxs-lookup"><span data-stu-id="b133d-104">Represents a method of shipment in Dynamics 365 Business Central, such as UPS, Fedex, and DHL.</span></span>

## <a name="methods"></a><span data-ttu-id="b133d-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="b133d-105">Methods</span></span>

| <span data-ttu-id="b133d-106">Método</span><span class="sxs-lookup"><span data-stu-id="b133d-106">Method</span></span>       | <span data-ttu-id="b133d-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b133d-107">Return Type</span></span>  |<span data-ttu-id="b133d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b133d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b133d-109">Obter shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="b133d-109">Get shipmentMethods</span></span>](../api/dynamics-shipmentmethods-get.md)|<span data-ttu-id="b133d-110">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="b133d-110">shipmentMethods</span></span>|<span data-ttu-id="b133d-111">Obtém um método de remessa.</span><span class="sxs-lookup"><span data-stu-id="b133d-111">Gets a shipment method.</span></span>|
|[<span data-ttu-id="b133d-112">Postar shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="b133d-112">Post shipmentMethods</span></span>](../api/dynamics-create-shipmentmethods.md)|<span data-ttu-id="b133d-113">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="b133d-113">shipmentMethods</span></span>|<span data-ttu-id="b133d-114">Cria um método de remessa.</span><span class="sxs-lookup"><span data-stu-id="b133d-114">Creates a shipment method.</span></span>|
|[<span data-ttu-id="b133d-115">Patch shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="b133d-115">Patch shipmentMethods</span></span>](../api/dynamics-shipmentmethods-update.md)|<span data-ttu-id="b133d-116">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="b133d-116">shipmentMethods</span></span>|<span data-ttu-id="b133d-117">Atualiza um método de remessa.</span><span class="sxs-lookup"><span data-stu-id="b133d-117">Updates a shipment method.</span></span>|
|[<span data-ttu-id="b133d-118">Excluir shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="b133d-118">Delete shipmentMethods</span></span>](../api/dynamics-shipmentmethods-delete.md)|<span data-ttu-id="b133d-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b133d-119">none</span></span>|<span data-ttu-id="b133d-120">Exclui um método de remessa.</span><span class="sxs-lookup"><span data-stu-id="b133d-120">Deletes a shipment method.</span></span>|

## <a name="properties"></a><span data-ttu-id="b133d-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b133d-121">Properties</span></span>
| <span data-ttu-id="b133d-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b133d-122">Property</span></span>     | <span data-ttu-id="b133d-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b133d-123">Type</span></span>   |<span data-ttu-id="b133d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b133d-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b133d-125">id</span><span class="sxs-lookup"><span data-stu-id="b133d-125">id</span></span>|<span data-ttu-id="b133d-126">GUID</span><span class="sxs-lookup"><span data-stu-id="b133d-126">GUID</span></span>|<span data-ttu-id="b133d-127">A ID exclusiva do shipmentMethod.</span><span class="sxs-lookup"><span data-stu-id="b133d-127">The unique ID of the shipmentMethod.</span></span> <span data-ttu-id="b133d-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="b133d-128">Non-editable.</span></span>|
|<span data-ttu-id="b133d-129">código</span><span class="sxs-lookup"><span data-stu-id="b133d-129">code</span></span>|<span data-ttu-id="b133d-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b133d-130">string</span></span>|<span data-ttu-id="b133d-131">Especifica o código do método de remessa.</span><span class="sxs-lookup"><span data-stu-id="b133d-131">Specifies the shipment method code.</span></span>|
|<span data-ttu-id="b133d-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b133d-132">displayName</span></span>|<span data-ttu-id="b133d-133">string</span><span class="sxs-lookup"><span data-stu-id="b133d-133">string</span></span>|<span data-ttu-id="b133d-134">Especifica o nome de exibição do método de remessa.</span><span class="sxs-lookup"><span data-stu-id="b133d-134">Specifies the shipment method display name.</span></span>|
|<span data-ttu-id="b133d-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b133d-135">lastModifiedDateTime</span></span>|<span data-ttu-id="b133d-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="b133d-136">datetime</span></span>|<span data-ttu-id="b133d-137">O último DateTime que o método de remessa foi modificado.</span><span class="sxs-lookup"><span data-stu-id="b133d-137">The last datetime the shipment method was modified.</span></span> <span data-ttu-id="b133d-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b133d-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="b133d-139">Relações</span><span class="sxs-lookup"><span data-stu-id="b133d-139">Relationships</span></span>
<span data-ttu-id="b133d-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b133d-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b133d-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b133d-141">JSON representation</span></span>

<span data-ttu-id="b133d-142">Veja a seguir uma representação JSON do shipmentMethod.</span><span class="sxs-lookup"><span data-stu-id="b133d-142">Here is a JSON representation of the shipmentMethod.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```


