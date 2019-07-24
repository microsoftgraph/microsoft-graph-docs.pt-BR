---
title: tipo de recurso publishedResource
description: tipo de recurso publishedResource.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 54a2b1b610f30ec3ce7d9853916aad345142cbf0
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841357"
---
# <a name="publishedresource-resource-type"></a><span data-ttu-id="cb40c-103">tipo de recurso publishedResource</span><span class="sxs-lookup"><span data-stu-id="cb40c-103">publishedResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb40c-104">Representa o recurso publicado no local.</span><span class="sxs-lookup"><span data-stu-id="cb40c-104">Represents on-premises published resource.</span></span> <span data-ttu-id="cb40c-105">Um administrador de locatários pode publicar vários tipos de recursos locais-aplicativos corporativos, controladores de domínio, servidores, etc. [os agentes locais](onpremisesagent.md) instalados por um administrador de locatários podem ser configurados para acessar/lidar com solicitações de um recurso publicado específico.</span><span class="sxs-lookup"><span data-stu-id="cb40c-105">A tenant administrator could publish various types of on-premises resources - enterprise applications, domain controllers, servers, etc. [On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular published resource.</span></span>

## <a name="methods"></a><span data-ttu-id="cb40c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="cb40c-106">Methods</span></span>

| <span data-ttu-id="cb40c-107">Método</span><span class="sxs-lookup"><span data-stu-id="cb40c-107">Method</span></span>       | <span data-ttu-id="cb40c-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cb40c-108">Return Type</span></span> | <span data-ttu-id="cb40c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb40c-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cb40c-110">Listar publishedResources</span><span class="sxs-lookup"><span data-stu-id="cb40c-110">List publishedResources</span></span>](../api/publishedresource-list.md) | <span data-ttu-id="cb40c-111">coleção Objects [publishedResource](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="cb40c-111">[publishedResource](publishedresource.md) objects collection</span></span> | <span data-ttu-id="cb40c-112">Obtenha uma coleção de objetos **publishedResources** .</span><span class="sxs-lookup"><span data-stu-id="cb40c-112">Get a **publishedResources** object collection.</span></span> |
| [<span data-ttu-id="cb40c-113">Obter publishedResource</span><span class="sxs-lookup"><span data-stu-id="cb40c-113">Get publishedResource</span></span>](../api/publishedresource-get.md) | [<span data-ttu-id="cb40c-114">publishedResource</span><span class="sxs-lookup"><span data-stu-id="cb40c-114">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="cb40c-115">Leia as propriedades e os relacionamentos de um objeto **publishedResource** .</span><span class="sxs-lookup"><span data-stu-id="cb40c-115">Read the properties and relationships of a **publishedResource** object.</span></span> |
| [<span data-ttu-id="cb40c-116">Criar publishedResource</span><span class="sxs-lookup"><span data-stu-id="cb40c-116">Create publishedResource</span></span>](../api/publishedresource-post.md) |  [<span data-ttu-id="cb40c-117">publishedResource</span><span class="sxs-lookup"><span data-stu-id="cb40c-117">publishedResource</span></span>](publishedresource.md)  | <span data-ttu-id="cb40c-118">Criar um novo **publishedResource**.</span><span class="sxs-lookup"><span data-stu-id="cb40c-118">Create a new **publishedResource**.</span></span> |
| [<span data-ttu-id="cb40c-119">Atualizar publishedResource</span><span class="sxs-lookup"><span data-stu-id="cb40c-119">Update publishedResource</span></span>](../api/publishedresource-update.md) | [<span data-ttu-id="cb40c-120">publishedResource</span><span class="sxs-lookup"><span data-stu-id="cb40c-120">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="cb40c-121">Atualizar um objeto **publishedResource** .</span><span class="sxs-lookup"><span data-stu-id="cb40c-121">Update a **publishedResource** object.</span></span> |
| [<span data-ttu-id="cb40c-122">Excluir publishedResource</span><span class="sxs-lookup"><span data-stu-id="cb40c-122">Delete  publishedResource</span></span>](../api/publishedresource-delete.md) | <span data-ttu-id="cb40c-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb40c-123">None</span></span> | <span data-ttu-id="cb40c-124">Excluir um objeto **publishedResource** .</span><span class="sxs-lookup"><span data-stu-id="cb40c-124">Delete a **publishedResource** object.</span></span> |
| [<span data-ttu-id="cb40c-125">Atribuir publishedResource a onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="cb40c-125">Assign publishedResource to onPremisesAgentGroup</span></span>](../api/publishedresource-post-agentgroups.md) | <span data-ttu-id="cb40c-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb40c-126">None</span></span> | <span data-ttu-id="cb40c-127">Atribua um objeto **publishedResource** a um **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="cb40c-127">Assign a **publishedResource** object to an **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="cb40c-128">Remover o publishedResource do onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="cb40c-128">Remove publishedResource from onPremisesAgentGroup</span></span>](../api/publishedresource-delete-agentgroups.md) | <span data-ttu-id="cb40c-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb40c-129">None</span></span> |  <span data-ttu-id="cb40c-130">Remover um objeto **publishedResource** de um **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="cb40c-130">Remove a **publishedResource** object from an **onPremisesAgentGroup**.</span></span>|

## <a name="properties"></a><span data-ttu-id="cb40c-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb40c-131">Properties</span></span>

| <span data-ttu-id="cb40c-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb40c-132">Property</span></span>     | <span data-ttu-id="cb40c-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb40c-133">Type</span></span>        | <span data-ttu-id="cb40c-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb40c-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cb40c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="cb40c-135">displayName</span></span>|<span data-ttu-id="cb40c-136">String</span><span class="sxs-lookup"><span data-stu-id="cb40c-136">String</span></span>| <span data-ttu-id="cb40c-137">Nome para exibição do publishedResource.</span><span class="sxs-lookup"><span data-stu-id="cb40c-137">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="cb40c-138">id</span><span class="sxs-lookup"><span data-stu-id="cb40c-138">id</span></span>|<span data-ttu-id="cb40c-139">String</span><span class="sxs-lookup"><span data-stu-id="cb40c-139">String</span></span>| <span data-ttu-id="cb40c-140">A ID de objeto do publishedResource.</span><span class="sxs-lookup"><span data-stu-id="cb40c-140">The object id of the publishedResource.</span></span> <span data-ttu-id="cb40c-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cb40c-141">Read-only.</span></span>|
|<span data-ttu-id="cb40c-142">publishingtype</span><span class="sxs-lookup"><span data-stu-id="cb40c-142">publishingType</span></span>|<span data-ttu-id="cb40c-143">string</span><span class="sxs-lookup"><span data-stu-id="cb40c-143">string</span></span>| <span data-ttu-id="cb40c-144">Os valores possíveis são: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="cb40c-144">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|
|<span data-ttu-id="cb40c-145">resourceName</span><span class="sxs-lookup"><span data-stu-id="cb40c-145">resourceName</span></span>|<span data-ttu-id="cb40c-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb40c-146">String</span></span>|<span data-ttu-id="cb40c-147">Nome do publishedResource.</span><span class="sxs-lookup"><span data-stu-id="cb40c-147">Name of the publishedResource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb40c-148">Relações</span><span class="sxs-lookup"><span data-stu-id="cb40c-148">Relationships</span></span>

| <span data-ttu-id="cb40c-149">Relação</span><span class="sxs-lookup"><span data-stu-id="cb40c-149">Relationship</span></span> | <span data-ttu-id="cb40c-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb40c-150">Type</span></span>        | <span data-ttu-id="cb40c-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb40c-151">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cb40c-152">agentGroups</span><span class="sxs-lookup"><span data-stu-id="cb40c-152">agentGroups</span></span>|<span data-ttu-id="cb40c-153">coleção [onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="cb40c-153">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="cb40c-154">Lista de **onPremisesAgentGroups** aos quais um **publishedResource** é atribuído.</span><span class="sxs-lookup"><span data-stu-id="cb40c-154">List of **onPremisesAgentGroups** that a **publishedResource** is assigned to.</span></span> <span data-ttu-id="cb40c-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cb40c-155">Read-only.</span></span> <span data-ttu-id="cb40c-156">Anulável.</span><span class="sxs-lookup"><span data-stu-id="cb40c-156">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb40c-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb40c-157">JSON representation</span></span>

<span data-ttu-id="cb40c-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cb40c-158">The following is a JSON representation of the resource.</span></span>

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
