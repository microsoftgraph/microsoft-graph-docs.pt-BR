---
title: tipo de recurso linkedResource
description: Representa a fonte do todoTask
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 102b7a918d7f6dbd76db42b738a741b9797aeafb
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313482"
---
# <a name="linkedresource-resource-type"></a><span data-ttu-id="131f5-103">tipo de recurso linkedResource</span><span class="sxs-lookup"><span data-stu-id="131f5-103">linkedResource resource type</span></span>

<span data-ttu-id="131f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="131f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="131f5-105">Representa um item em um aplicativo parceiro relacionado a um [todoTask](./todotask.md).</span><span class="sxs-lookup"><span data-stu-id="131f5-105">Represents an item in a partner application related to a [todoTask](./todotask.md).</span></span> <span data-ttu-id="131f5-106">Um exemplo é um email de onde a tarefa foi criada.</span><span class="sxs-lookup"><span data-stu-id="131f5-106">An example is an email from where the task was created.</span></span> <span data-ttu-id="131f5-107">Um objeto **linkedResource** armazena informações sobre esse aplicativo de origem e permite que você vincule novamente ao item relacionado.</span><span class="sxs-lookup"><span data-stu-id="131f5-107">A **linkedResource** object stores information about that source application, and lets you link back to the related item.</span></span> <span data-ttu-id="131f5-108">Você pode ver o **linkedResource** no modo de exibição detalhes da tarefa, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="131f5-108">You can see the **linkedResource** in the task details view, as shown.</span></span>

![Recurso vinculado no painel de detalhes da tarefa](/graph/images/todo-linkedresource-taskdetail.png)

<span data-ttu-id="131f5-110">Alguns objetos **linkedResource** não estão associados a qualquer URL da Web, e nesse caso, a propriedade **WebUrl** não é necessária.</span><span class="sxs-lookup"><span data-stu-id="131f5-110">Some **linkedResource** objects are not associated with any web URLs, in which case, the **webUrl** property is not required.</span></span> <span data-ttu-id="131f5-111">Por exemplo, o item vinculado pode ser de um aplicativo de negócios personalizado ou de uma plataforma nativa, como um aplicativo do SMS em um telefone celular.</span><span class="sxs-lookup"><span data-stu-id="131f5-111">For example, the linked item can be from a custom business app or native platform app, such as an SMS app on a mobile phone.</span></span> <span data-ttu-id="131f5-112">Veja como um **linkedResource** aparece com e sem uma URL.</span><span class="sxs-lookup"><span data-stu-id="131f5-112">Here is how a **linkedResource** appears with and without a URL.</span></span>

![Recurso vinculado com e sem URL](/graph/images/todo-linkedresource.png)

