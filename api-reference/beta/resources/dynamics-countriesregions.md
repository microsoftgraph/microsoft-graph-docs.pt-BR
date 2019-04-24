---
title: tipo de recurso countriesRegions
description: Um objeto de países/regiões no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: b6f50ba3046a402f2b8729529675653286808459
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507263"
---
# <a name="countriesregions-resource-type"></a><span data-ttu-id="3d58b-103">tipo de recurso countriesRegions</span><span class="sxs-lookup"><span data-stu-id="3d58b-103">countriesRegions resource type</span></span>
<span data-ttu-id="3d58b-104">Representa um objeto countriesRegions no Dynamics 365 Business central, que é parte de um endereço.</span><span class="sxs-lookup"><span data-stu-id="3d58b-104">Represents a countriesRegions object in Dynamics 365 Business Central, which is part of an address.</span></span>

## <a name="methods"></a><span data-ttu-id="3d58b-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="3d58b-105">Methods</span></span>

| <span data-ttu-id="3d58b-106">Método</span><span class="sxs-lookup"><span data-stu-id="3d58b-106">Method</span></span>                                                              | <span data-ttu-id="3d58b-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3d58b-107">Return Type</span></span>    |<span data-ttu-id="3d58b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d58b-108">Description</span></span>                |
|:--------------------------------------------------------------------|:---------------|:--------------------------|
|[<span data-ttu-id="3d58b-109">Obter countriesRegions</span><span class="sxs-lookup"><span data-stu-id="3d58b-109">Get countriesRegions</span></span>](../api/dynamics-countriesregions-get.md)      |<span data-ttu-id="3d58b-110">countriesRegions</span><span class="sxs-lookup"><span data-stu-id="3d58b-110">countriesRegions</span></span>|<span data-ttu-id="3d58b-111">Obter um país/região.</span><span class="sxs-lookup"><span data-stu-id="3d58b-111">Get a Countries/Regions.</span></span>   |
|[<span data-ttu-id="3d58b-112">Postar countriesRegions</span><span class="sxs-lookup"><span data-stu-id="3d58b-112">Post countriesRegions</span></span>](../api/dynamics-create-countriesregions.md)  |<span data-ttu-id="3d58b-113">countriesRegions</span><span class="sxs-lookup"><span data-stu-id="3d58b-113">countriesRegions</span></span>|<span data-ttu-id="3d58b-114">Criar um país/região.</span><span class="sxs-lookup"><span data-stu-id="3d58b-114">Create a Countries/Regions.</span></span>|
|[<span data-ttu-id="3d58b-115">Patch countriesRegions</span><span class="sxs-lookup"><span data-stu-id="3d58b-115">Patch countriesRegions</span></span>](../api/dynamics-countriesregions-update.md) |<span data-ttu-id="3d58b-116">countriesRegions</span><span class="sxs-lookup"><span data-stu-id="3d58b-116">countriesRegions</span></span>|<span data-ttu-id="3d58b-117">Atualize um país/região.</span><span class="sxs-lookup"><span data-stu-id="3d58b-117">Update a Countries/Regions.</span></span>|
|[<span data-ttu-id="3d58b-118">Excluir countriesRegions</span><span class="sxs-lookup"><span data-stu-id="3d58b-118">Delete countriesRegions</span></span>](../api/dynamics-countriesregions-delete.md)|<span data-ttu-id="3d58b-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3d58b-119">none</span></span>            |<span data-ttu-id="3d58b-120">Exclua os países/regiões.</span><span class="sxs-lookup"><span data-stu-id="3d58b-120">Delete a Countries/Regions.</span></span>|

## <a name="properties"></a><span data-ttu-id="3d58b-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d58b-121">Properties</span></span>
| <span data-ttu-id="3d58b-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d58b-122">Property</span></span>       | <span data-ttu-id="3d58b-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d58b-123">Type</span></span>       |<span data-ttu-id="3d58b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d58b-124">Description</span></span>                                                  |
|:---------------|:-----------|:------------------------------------------------------------|
|<span data-ttu-id="3d58b-125">id</span><span class="sxs-lookup"><span data-stu-id="3d58b-125">id</span></span>              |<span data-ttu-id="3d58b-126">GUID</span><span class="sxs-lookup"><span data-stu-id="3d58b-126">GUID</span></span>        |<span data-ttu-id="3d58b-127">A identificação exclusiva do país/região.</span><span class="sxs-lookup"><span data-stu-id="3d58b-127">The unique ID of the country/region.</span></span> <span data-ttu-id="3d58b-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="3d58b-128">Non-editable.</span></span>           |
|<span data-ttu-id="3d58b-129">código</span><span class="sxs-lookup"><span data-stu-id="3d58b-129">code</span></span>            |<span data-ttu-id="3d58b-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d58b-130">string</span></span>      |<span data-ttu-id="3d58b-131">Especifica o código do país/região.</span><span class="sxs-lookup"><span data-stu-id="3d58b-131">Specifies the code of the country/region.</span></span>                    |
|<span data-ttu-id="3d58b-132">displayName</span><span class="sxs-lookup"><span data-stu-id="3d58b-132">displayName</span></span>     |<span data-ttu-id="3d58b-133">string</span><span class="sxs-lookup"><span data-stu-id="3d58b-133">string</span></span>      |<span data-ttu-id="3d58b-134">Especifica o nome de exibição do país/região.</span><span class="sxs-lookup"><span data-stu-id="3d58b-134">Specifies the display name of the country/region.</span></span>            |
|<span data-ttu-id="3d58b-135">addressFormat</span><span class="sxs-lookup"><span data-stu-id="3d58b-135">addressFormat</span></span>   |<span data-ttu-id="3d58b-136">string</span><span class="sxs-lookup"><span data-stu-id="3d58b-136">string</span></span>      |<span data-ttu-id="3d58b-137">Especifica o formato do endereço exibido em documentos de face externa.</span><span class="sxs-lookup"><span data-stu-id="3d58b-137">Specifies the format of the address that is displayed on external-facing documents.</span></span> <span data-ttu-id="3d58b-138">Você vincula um formato de endereço a um código de país/região para que documentos externos baseados em cartões ou documentos com esse código de país/região usem o formato de endereço especificado.</span><span class="sxs-lookup"><span data-stu-id="3d58b-138">You link an address format to a country/region code so that external-facing documents based on cards or documents with that country/region code use the specified address format.</span></span>|
|<span data-ttu-id="3d58b-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d58b-139">lastModifiedDateTime</span></span>|<span data-ttu-id="3d58b-140">DateTime</span><span class="sxs-lookup"><span data-stu-id="3d58b-140">datetime</span></span>|<span data-ttu-id="3d58b-141">O último DateTime que o país/região foi modificado.</span><span class="sxs-lookup"><span data-stu-id="3d58b-141">The last datetime the country/region was modified.</span></span> <span data-ttu-id="3d58b-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3d58b-142">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="3d58b-143">Relações</span><span class="sxs-lookup"><span data-stu-id="3d58b-143">Relationships</span></span>
<span data-ttu-id="3d58b-144">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3d58b-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d58b-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d58b-145">JSON representation</span></span>

<span data-ttu-id="3d58b-146">Veja a seguir uma representação JSON do countriesRegions.</span><span class="sxs-lookup"><span data-stu-id="3d58b-146">Here is a JSON representation of the countriesRegions.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "addressFormat": "string",
  "lastModifiedDateTime": "datetime"
}

```


