---
title: tipo de recurso onPremisesAgentGroup
description: tipo de recurso onPremisesAgentGroup.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 84f0236c2c2e52742a84f19eae8eb7693f1b559b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052593"
---
# <a name="onpremisesagentgroup-resource-type"></a><span data-ttu-id="e7a8b-103">tipo de recurso onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="e7a8b-103">onPremisesAgentGroup resource type</span></span>

<span data-ttu-id="e7a8b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7a8b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7a8b-105">Representa o grupo de agentes local.</span><span class="sxs-lookup"><span data-stu-id="e7a8b-105">Represents on-premises agents group.</span></span> <span data-ttu-id="e7a8b-106">Os grupos de agentes permitem que um administrador de locatários atribua [agentes](onpremisesagent.md) específicos para atender [recursos locais publicados](publishedresource.md)específicos.</span><span class="sxs-lookup"><span data-stu-id="e7a8b-106">Agent groups enable a tenant admin to assign specific [agents](onpremisesagent.md) to serve specific [published on-premises resources](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e7a8b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="e7a8b-107">Methods</span></span>

| <span data-ttu-id="e7a8b-108">Método</span><span class="sxs-lookup"><span data-stu-id="e7a8b-108">Method</span></span>       | <span data-ttu-id="e7a8b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e7a8b-109">Return Type</span></span> | <span data-ttu-id="e7a8b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7a8b-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e7a8b-111">Listar onPremisesAgentGroups</span><span class="sxs-lookup"><span data-stu-id="e7a8b-111">List onPremisesAgentGroups</span></span>](../api/onpremisesagentgroup-list.md) | <span data-ttu-id="e7a8b-112">coleção onPremisesAgentGroups</span><span class="sxs-lookup"><span data-stu-id="e7a8b-112">onPremisesAgentGroups collection</span></span> | <span data-ttu-id="e7a8b-113">Obtenha uma coleção de objetos **onPremisesAgentGroup** .</span><span class="sxs-lookup"><span data-stu-id="e7a8b-113">Get an **onPremisesAgentGroup** objects collection.</span></span> |
| [<span data-ttu-id="e7a8b-114">Obter onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="e7a8b-114">Get onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-get.md) | [<span data-ttu-id="e7a8b-115">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="e7a8b-115">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="e7a8b-116">Leia as propriedades e os relacionamentos de um objeto **onPremisesAgentGroup** .</span><span class="sxs-lookup"><span data-stu-id="e7a8b-116">Read the properties and relationships of an **onPremisesAgentGroup** object.</span></span> |
| [<span data-ttu-id="e7a8b-117">Criar onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="e7a8b-117">Create onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-post.md)  | [<span data-ttu-id="e7a8b-118">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="e7a8b-118">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="e7a8b-119">Criar um novo **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="e7a8b-119">Create a new **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="e7a8b-120">Atualizar onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="e7a8b-120">Update onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-update.md) | [<span data-ttu-id="e7a8b-121">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="e7a8b-121">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="e7a8b-122">Atualize um objeto **onPremisesAgentGroup** .</span><span class="sxs-lookup"><span data-stu-id="e7a8b-122">Update an **onPremisesAgentGroup** object.</span></span> |
| [<span data-ttu-id="e7a8b-123">Excluir onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="e7a8b-123">Delete  onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-delete.md) | <span data-ttu-id="e7a8b-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e7a8b-124">None</span></span> | <span data-ttu-id="e7a8b-125">Excluir um objeto **onPremisesAgentGroup** .</span><span class="sxs-lookup"><span data-stu-id="e7a8b-125">Delete an **onPremisesAgentGroup** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e7a8b-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e7a8b-126">Properties</span></span>

| <span data-ttu-id="e7a8b-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7a8b-127">Property</span></span>     | <span data-ttu-id="e7a8b-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7a8b-128">Type</span></span>        | <span data-ttu-id="e7a8b-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7a8b-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e7a8b-130">displayName</span><span class="sxs-lookup"><span data-stu-id="e7a8b-130">displayName</span></span>|<span data-ttu-id="e7a8b-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7a8b-131">String</span></span>|<span data-ttu-id="e7a8b-132">Nome para exibição do **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="e7a8b-132">Display name of the **onPremisesAgentGroup**.</span></span>|
|<span data-ttu-id="e7a8b-133">id</span><span class="sxs-lookup"><span data-stu-id="e7a8b-133">id</span></span>|<span data-ttu-id="e7a8b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7a8b-134">String</span></span>| <span data-ttu-id="e7a8b-135">A ID de objeto do **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="e7a8b-135">The object ID of the **onPremisesAgentGroup**.</span></span> <span data-ttu-id="e7a8b-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7a8b-136">Read-only.</span></span>|
|<span data-ttu-id="e7a8b-137">isDefault</span><span class="sxs-lookup"><span data-stu-id="e7a8b-137">isDefault</span></span>|<span data-ttu-id="e7a8b-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="e7a8b-138">Boolean</span></span>|<span data-ttu-id="e7a8b-139">Indica se o **onPremisesAgentGroup** é o grupo de agente padrão.</span><span class="sxs-lookup"><span data-stu-id="e7a8b-139">Indicates if the **onPremisesAgentGroup** is the default agent group.</span></span> <span data-ttu-id="e7a8b-140">Somente um único grupo de agentes pode ser o padrão **onPremisesAgentGroup** e é definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="e7a8b-140">Only a single agent group can be the default **onPremisesAgentGroup** and is set by the system.</span></span>|
|<span data-ttu-id="e7a8b-141">publishingtype</span><span class="sxs-lookup"><span data-stu-id="e7a8b-141">publishingType</span></span>|<span data-ttu-id="e7a8b-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7a8b-142">string</span></span>| <span data-ttu-id="e7a8b-143">Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="e7a8b-143">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7a8b-144">Relações</span><span class="sxs-lookup"><span data-stu-id="e7a8b-144">Relationships</span></span>

| <span data-ttu-id="e7a8b-145">Relação</span><span class="sxs-lookup"><span data-stu-id="e7a8b-145">Relationship</span></span> | <span data-ttu-id="e7a8b-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7a8b-146">Type</span></span>        | <span data-ttu-id="e7a8b-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7a8b-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e7a8b-148">SNMP</span><span class="sxs-lookup"><span data-stu-id="e7a8b-148">agents</span></span>|<span data-ttu-id="e7a8b-149">coleção [onPremisesAgent](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="e7a8b-149">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="e7a8b-150">Lista de **onPremisesAgent** que são atribuídas a um **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="e7a8b-150">List of **onPremisesAgent** that are assigned to an **onPremisesAgentGroup**.</span></span> <span data-ttu-id="e7a8b-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7a8b-151">Read-only.</span></span> <span data-ttu-id="e7a8b-152">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e7a8b-152">Nullable.</span></span>|
|<span data-ttu-id="e7a8b-153">publishedResources</span><span class="sxs-lookup"><span data-stu-id="e7a8b-153">publishedResources</span></span>|<span data-ttu-id="e7a8b-154">coleção [publishedResource](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="e7a8b-154">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="e7a8b-155">Lista de **publishedResource** que são atribuídas a um **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="e7a8b-155">List of **publishedResource** that are assigned to an **onPremisesAgentGroup**.</span></span> <span data-ttu-id="e7a8b-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7a8b-156">Read-only.</span></span> <span data-ttu-id="e7a8b-157">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e7a8b-157">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e7a8b-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e7a8b-158">JSON representation</span></span>

<span data-ttu-id="e7a8b-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e7a8b-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgentGroup",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "isDefault": true,
  "publishingType": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesAgentGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