## <a name="methods"></a><span data-ttu-id="131f5-114">Métodos</span><span class="sxs-lookup"><span data-stu-id="131f5-114">Methods</span></span>
|<span data-ttu-id="131f5-115">Método</span><span class="sxs-lookup"><span data-stu-id="131f5-115">Method</span></span>|<span data-ttu-id="131f5-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="131f5-116">Return type</span></span>|<span data-ttu-id="131f5-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="131f5-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="131f5-118">Listar linkedResources</span><span class="sxs-lookup"><span data-stu-id="131f5-118">List linkedResources</span></span>](../api/todotask-list-linkedresources.md)|<span data-ttu-id="131f5-119">coleção [linkedResource](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="131f5-119">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="131f5-120">Obtenha o linkedResources da propriedade de navegação linkedResources.</span><span class="sxs-lookup"><span data-stu-id="131f5-120">Get the linkedResources from the linkedResources navigation property.</span></span>|
|[<span data-ttu-id="131f5-121">Criar linkedResource</span><span class="sxs-lookup"><span data-stu-id="131f5-121">Create linkedResource</span></span>](../api/todotask-post-linkedresources.md)|[<span data-ttu-id="131f5-122">linkedResource</span><span class="sxs-lookup"><span data-stu-id="131f5-122">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="131f5-123">Criar um novo objeto linkedResources.</span><span class="sxs-lookup"><span data-stu-id="131f5-123">Create a new linkedResources object.</span></span>|
|[<span data-ttu-id="131f5-124">Obter linkedResource</span><span class="sxs-lookup"><span data-stu-id="131f5-124">Get linkedResource</span></span>](../api/linkedresource-get.md)|[<span data-ttu-id="131f5-125">linkedResource</span><span class="sxs-lookup"><span data-stu-id="131f5-125">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="131f5-126">Leia as propriedades e os relacionamentos de um objeto [linkedResource](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="131f5-126">Read the properties and relationships of a [linkedResource](../resources/linkedresource.md) object.</span></span>|
|[<span data-ttu-id="131f5-127">Atualizar linkedResource</span><span class="sxs-lookup"><span data-stu-id="131f5-127">Update linkedResource</span></span>](../api/linkedresource-update.md)|[<span data-ttu-id="131f5-128">linkedResource</span><span class="sxs-lookup"><span data-stu-id="131f5-128">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="131f5-129">Atualiza as propriedades de um objeto [linkedResource](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="131f5-129">Update the properties of a [linkedResource](../resources/linkedresource.md) object.</span></span>|
|[<span data-ttu-id="131f5-130">Excluir linkedResource</span><span class="sxs-lookup"><span data-stu-id="131f5-130">Delete linkedResource</span></span>](../api/linkedresource-delete.md)|<span data-ttu-id="131f5-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="131f5-131">None</span></span>|<span data-ttu-id="131f5-132">Exclui um objeto [linkedResource](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="131f5-132">Deletes a [linkedResource](../resources/linkedresource.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="131f5-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="131f5-133">Properties</span></span>
|<span data-ttu-id="131f5-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="131f5-134">Property</span></span>|<span data-ttu-id="131f5-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="131f5-135">Type</span></span>|<span data-ttu-id="131f5-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="131f5-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="131f5-137">applicationName</span><span class="sxs-lookup"><span data-stu-id="131f5-137">applicationName</span></span>|<span data-ttu-id="131f5-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="131f5-138">String</span></span>|<span data-ttu-id="131f5-139">Campo que indica o nome do aplicativo de origem que está enviando o **linkedResource**.</span><span class="sxs-lookup"><span data-stu-id="131f5-139">Field indicating the app name of the source that is sending the **linkedResource**.</span></span>|
|<span data-ttu-id="131f5-140">displayName</span><span class="sxs-lookup"><span data-stu-id="131f5-140">displayName</span></span>|<span data-ttu-id="131f5-141">String</span><span class="sxs-lookup"><span data-stu-id="131f5-141">String</span></span>|<span data-ttu-id="131f5-142">Campo que indica o título do **linkedResource**.</span><span class="sxs-lookup"><span data-stu-id="131f5-142">Field indicating the title of the **linkedResource**.</span></span>|
|<span data-ttu-id="131f5-143">externalId</span><span class="sxs-lookup"><span data-stu-id="131f5-143">externalId</span></span>|<span data-ttu-id="131f5-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="131f5-144">String</span></span>|<span data-ttu-id="131f5-145">ID do objeto que está associado a essa tarefa no sistema de parceiros ou de terceiros.</span><span class="sxs-lookup"><span data-stu-id="131f5-145">Id of the object that is associated with this task on the third-party/partner system.</span></span>|
|<span data-ttu-id="131f5-146">id</span><span class="sxs-lookup"><span data-stu-id="131f5-146">id</span></span>|<span data-ttu-id="131f5-147">String</span><span class="sxs-lookup"><span data-stu-id="131f5-147">String</span></span>|<span data-ttu-id="131f5-148">ID gerada pelo servidor para o **linkedResource**.</span><span class="sxs-lookup"><span data-stu-id="131f5-148">Server generated ID for the **linkedResource**.</span></span> <span data-ttu-id="131f5-149">Herdado de [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="131f5-149">Inherited from [entity](../resources/entity.md).</span></span>|
|<span data-ttu-id="131f5-150">webUrl</span><span class="sxs-lookup"><span data-stu-id="131f5-150">webUrl</span></span>|<span data-ttu-id="131f5-151">String</span><span class="sxs-lookup"><span data-stu-id="131f5-151">String</span></span>|<span data-ttu-id="131f5-152">Link profundo para o **linkedResource**.</span><span class="sxs-lookup"><span data-stu-id="131f5-152">Deep link to the **linkedResource**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="131f5-153">Relações</span><span class="sxs-lookup"><span data-stu-id="131f5-153">Relationships</span></span>
<span data-ttu-id="131f5-154">Nenhum</span><span class="sxs-lookup"><span data-stu-id="131f5-154">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="131f5-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="131f5-155">JSON representation</span></span>
<span data-ttu-id="131f5-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="131f5-156">The following is a JSON representation of the resource.</span></span>
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



