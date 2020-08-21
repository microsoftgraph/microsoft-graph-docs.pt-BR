---
title: tipo de recurso linkedResource
description: Representa a fonte do todoTask
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0a386cd8ed714a6f7127ea0a872a4170997bb8b9
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849861"
---
# <a name="linkedresource-resource-type"></a><span data-ttu-id="d4338-103">tipo de recurso linkedResource</span><span class="sxs-lookup"><span data-stu-id="d4338-103">linkedResource resource type</span></span>

<span data-ttu-id="d4338-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4338-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4338-105">Representa um item em um aplicativo parceiro relacionado a um [todoTask](./todotask.md).</span><span class="sxs-lookup"><span data-stu-id="d4338-105">Represents an item in a partner application related to a [todoTask](./todotask.md).</span></span> <span data-ttu-id="d4338-106">Um exemplo é um email que criou a tarefa.</span><span class="sxs-lookup"><span data-stu-id="d4338-106">An example is an email that created the task.</span></span> <span data-ttu-id="d4338-107">Um objeto **linkedResource** armazena informações sobre esse aplicativo de origem e permite que você vincule novamente ao item relacionado.</span><span class="sxs-lookup"><span data-stu-id="d4338-107">A **linkedResource** object stores information about that source application, and lets you link back to the related item.</span></span>

## <a name="methods"></a><span data-ttu-id="d4338-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="d4338-108">Methods</span></span>
|<span data-ttu-id="d4338-109">Método</span><span class="sxs-lookup"><span data-stu-id="d4338-109">Method</span></span>|<span data-ttu-id="d4338-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d4338-110">Return type</span></span>|<span data-ttu-id="d4338-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4338-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d4338-112">Listar linkedResources</span><span class="sxs-lookup"><span data-stu-id="d4338-112">List linkedResources</span></span>](../api/todotask-list-linkedresources.md)|<span data-ttu-id="d4338-113">coleção [linkedResource](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="d4338-113">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="d4338-114">Obtenha o linkedResources da propriedade de navegação linkedResources.</span><span class="sxs-lookup"><span data-stu-id="d4338-114">Get the linkedResources from the linkedResources navigation property.</span></span>|
|[<span data-ttu-id="d4338-115">Criar linkedResource</span><span class="sxs-lookup"><span data-stu-id="d4338-115">Create linkedResource</span></span>](../api/todotask-post-linkedresources.md)|[<span data-ttu-id="d4338-116">linkedResource</span><span class="sxs-lookup"><span data-stu-id="d4338-116">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="d4338-117">Criar um novo objeto linkedResources.</span><span class="sxs-lookup"><span data-stu-id="d4338-117">Create a new linkedResources object.</span></span>|
|[<span data-ttu-id="d4338-118">Obter linkedResource</span><span class="sxs-lookup"><span data-stu-id="d4338-118">Get linkedResource</span></span>](../api/linkedresource-get.md)|[<span data-ttu-id="d4338-119">linkedResource</span><span class="sxs-lookup"><span data-stu-id="d4338-119">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="d4338-120">Leia as propriedades e os relacionamentos de um objeto [linkedResource](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="d4338-120">Read the properties and relationships of a [linkedResource](../resources/linkedresource.md) object.</span></span>|
|[<span data-ttu-id="d4338-121">Atualizar linkedResource</span><span class="sxs-lookup"><span data-stu-id="d4338-121">Update linkedResource</span></span>](../api/linkedresource-update.md)|[<span data-ttu-id="d4338-122">linkedResource</span><span class="sxs-lookup"><span data-stu-id="d4338-122">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="d4338-123">Atualiza as propriedades de um objeto [linkedResource](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="d4338-123">Update the properties of a [linkedResource](../resources/linkedresource.md) object.</span></span>|
|[<span data-ttu-id="d4338-124">Excluir linkedResource</span><span class="sxs-lookup"><span data-stu-id="d4338-124">Delete linkedResource</span></span>](../api/linkedresource-delete.md)|<span data-ttu-id="d4338-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d4338-125">None</span></span>|<span data-ttu-id="d4338-126">Exclui um objeto [linkedResource](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="d4338-126">Deletes a [linkedResource](../resources/linkedresource.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d4338-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d4338-127">Properties</span></span>
|<span data-ttu-id="d4338-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4338-128">Property</span></span>|<span data-ttu-id="d4338-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4338-129">Type</span></span>|<span data-ttu-id="d4338-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4338-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4338-131">applicationName</span><span class="sxs-lookup"><span data-stu-id="d4338-131">applicationName</span></span>|<span data-ttu-id="d4338-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4338-132">String</span></span>|<span data-ttu-id="d4338-133">Campo que indica o nome do aplicativo de origem que está enviando o **linkedResource**.</span><span class="sxs-lookup"><span data-stu-id="d4338-133">Field indicating the app name of the source that is sending the **linkedResource**.</span></span>|
|<span data-ttu-id="d4338-134">displayName</span><span class="sxs-lookup"><span data-stu-id="d4338-134">displayName</span></span>|<span data-ttu-id="d4338-135">String</span><span class="sxs-lookup"><span data-stu-id="d4338-135">String</span></span>|<span data-ttu-id="d4338-136">Campo que indica o título do **linkedResource**.</span><span class="sxs-lookup"><span data-stu-id="d4338-136">Field indicating the title of the **linkedResource**.</span></span>|
|<span data-ttu-id="d4338-137">externalId</span><span class="sxs-lookup"><span data-stu-id="d4338-137">externalId</span></span>|<span data-ttu-id="d4338-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4338-138">String</span></span>|<span data-ttu-id="d4338-139">ID do objeto que está associado a essa tarefa no sistema de parceiros ou de terceiros.</span><span class="sxs-lookup"><span data-stu-id="d4338-139">Id of the object that is associated with this task on the third-party/partner system.</span></span>|
|<span data-ttu-id="d4338-140">id</span><span class="sxs-lookup"><span data-stu-id="d4338-140">id</span></span>|<span data-ttu-id="d4338-141">String</span><span class="sxs-lookup"><span data-stu-id="d4338-141">String</span></span>|<span data-ttu-id="d4338-142">ID gerada pelo servidor para o **linkedResource**.</span><span class="sxs-lookup"><span data-stu-id="d4338-142">Server generated ID for the **linkedResource**.</span></span> <span data-ttu-id="d4338-143">Herdado de [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="d4338-143">Inherited from [entity](../resources/entity.md).</span></span>|
|<span data-ttu-id="d4338-144">webUrl</span><span class="sxs-lookup"><span data-stu-id="d4338-144">webUrl</span></span>|<span data-ttu-id="d4338-145">String</span><span class="sxs-lookup"><span data-stu-id="d4338-145">String</span></span>|<span data-ttu-id="d4338-146">Link profundo para o **linkedResource**.</span><span class="sxs-lookup"><span data-stu-id="d4338-146">Deep link to the **linkedResource**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4338-147">Relações</span><span class="sxs-lookup"><span data-stu-id="d4338-147">Relationships</span></span>
<span data-ttu-id="d4338-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d4338-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4338-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d4338-149">JSON representation</span></span>
<span data-ttu-id="d4338-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d4338-150">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.linkedResource",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.linkedResource",
  "id": "String (identifier)",
  "webUrl": "String",
  "applicationName": "String",
  "displayName": "String",
  "externalId": "String"
}
```

