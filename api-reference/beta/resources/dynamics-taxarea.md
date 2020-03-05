---
title: tipo de recurso taxAreas
description: Uma área de impostos.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d2c4f007c23ae32fb79255a0a8f1509589740a70
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503429"
---
# <a name="taxareas-resource-type"></a><span data-ttu-id="89646-103">tipo de recurso taxAreas</span><span class="sxs-lookup"><span data-stu-id="89646-103">taxAreas resource type</span></span>

<span data-ttu-id="89646-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="89646-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89646-105">Representa um tipo de recurso de área de imposto no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="89646-105">Represents a tax area resource type in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="89646-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="89646-106">Methods</span></span>
| <span data-ttu-id="89646-107">Método</span><span class="sxs-lookup"><span data-stu-id="89646-107">Method</span></span>       | <span data-ttu-id="89646-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="89646-108">Return Type</span></span>  |<span data-ttu-id="89646-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="89646-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="89646-110">Obter taxAreas</span><span class="sxs-lookup"><span data-stu-id="89646-110">Get taxAreas</span></span>](../api/dynamics-taxarea-get.md)|<span data-ttu-id="89646-111">taxAreas</span><span class="sxs-lookup"><span data-stu-id="89646-111">taxAreas</span></span>|<span data-ttu-id="89646-112">Obtém um objeto de área de impostos.</span><span class="sxs-lookup"><span data-stu-id="89646-112">Gets a tax area object.</span></span>|
|[<span data-ttu-id="89646-113">Postar taxAreas</span><span class="sxs-lookup"><span data-stu-id="89646-113">Post taxAreas</span></span>](../api/dynamics-create-taxarea.md)|<span data-ttu-id="89646-114">taxAreas</span><span class="sxs-lookup"><span data-stu-id="89646-114">taxAreas</span></span>|<span data-ttu-id="89646-115">Cria um objeto de área de impostos.</span><span class="sxs-lookup"><span data-stu-id="89646-115">Creates a tax area object.</span></span>|
|[<span data-ttu-id="89646-116">Patch taxAreas</span><span class="sxs-lookup"><span data-stu-id="89646-116">Patch taxAreas</span></span>](../api/dynamics-taxarea-update.md)|<span data-ttu-id="89646-117">taxAreas</span><span class="sxs-lookup"><span data-stu-id="89646-117">taxAreas</span></span>|<span data-ttu-id="89646-118">Atualiza um objeto de área de impostos.</span><span class="sxs-lookup"><span data-stu-id="89646-118">Updates a tax area object.</span></span>|
|[<span data-ttu-id="89646-119">Excluir taxAreas</span><span class="sxs-lookup"><span data-stu-id="89646-119">Delete taxAreas</span></span>](../api/dynamics-taxarea-delete.md)|<span data-ttu-id="89646-120">nenhuma</span><span class="sxs-lookup"><span data-stu-id="89646-120">none</span></span>|<span data-ttu-id="89646-121">Exclui um objeto de área de impostos.</span><span class="sxs-lookup"><span data-stu-id="89646-121">Deletes a tax area object.</span></span>|

## <a name="properties"></a><span data-ttu-id="89646-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89646-122">Properties</span></span>
| <span data-ttu-id="89646-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89646-123">Property</span></span>     | <span data-ttu-id="89646-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="89646-124">Type</span></span>   |<span data-ttu-id="89646-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="89646-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89646-126">id</span><span class="sxs-lookup"><span data-stu-id="89646-126">id</span></span>|<span data-ttu-id="89646-127">GUID</span><span class="sxs-lookup"><span data-stu-id="89646-127">GUID</span></span>|<span data-ttu-id="89646-128">A identificação exclusiva da área de impostos.</span><span class="sxs-lookup"><span data-stu-id="89646-128">The unique ID of the tax area.</span></span> <span data-ttu-id="89646-129">Não editável.</span><span class="sxs-lookup"><span data-stu-id="89646-129">Non-editable.</span></span>|
|<span data-ttu-id="89646-130">código</span><span class="sxs-lookup"><span data-stu-id="89646-130">code</span></span>|<span data-ttu-id="89646-131">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="89646-131">string, maximum size 20</span></span>| <span data-ttu-id="89646-132">O código da área de impostos.</span><span class="sxs-lookup"><span data-stu-id="89646-132">The code of the tax area.</span></span>|
|<span data-ttu-id="89646-133">displayName</span><span class="sxs-lookup"><span data-stu-id="89646-133">displayName</span></span>|<span data-ttu-id="89646-134">Cadeia de caracteres, tamanho máximo 50</span><span class="sxs-lookup"><span data-stu-id="89646-134">string, maximum size 50</span></span>| <span data-ttu-id="89646-135">O nome de exibição da área de impostos.</span><span class="sxs-lookup"><span data-stu-id="89646-135">The display name of the tax area.</span></span>|
|<span data-ttu-id="89646-136">taxType</span><span class="sxs-lookup"><span data-stu-id="89646-136">taxType</span></span>|<span data-ttu-id="89646-137">string</span><span class="sxs-lookup"><span data-stu-id="89646-137">string</span></span>|<span data-ttu-id="89646-138">O tipo de imposto da área de impostos.</span><span class="sxs-lookup"><span data-stu-id="89646-138">The tax type of the tax area.</span></span>|
|<span data-ttu-id="89646-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89646-139">lastModifiedDateTime</span></span>|<span data-ttu-id="89646-140">datetime</span><span class="sxs-lookup"><span data-stu-id="89646-140">datetime</span></span>|<span data-ttu-id="89646-141">A última data/hora em que a área de impostos foi modificada.</span><span class="sxs-lookup"><span data-stu-id="89646-141">The last datetime the tax area was modified.</span></span> <span data-ttu-id="89646-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="89646-142">Read-Only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89646-143">Relações</span><span class="sxs-lookup"><span data-stu-id="89646-143">Relationships</span></span>

## <a name="json-representation"></a><span data-ttu-id="89646-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89646-144">JSON representation</span></span>

<span data-ttu-id="89646-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="89646-145">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "taxType": "String",
  "lastModifiedDateTime": "datetime"
}
```


