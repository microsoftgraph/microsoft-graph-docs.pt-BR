---
title: tipo de recurso publishedResource
description: tipo de recurso publishedResource.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7b6f81f9e3a6b399f7e029e21330fe83b533af87
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521289"
---
# <a name="publishedresource-resource-type"></a><span data-ttu-id="7479a-103">tipo de recurso publishedResource</span><span class="sxs-lookup"><span data-stu-id="7479a-103">publishedResource resource type</span></span>

<span data-ttu-id="7479a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7479a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7479a-105">Representa o recurso publicado no local.</span><span class="sxs-lookup"><span data-stu-id="7479a-105">Represents on-premises published resource.</span></span> <span data-ttu-id="7479a-106">Um administrador de locatários pode publicar vários tipos de recursos locais-aplicativos corporativos, controladores de domínio, servidores, etc. [os agentes locais](onpremisesagent.md) instalados por um administrador de locatários podem ser configurados para acessar/lidar com solicitações de um recurso publicado específico.</span><span class="sxs-lookup"><span data-stu-id="7479a-106">A tenant administrator could publish various types of on-premises resources - enterprise applications, domain controllers, servers, etc. [On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular published resource.</span></span>

## <a name="methods"></a><span data-ttu-id="7479a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="7479a-107">Methods</span></span>

| <span data-ttu-id="7479a-108">Método</span><span class="sxs-lookup"><span data-stu-id="7479a-108">Method</span></span>       | <span data-ttu-id="7479a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7479a-109">Return Type</span></span> | <span data-ttu-id="7479a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7479a-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7479a-111">Listar publishedResources</span><span class="sxs-lookup"><span data-stu-id="7479a-111">List publishedResources</span></span>](../api/publishedresource-list.md) | <span data-ttu-id="7479a-112">coleção Objects [publishedResource](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="7479a-112">[publishedResource](publishedresource.md) objects collection</span></span> | <span data-ttu-id="7479a-113">Obtenha uma coleção de objetos **publishedResources** .</span><span class="sxs-lookup"><span data-stu-id="7479a-113">Get a **publishedResources** object collection.</span></span> |
| [<span data-ttu-id="7479a-114">Obter publishedResource</span><span class="sxs-lookup"><span data-stu-id="7479a-114">Get publishedResource</span></span>](../api/publishedresource-get.md) | [<span data-ttu-id="7479a-115">publishedResource</span><span class="sxs-lookup"><span data-stu-id="7479a-115">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="7479a-116">Leia as propriedades e os relacionamentos de um objeto **publishedResource** .</span><span class="sxs-lookup"><span data-stu-id="7479a-116">Read the properties and relationships of a **publishedResource** object.</span></span> |
| [<span data-ttu-id="7479a-117">Criar publishedResource</span><span class="sxs-lookup"><span data-stu-id="7479a-117">Create publishedResource</span></span>](../api/publishedresource-post.md) |  [<span data-ttu-id="7479a-118">publishedResource</span><span class="sxs-lookup"><span data-stu-id="7479a-118">publishedResource</span></span>](publishedresource.md)  | <span data-ttu-id="7479a-119">Criar um novo **publishedResource**.</span><span class="sxs-lookup"><span data-stu-id="7479a-119">Create a new **publishedResource**.</span></span> |
| [<span data-ttu-id="7479a-120">Atualizar publishedResource</span><span class="sxs-lookup"><span data-stu-id="7479a-120">Update publishedResource</span></span>](../api/publishedresource-update.md) | [<span data-ttu-id="7479a-121">publishedResource</span><span class="sxs-lookup"><span data-stu-id="7479a-121">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="7479a-122">Atualizar um objeto **publishedResource** .</span><span class="sxs-lookup"><span data-stu-id="7479a-122">Update a **publishedResource** object.</span></span> |
| [<span data-ttu-id="7479a-123">Excluir publishedResource</span><span class="sxs-lookup"><span data-stu-id="7479a-123">Delete  publishedResource</span></span>](../api/publishedresource-delete.md) | <span data-ttu-id="7479a-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7479a-124">None</span></span> | <span data-ttu-id="7479a-125">Excluir um objeto **publishedResource** .</span><span class="sxs-lookup"><span data-stu-id="7479a-125">Delete a **publishedResource** object.</span></span> |
| [<span data-ttu-id="7479a-126">Atribuir publishedResource a onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="7479a-126">Assign publishedResource to onPremisesAgentGroup</span></span>](../api/publishedresource-post-agentgroups.md) | <span data-ttu-id="7479a-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7479a-127">None</span></span> | <span data-ttu-id="7479a-128">Atribua um objeto **publishedResource** a um **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="7479a-128">Assign a **publishedResource** object to an **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="7479a-129">Remover o publishedResource do onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="7479a-129">Remove publishedResource from onPremisesAgentGroup</span></span>](../api/publishedresource-delete-agentgroups.md) | <span data-ttu-id="7479a-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7479a-130">None</span></span> |  <span data-ttu-id="7479a-131">Remover um objeto **publishedResource** de um **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="7479a-131">Remove a **publishedResource** object from an **onPremisesAgentGroup**.</span></span>|

## <a name="properties"></a><span data-ttu-id="7479a-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7479a-132">Properties</span></span>

| <span data-ttu-id="7479a-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7479a-133">Property</span></span>     | <span data-ttu-id="7479a-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="7479a-134">Type</span></span>        | <span data-ttu-id="7479a-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="7479a-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7479a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7479a-136">displayName</span></span>|<span data-ttu-id="7479a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7479a-137">String</span></span>| <span data-ttu-id="7479a-138">Nome para exibição do publishedResource.</span><span class="sxs-lookup"><span data-stu-id="7479a-138">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="7479a-139">id</span><span class="sxs-lookup"><span data-stu-id="7479a-139">id</span></span>|<span data-ttu-id="7479a-140">String</span><span class="sxs-lookup"><span data-stu-id="7479a-140">String</span></span>| <span data-ttu-id="7479a-141">A ID de objeto do publishedResource.</span><span class="sxs-lookup"><span data-stu-id="7479a-141">The object id of the publishedResource.</span></span> <span data-ttu-id="7479a-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7479a-142">Read-only.</span></span>|
|<span data-ttu-id="7479a-143">publishingtype</span><span class="sxs-lookup"><span data-stu-id="7479a-143">publishingType</span></span>|<span data-ttu-id="7479a-144">string</span><span class="sxs-lookup"><span data-stu-id="7479a-144">string</span></span>| <span data-ttu-id="7479a-145">Os valores possíveis são: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="7479a-145">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|
|<span data-ttu-id="7479a-146">resourceName</span><span class="sxs-lookup"><span data-stu-id="7479a-146">resourceName</span></span>|<span data-ttu-id="7479a-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7479a-147">String</span></span>|<span data-ttu-id="7479a-148">Nome do publishedResource.</span><span class="sxs-lookup"><span data-stu-id="7479a-148">Name of the publishedResource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7479a-149">Relações</span><span class="sxs-lookup"><span data-stu-id="7479a-149">Relationships</span></span>

| <span data-ttu-id="7479a-150">Relação</span><span class="sxs-lookup"><span data-stu-id="7479a-150">Relationship</span></span> | <span data-ttu-id="7479a-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="7479a-151">Type</span></span>        | <span data-ttu-id="7479a-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="7479a-152">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7479a-153">agentGroups</span><span class="sxs-lookup"><span data-stu-id="7479a-153">agentGroups</span></span>|<span data-ttu-id="7479a-154">coleção [onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="7479a-154">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="7479a-155">Lista de **onPremisesAgentGroups** aos quais um **publishedResource** é atribuído.</span><span class="sxs-lookup"><span data-stu-id="7479a-155">List of **onPremisesAgentGroups** that a **publishedResource** is assigned to.</span></span> <span data-ttu-id="7479a-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7479a-156">Read-only.</span></span> <span data-ttu-id="7479a-157">Anulável.</span><span class="sxs-lookup"><span data-stu-id="7479a-157">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7479a-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7479a-158">JSON representation</span></span>

<span data-ttu-id="7479a-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7479a-159">The following is a JSON representation of the resource.</span></span>

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
