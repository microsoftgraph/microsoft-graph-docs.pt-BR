---
title: Tipo de recurso publishedResource
description: Tipo de recurso publishedResource.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: e55abdad4a03319407b1c6e31e37e717739f0d10
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941761"
---
# <a name="publishedresource-resource-type"></a><span data-ttu-id="6db1e-103">Tipo de recurso publishedResource</span><span class="sxs-lookup"><span data-stu-id="6db1e-103">publishedResource resource type</span></span>

<span data-ttu-id="6db1e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6db1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6db1e-105">Representa o recurso publicado local.</span><span class="sxs-lookup"><span data-stu-id="6db1e-105">Represents on-premises published resource.</span></span> <span data-ttu-id="6db1e-106">Um administrador de locatários pode publicar vários tipos de recursos locais - aplicativos corporativos, controladores de domínio, servidores etc. Agentes locais instalados por um administrador de locatários podem ser [configurados](onpremisesagent.md) para acessar/manipular solicitações para um recurso publicado específico.</span><span class="sxs-lookup"><span data-stu-id="6db1e-106">A tenant administrator can publish various types of on-premises resources - enterprise applications, domain controllers, servers, etc. [On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular published resource.</span></span>

## <a name="methods"></a><span data-ttu-id="6db1e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="6db1e-107">Methods</span></span>

| <span data-ttu-id="6db1e-108">Método</span><span class="sxs-lookup"><span data-stu-id="6db1e-108">Method</span></span>       | <span data-ttu-id="6db1e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6db1e-109">Return Type</span></span> | <span data-ttu-id="6db1e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6db1e-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6db1e-111">Listar publishedResources</span><span class="sxs-lookup"><span data-stu-id="6db1e-111">List publishedResources</span></span>](../api/publishedresource-list.md) | <span data-ttu-id="6db1e-112">[Coleção de objetos publishedResource](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="6db1e-112">[publishedResource](publishedresource.md) objects collection</span></span> | <span data-ttu-id="6db1e-113">Obter uma **coleção de objetos publishedResources.**</span><span class="sxs-lookup"><span data-stu-id="6db1e-113">Get a **publishedResources** object collection.</span></span> |
| [<span data-ttu-id="6db1e-114">Obter publishedResource</span><span class="sxs-lookup"><span data-stu-id="6db1e-114">Get publishedResource</span></span>](../api/publishedresource-get.md) | [<span data-ttu-id="6db1e-115">publishedResource</span><span class="sxs-lookup"><span data-stu-id="6db1e-115">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="6db1e-116">Leia as propriedades e as relações de um **objeto publishedResource.**</span><span class="sxs-lookup"><span data-stu-id="6db1e-116">Read the properties and relationships of a **publishedResource** object.</span></span> |
| [<span data-ttu-id="6db1e-117">Criar publishedResource</span><span class="sxs-lookup"><span data-stu-id="6db1e-117">Create publishedResource</span></span>](../api/publishedresource-post.md) |  [<span data-ttu-id="6db1e-118">publishedResource</span><span class="sxs-lookup"><span data-stu-id="6db1e-118">publishedResource</span></span>](publishedresource.md)  | <span data-ttu-id="6db1e-119">Criar um novo **publishedResource**.</span><span class="sxs-lookup"><span data-stu-id="6db1e-119">Create a new **publishedResource**.</span></span> |
| [<span data-ttu-id="6db1e-120">Atualizar publishedResource</span><span class="sxs-lookup"><span data-stu-id="6db1e-120">Update publishedResource</span></span>](../api/publishedresource-update.md) | [<span data-ttu-id="6db1e-121">publishedResource</span><span class="sxs-lookup"><span data-stu-id="6db1e-121">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="6db1e-122">Atualize um **objeto publishedResource.**</span><span class="sxs-lookup"><span data-stu-id="6db1e-122">Update a **publishedResource** object.</span></span> |
| [<span data-ttu-id="6db1e-123">Excluir publishedResource</span><span class="sxs-lookup"><span data-stu-id="6db1e-123">Delete  publishedResource</span></span>](../api/publishedresource-delete.md) | <span data-ttu-id="6db1e-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6db1e-124">None</span></span> | <span data-ttu-id="6db1e-125">**Exclua um objeto publishedResource.**</span><span class="sxs-lookup"><span data-stu-id="6db1e-125">Delete a **publishedResource** object.</span></span> |
| [<span data-ttu-id="6db1e-126">Atribuir publishedResource ao onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="6db1e-126">Assign publishedResource to onPremisesAgentGroup</span></span>](../api/publishedresource-post-agentgroups.md) | <span data-ttu-id="6db1e-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6db1e-127">None</span></span> | <span data-ttu-id="6db1e-128">Atribua um **objeto publishedResource** a **um onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="6db1e-128">Assign a **publishedResource** object to an **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="6db1e-129">Remover publishedResource do onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="6db1e-129">Remove publishedResource from onPremisesAgentGroup</span></span>](../api/publishedresource-delete-agentgroups.md) | <span data-ttu-id="6db1e-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6db1e-130">None</span></span> |  <span data-ttu-id="6db1e-131">Remover um **objeto publishedResource** de **um onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="6db1e-131">Remove a **publishedResource** object from an **onPremisesAgentGroup**.</span></span>|

## <a name="properties"></a><span data-ttu-id="6db1e-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6db1e-132">Properties</span></span>

| <span data-ttu-id="6db1e-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6db1e-133">Property</span></span>     | <span data-ttu-id="6db1e-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="6db1e-134">Type</span></span>        | <span data-ttu-id="6db1e-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="6db1e-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6db1e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6db1e-136">displayName</span></span>|<span data-ttu-id="6db1e-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6db1e-137">String</span></span>| <span data-ttu-id="6db1e-138">Nome de exibição do publishedResource.</span><span class="sxs-lookup"><span data-stu-id="6db1e-138">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="6db1e-139">id</span><span class="sxs-lookup"><span data-stu-id="6db1e-139">id</span></span>|<span data-ttu-id="6db1e-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6db1e-140">String</span></span>| <span data-ttu-id="6db1e-141">A id do objeto do publishedResource.</span><span class="sxs-lookup"><span data-stu-id="6db1e-141">The object id of the publishedResource.</span></span> <span data-ttu-id="6db1e-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6db1e-142">Read-only.</span></span>|
|<span data-ttu-id="6db1e-143">publishingType</span><span class="sxs-lookup"><span data-stu-id="6db1e-143">publishingType</span></span>|<span data-ttu-id="6db1e-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6db1e-144">String</span></span>| <span data-ttu-id="6db1e-145">Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="6db1e-145">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|
|<span data-ttu-id="6db1e-146">resourceName</span><span class="sxs-lookup"><span data-stu-id="6db1e-146">resourceName</span></span>|<span data-ttu-id="6db1e-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6db1e-147">String</span></span>|<span data-ttu-id="6db1e-148">Nome do publishedResource.</span><span class="sxs-lookup"><span data-stu-id="6db1e-148">Name of the publishedResource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6db1e-149">Relações</span><span class="sxs-lookup"><span data-stu-id="6db1e-149">Relationships</span></span>

| <span data-ttu-id="6db1e-150">Relação</span><span class="sxs-lookup"><span data-stu-id="6db1e-150">Relationship</span></span> | <span data-ttu-id="6db1e-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="6db1e-151">Type</span></span>        | <span data-ttu-id="6db1e-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="6db1e-152">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6db1e-153">agentGroups</span><span class="sxs-lookup"><span data-stu-id="6db1e-153">agentGroups</span></span>|<span data-ttu-id="6db1e-154">[Coleção onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="6db1e-154">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="6db1e-155">Lista de **onPremisesAgentGroups** aos que um **publishedResource** é atribuído.</span><span class="sxs-lookup"><span data-stu-id="6db1e-155">List of **onPremisesAgentGroups** that a **publishedResource** is assigned to.</span></span> <span data-ttu-id="6db1e-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6db1e-156">Read-only.</span></span> <span data-ttu-id="6db1e-157">Anulável.</span><span class="sxs-lookup"><span data-stu-id="6db1e-157">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6db1e-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6db1e-158">JSON representation</span></span>

<span data-ttu-id="6db1e-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6db1e-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publishedResource",
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


