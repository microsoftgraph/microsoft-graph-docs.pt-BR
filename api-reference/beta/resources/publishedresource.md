---
title: tipo de recurso publishedResource
description: tipo de recurso publishedResource.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d42464fa6e249fef8d7b535b6327751f48d17167
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556321"
---
# <a name="publishedresource-resource-type"></a><span data-ttu-id="5da76-103">tipo de recurso publishedResource</span><span class="sxs-lookup"><span data-stu-id="5da76-103">publishedResource resource type</span></span>

<span data-ttu-id="5da76-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5da76-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5da76-105">Representa o recurso publicado no local.</span><span class="sxs-lookup"><span data-stu-id="5da76-105">Represents on-premises published resource.</span></span> <span data-ttu-id="5da76-106">Um administrador de locatários pode publicar vários tipos de recursos locais-aplicativos corporativos, controladores de domínio, servidores, etc. [os agentes locais](onpremisesagent.md) instalados por um administrador de locatários podem ser configurados para acessar/lidar com solicitações de um recurso publicado específico.</span><span class="sxs-lookup"><span data-stu-id="5da76-106">A tenant administrator can publish various types of on-premises resources - enterprise applications, domain controllers, servers, etc. [On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular published resource.</span></span>

## <a name="methods"></a><span data-ttu-id="5da76-107">Methods</span><span class="sxs-lookup"><span data-stu-id="5da76-107">Methods</span></span>

| <span data-ttu-id="5da76-108">Método</span><span class="sxs-lookup"><span data-stu-id="5da76-108">Method</span></span>       | <span data-ttu-id="5da76-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5da76-109">Return Type</span></span> | <span data-ttu-id="5da76-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5da76-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5da76-111">Listar publishedResources</span><span class="sxs-lookup"><span data-stu-id="5da76-111">List publishedResources</span></span>](../api/publishedresource-list.md) | <span data-ttu-id="5da76-112">coleção Objects [publishedResource](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="5da76-112">[publishedResource](publishedresource.md) objects collection</span></span> | <span data-ttu-id="5da76-113">Obtenha uma coleção de objetos **publishedResources** .</span><span class="sxs-lookup"><span data-stu-id="5da76-113">Get a **publishedResources** object collection.</span></span> |
| [<span data-ttu-id="5da76-114">Obter publishedResource</span><span class="sxs-lookup"><span data-stu-id="5da76-114">Get publishedResource</span></span>](../api/publishedresource-get.md) | [<span data-ttu-id="5da76-115">publishedResource</span><span class="sxs-lookup"><span data-stu-id="5da76-115">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="5da76-116">Leia as propriedades e os relacionamentos de um objeto **publishedResource** .</span><span class="sxs-lookup"><span data-stu-id="5da76-116">Read the properties and relationships of a **publishedResource** object.</span></span> |
| [<span data-ttu-id="5da76-117">Criar publishedResource</span><span class="sxs-lookup"><span data-stu-id="5da76-117">Create publishedResource</span></span>](../api/publishedresource-post.md) |  [<span data-ttu-id="5da76-118">publishedResource</span><span class="sxs-lookup"><span data-stu-id="5da76-118">publishedResource</span></span>](publishedresource.md)  | <span data-ttu-id="5da76-119">Criar um novo **publishedResource**.</span><span class="sxs-lookup"><span data-stu-id="5da76-119">Create a new **publishedResource**.</span></span> |
| [<span data-ttu-id="5da76-120">Atualizar publishedResource</span><span class="sxs-lookup"><span data-stu-id="5da76-120">Update publishedResource</span></span>](../api/publishedresource-update.md) | [<span data-ttu-id="5da76-121">publishedResource</span><span class="sxs-lookup"><span data-stu-id="5da76-121">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="5da76-122">Atualizar um objeto **publishedResource** .</span><span class="sxs-lookup"><span data-stu-id="5da76-122">Update a **publishedResource** object.</span></span> |
| [<span data-ttu-id="5da76-123">Excluir publishedResource</span><span class="sxs-lookup"><span data-stu-id="5da76-123">Delete  publishedResource</span></span>](../api/publishedresource-delete.md) | <span data-ttu-id="5da76-124">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="5da76-124">None</span></span> | <span data-ttu-id="5da76-125">Excluir um objeto **publishedResource** .</span><span class="sxs-lookup"><span data-stu-id="5da76-125">Delete a **publishedResource** object.</span></span> |
| [<span data-ttu-id="5da76-126">Atribuir publishedResource a onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="5da76-126">Assign publishedResource to onPremisesAgentGroup</span></span>](../api/publishedresource-post-agentgroups.md) | <span data-ttu-id="5da76-127">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="5da76-127">None</span></span> | <span data-ttu-id="5da76-128">Atribua um objeto **publishedResource** a um **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="5da76-128">Assign a **publishedResource** object to an **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="5da76-129">Remover o publishedResource do onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="5da76-129">Remove publishedResource from onPremisesAgentGroup</span></span>](../api/publishedresource-delete-agentgroups.md) | <span data-ttu-id="5da76-130">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="5da76-130">None</span></span> |  <span data-ttu-id="5da76-131">Remover um objeto **publishedResource** de um **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="5da76-131">Remove a **publishedResource** object from an **onPremisesAgentGroup**.</span></span>|

## <a name="properties"></a><span data-ttu-id="5da76-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5da76-132">Properties</span></span>

| <span data-ttu-id="5da76-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5da76-133">Property</span></span>     | <span data-ttu-id="5da76-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="5da76-134">Type</span></span>        | <span data-ttu-id="5da76-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="5da76-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5da76-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5da76-136">displayName</span></span>|<span data-ttu-id="5da76-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5da76-137">String</span></span>| <span data-ttu-id="5da76-138">Nome para exibição do publishedResource.</span><span class="sxs-lookup"><span data-stu-id="5da76-138">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="5da76-139">id</span><span class="sxs-lookup"><span data-stu-id="5da76-139">id</span></span>|<span data-ttu-id="5da76-140">String</span><span class="sxs-lookup"><span data-stu-id="5da76-140">String</span></span>| <span data-ttu-id="5da76-141">A ID de objeto do publishedResource.</span><span class="sxs-lookup"><span data-stu-id="5da76-141">The object id of the publishedResource.</span></span> <span data-ttu-id="5da76-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5da76-142">Read-only.</span></span>|
|<span data-ttu-id="5da76-143">publishingtype</span><span class="sxs-lookup"><span data-stu-id="5da76-143">publishingType</span></span>|<span data-ttu-id="5da76-144">string</span><span class="sxs-lookup"><span data-stu-id="5da76-144">string</span></span>| <span data-ttu-id="5da76-145">Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="5da76-145">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|
|<span data-ttu-id="5da76-146">resourceName</span><span class="sxs-lookup"><span data-stu-id="5da76-146">resourceName</span></span>|<span data-ttu-id="5da76-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5da76-147">String</span></span>|<span data-ttu-id="5da76-148">Nome do publishedResource.</span><span class="sxs-lookup"><span data-stu-id="5da76-148">Name of the publishedResource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5da76-149">Relações</span><span class="sxs-lookup"><span data-stu-id="5da76-149">Relationships</span></span>

| <span data-ttu-id="5da76-150">Relação</span><span class="sxs-lookup"><span data-stu-id="5da76-150">Relationship</span></span> | <span data-ttu-id="5da76-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="5da76-151">Type</span></span>        | <span data-ttu-id="5da76-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="5da76-152">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5da76-153">agentGroups</span><span class="sxs-lookup"><span data-stu-id="5da76-153">agentGroups</span></span>|<span data-ttu-id="5da76-154">coleção [onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="5da76-154">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="5da76-155">Lista de **onPremisesAgentGroups** aos quais um **publishedResource** é atribuído.</span><span class="sxs-lookup"><span data-stu-id="5da76-155">List of **onPremisesAgentGroups** that a **publishedResource** is assigned to.</span></span> <span data-ttu-id="5da76-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5da76-156">Read-only.</span></span> <span data-ttu-id="5da76-157">Anulável.</span><span class="sxs-lookup"><span data-stu-id="5da76-157">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5da76-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5da76-158">JSON representation</span></span>

<span data-ttu-id="5da76-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5da76-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publishedResource",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "publishingType": "string",
  "resourceName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "publishedResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
