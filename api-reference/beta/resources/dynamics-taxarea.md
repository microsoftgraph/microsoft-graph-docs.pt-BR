---
title: tipo de recurso taxAreas
description: Uma área de impostos.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: aeda0ca136c178355a8a8f9589eb7410399ef62a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507228"
---
# <a name="taxareas-resource-type"></a><span data-ttu-id="56aa7-103">tipo de recurso taxAreas</span><span class="sxs-lookup"><span data-stu-id="56aa7-103">taxAreas resource type</span></span>
<span data-ttu-id="56aa7-104">Representa um tipo de recurso de área de imposto no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="56aa7-104">Represents a tax area resource type in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="56aa7-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="56aa7-105">Methods</span></span>
| <span data-ttu-id="56aa7-106">Método</span><span class="sxs-lookup"><span data-stu-id="56aa7-106">Method</span></span>       | <span data-ttu-id="56aa7-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="56aa7-107">Return Type</span></span>  |<span data-ttu-id="56aa7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="56aa7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="56aa7-109">Obter taxAreas</span><span class="sxs-lookup"><span data-stu-id="56aa7-109">Get taxAreas</span></span>](../api/dynamics-taxarea-get.md)|<span data-ttu-id="56aa7-110">taxAreas</span><span class="sxs-lookup"><span data-stu-id="56aa7-110">taxAreas</span></span>|<span data-ttu-id="56aa7-111">Obtém um objeto de área de impostos.</span><span class="sxs-lookup"><span data-stu-id="56aa7-111">Gets a tax area object.</span></span>|
|[<span data-ttu-id="56aa7-112">Postar taxAreas</span><span class="sxs-lookup"><span data-stu-id="56aa7-112">Post taxAreas</span></span>](../api/dynamics-create-taxarea.md)|<span data-ttu-id="56aa7-113">taxAreas</span><span class="sxs-lookup"><span data-stu-id="56aa7-113">taxAreas</span></span>|<span data-ttu-id="56aa7-114">Cria um objeto de área de impostos.</span><span class="sxs-lookup"><span data-stu-id="56aa7-114">Creates a tax area object.</span></span>|
|[<span data-ttu-id="56aa7-115">Patch taxAreas</span><span class="sxs-lookup"><span data-stu-id="56aa7-115">Patch taxAreas</span></span>](../api/dynamics-taxarea-update.md)|<span data-ttu-id="56aa7-116">taxAreas</span><span class="sxs-lookup"><span data-stu-id="56aa7-116">taxAreas</span></span>|<span data-ttu-id="56aa7-117">Atualiza um objeto de área de impostos.</span><span class="sxs-lookup"><span data-stu-id="56aa7-117">Updates a tax area object.</span></span>|
|[<span data-ttu-id="56aa7-118">Excluir taxAreas</span><span class="sxs-lookup"><span data-stu-id="56aa7-118">Delete taxAreas</span></span>](../api/dynamics-taxarea-delete.md)|<span data-ttu-id="56aa7-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="56aa7-119">none</span></span>|<span data-ttu-id="56aa7-120">Exclui um objeto de área de impostos.</span><span class="sxs-lookup"><span data-stu-id="56aa7-120">Deletes a tax area object.</span></span>|

## <a name="properties"></a><span data-ttu-id="56aa7-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56aa7-121">Properties</span></span>
| <span data-ttu-id="56aa7-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56aa7-122">Property</span></span>     | <span data-ttu-id="56aa7-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="56aa7-123">Type</span></span>   |<span data-ttu-id="56aa7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="56aa7-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56aa7-125">id</span><span class="sxs-lookup"><span data-stu-id="56aa7-125">id</span></span>|<span data-ttu-id="56aa7-126">GUID</span><span class="sxs-lookup"><span data-stu-id="56aa7-126">GUID</span></span>|<span data-ttu-id="56aa7-127">A identificação exclusiva da área de impostos.</span><span class="sxs-lookup"><span data-stu-id="56aa7-127">The unique ID of the tax area.</span></span> <span data-ttu-id="56aa7-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="56aa7-128">Non-editable.</span></span>|
|<span data-ttu-id="56aa7-129">code</span><span class="sxs-lookup"><span data-stu-id="56aa7-129">code</span></span>|<span data-ttu-id="56aa7-130">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="56aa7-130">string, maximum size 20</span></span>| <span data-ttu-id="56aa7-131">O código da área de impostos.</span><span class="sxs-lookup"><span data-stu-id="56aa7-131">The code of the tax area.</span></span>|
|<span data-ttu-id="56aa7-132">displayName</span><span class="sxs-lookup"><span data-stu-id="56aa7-132">displayName</span></span>|<span data-ttu-id="56aa7-133">Cadeia de caracteres, tamanho máximo 50</span><span class="sxs-lookup"><span data-stu-id="56aa7-133">string, maximum size 50</span></span>| <span data-ttu-id="56aa7-134">O nome de exibição da área de impostos.</span><span class="sxs-lookup"><span data-stu-id="56aa7-134">The display name of the tax area.</span></span>|
|<span data-ttu-id="56aa7-135">taxType</span><span class="sxs-lookup"><span data-stu-id="56aa7-135">taxType</span></span>|<span data-ttu-id="56aa7-136">string</span><span class="sxs-lookup"><span data-stu-id="56aa7-136">string</span></span>|<span data-ttu-id="56aa7-137">O tipo de imposto da área de impostos.</span><span class="sxs-lookup"><span data-stu-id="56aa7-137">The tax type of the tax area.</span></span>|
|<span data-ttu-id="56aa7-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56aa7-138">lastModifiedDateTime</span></span>|<span data-ttu-id="56aa7-139">DateTime</span><span class="sxs-lookup"><span data-stu-id="56aa7-139">datetime</span></span>|<span data-ttu-id="56aa7-140">A última data/hora em que a área de impostos foi modificada.</span><span class="sxs-lookup"><span data-stu-id="56aa7-140">The last datetime the tax area was modified.</span></span> <span data-ttu-id="56aa7-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56aa7-141">Read-Only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56aa7-142">Relações</span><span class="sxs-lookup"><span data-stu-id="56aa7-142">Relationships</span></span>

## <a name="json-representation"></a><span data-ttu-id="56aa7-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56aa7-143">JSON representation</span></span>

<span data-ttu-id="56aa7-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="56aa7-144">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "taxType": "String",
  "lastModifiedDateTime": "datetime"
}
```


