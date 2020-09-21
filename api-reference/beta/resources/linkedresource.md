---
title: tipo de recurso linkedResource
description: Representa a fonte do todoTask
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3cbfaa0bf809a1996fe7a7c7df7014324406bcf2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058106"
---
# <a name="linkedresource-resource-type"></a><span data-ttu-id="1ab2e-103">tipo de recurso linkedResource</span><span class="sxs-lookup"><span data-stu-id="1ab2e-103">linkedResource resource type</span></span>

<span data-ttu-id="1ab2e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ab2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ab2e-105">Representa um item em um aplicativo parceiro relacionado a um [todoTask](./todotask.md).</span><span class="sxs-lookup"><span data-stu-id="1ab2e-105">Represents an item in a partner application related to a [todoTask](./todotask.md).</span></span> <span data-ttu-id="1ab2e-106">Um exemplo é um email que criou a tarefa.</span><span class="sxs-lookup"><span data-stu-id="1ab2e-106">An example is an email that created the task.</span></span> <span data-ttu-id="1ab2e-107">Um objeto **linkedResource** armazena informações sobre esse aplicativo de origem e permite que você vincule novamente ao item relacionado.</span><span class="sxs-lookup"><span data-stu-id="1ab2e-107">A **linkedResource** object stores information about that source application, and lets you link back to the related item.</span></span>

## <a name="methods"></a><span data-ttu-id="1ab2e-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="1ab2e-108">Methods</span></span>
|<span data-ttu-id="1ab2e-109">Método</span><span class="sxs-lookup"><span data-stu-id="1ab2e-109">Method</span></span>|<span data-ttu-id="1ab2e-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1ab2e-110">Return type</span></span>|<span data-ttu-id="1ab2e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ab2e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1ab2e-112">Listar linkedResources</span><span class="sxs-lookup"><span data-stu-id="1ab2e-112">List linkedResources</span></span>](../api/todotask-list-linkedresources.md)|<span data-ttu-id="1ab2e-113">coleção [linkedResource](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="1ab2e-113">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="1ab2e-114">Obtenha o linkedResources da propriedade de navegação linkedResources.</span><span class="sxs-lookup"><span data-stu-id="1ab2e-114">Get the linkedResources from the linkedResources navigation property.</span></span>|
|[<span data-ttu-id="1ab2e-115">Criar linkedResource</span><span class="sxs-lookup"><span data-stu-id="1ab2e-115">Create linkedResource</span></span>](../api/todotask-post-linkedresources.md)|[<span data-ttu-id="1ab2e-116">linkedResource</span><span class="sxs-lookup"><span data-stu-id="1ab2e-116">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="1ab2e-117">Criar um novo objeto linkedResources.</span><span class="sxs-lookup"><span data-stu-id="1ab2e-117">Create a new linkedResources object.</span></span>|
|[<span data-ttu-id="1ab2e-118">Obter linkedResource</span><span class="sxs-lookup"><span data-stu-id="1ab2e-118">Get linkedResource</span></span>](../api/linkedresource-get.md)|[<span data-ttu-id="1ab2e-119">linkedResource</span><span class="sxs-lookup"><span data-stu-id="1ab2e-119">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="1ab2e-120">Leia as propriedades e os relacionamentos de um objeto [linkedResource](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="1ab2e-120">Read the properties and relationships of a [linkedResource](../resources/linkedresource.md) object.</span></span>|
|[<span data-ttu-id="1ab2e-121">Atualizar linkedResource</span><span class="sxs-lookup"><span data-stu-id="1ab2e-121">Update linkedResource</span></span>](../api/linkedresource-update.md)|[<span data-ttu-id="1ab2e-122">linkedResource</span><span class="sxs-lookup"><span data-stu-id="1ab2e-122">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="1ab2e-123">Atualiza as propriedades de um objeto [linkedResource](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="1ab2e-123">Update the properties of a [linkedResource](../resources/linkedresource.md) object.</span></span>|
|[<span data-ttu-id="1ab2e-124">Excluir linkedResource</span><span class="sxs-lookup"><span data-stu-id="1ab2e-124">Delete linkedResource</span></span>](../api/linkedresource-delete.md)|<span data-ttu-id="1ab2e-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1ab2e-125">None</span></span>|<span data-ttu-id="1ab2e-126">Exclui um objeto [linkedResource](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="1ab2e-126">Deletes a [linkedResource](../resources/linkedresource.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1ab2e-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ab2e-127">Properties</span></span>
|<span data-ttu-id="1ab2e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ab2e-128">Property</span></span>|<span data-ttu-id="1ab2e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ab2e-129">Type</span></span>|<span data-ttu-id="1ab2e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ab2e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ab2e-131">applicationName</span><span class="sxs-lookup"><span data-stu-id="1ab2e-131">applicationName</span></span>|<span data-ttu-id="1ab2e-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ab2e-132">String</span></span>|<span data-ttu-id="1ab2e-133">Campo que indica o nome do aplicativo de origem que está enviando o **linkedResource**.</span><span class="sxs-lookup"><span data-stu-id="1ab2e-133">Field indicating the app name of the source that is sending the **linkedResource**.</span></span>|
|<span data-ttu-id="1ab2e-134">displayName</span><span class="sxs-lookup"><span data-stu-id="1ab2e-134">displayName</span></span>|<span data-ttu-id="1ab2e-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ab2e-135">String</span></span>|<span data-ttu-id="1ab2e-136">Campo que indica o título do **linkedResource**.</span><span class="sxs-lookup"><span data-stu-id="1ab2e-136">Field indicating the title of the **linkedResource**.</span></span>|
|<span data-ttu-id="1ab2e-137">externalId</span><span class="sxs-lookup"><span data-stu-id="1ab2e-137">externalId</span></span>|<span data-ttu-id="1ab2e-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ab2e-138">String</span></span>|<span data-ttu-id="1ab2e-139">ID do objeto que está associado a essa tarefa no sistema de parceiros ou de terceiros.</span><span class="sxs-lookup"><span data-stu-id="1ab2e-139">Id of the object that is associated with this task on the third-party/partner system.</span></span>|
|<span data-ttu-id="1ab2e-140">id</span><span class="sxs-lookup"><span data-stu-id="1ab2e-140">id</span></span>|<span data-ttu-id="1ab2e-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ab2e-141">String</span></span>|<span data-ttu-id="1ab2e-142">ID gerada pelo servidor para o **linkedResource**.</span><span class="sxs-lookup"><span data-stu-id="1ab2e-142">Server generated ID for the **linkedResource**.</span></span> <span data-ttu-id="1ab2e-143">Herdado de [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="1ab2e-143">Inherited from [entity](../resources/entity.md).</span></span>|
|<span data-ttu-id="1ab2e-144">webUrl</span><span class="sxs-lookup"><span data-stu-id="1ab2e-144">webUrl</span></span>|<span data-ttu-id="1ab2e-145">String</span><span class="sxs-lookup"><span data-stu-id="1ab2e-145">String</span></span>|<span data-ttu-id="1ab2e-146">Link profundo para o **linkedResource**.</span><span class="sxs-lookup"><span data-stu-id="1ab2e-146">Deep link to the **linkedResource**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ab2e-147">Relações</span><span class="sxs-lookup"><span data-stu-id="1ab2e-147">Relationships</span></span>
<span data-ttu-id="1ab2e-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1ab2e-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ab2e-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ab2e-149">JSON representation</span></span>
<span data-ttu-id="1ab2e-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ab2e-150">The following is a JSON representation of the resource.</span></span>
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



