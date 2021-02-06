---
title: Tipo de recurso onPremisesAgentGroup
description: Tipo de recurso onPremisesAgentGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 0056f78eaecfad34a10dfb1ad2da04c15a6bc370
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136147"
---
# <a name="onpremisesagentgroup-resource-type"></a><span data-ttu-id="40540-103">Tipo de recurso onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="40540-103">onPremisesAgentGroup resource type</span></span>

<span data-ttu-id="40540-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40540-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40540-105">Representa o grupo de agentes locais.</span><span class="sxs-lookup"><span data-stu-id="40540-105">Represents on-premises agents group.</span></span> <span data-ttu-id="40540-106">Os grupos de agentes permitem que um administrador de locatários atribua [agentes](onpremisesagent.md) específicos para atender a recursos locais [publicados específicos.](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="40540-106">Agent groups enable a tenant admin to assign specific [agents](onpremisesagent.md) to serve specific [published on-premises resources](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="40540-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="40540-107">Methods</span></span>

| <span data-ttu-id="40540-108">Método</span><span class="sxs-lookup"><span data-stu-id="40540-108">Method</span></span>       | <span data-ttu-id="40540-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="40540-109">Return Type</span></span> | <span data-ttu-id="40540-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="40540-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="40540-111">Listar onPremisesAgentGroups</span><span class="sxs-lookup"><span data-stu-id="40540-111">List onPremisesAgentGroups</span></span>](../api/onpremisesagentgroup-list.md) | <span data-ttu-id="40540-112">Coleção onPremisesAgentGroups</span><span class="sxs-lookup"><span data-stu-id="40540-112">onPremisesAgentGroups collection</span></span> | <span data-ttu-id="40540-113">Obter uma **coleção de objetos onPremisesAgentGroup.**</span><span class="sxs-lookup"><span data-stu-id="40540-113">Get an **onPremisesAgentGroup** objects collection.</span></span> |
| [<span data-ttu-id="40540-114">Obter onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="40540-114">Get onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-get.md) | [<span data-ttu-id="40540-115">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="40540-115">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="40540-116">Leia as propriedades e os relacionamentos de um **objeto onPremisesAgentGroup.**</span><span class="sxs-lookup"><span data-stu-id="40540-116">Read the properties and relationships of an **onPremisesAgentGroup** object.</span></span> |
| [<span data-ttu-id="40540-117">Criar onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="40540-117">Create onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-post.md)  | [<span data-ttu-id="40540-118">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="40540-118">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="40540-119">Crie um novo **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="40540-119">Create a new **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="40540-120">Atualizar onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="40540-120">Update onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-update.md) | [<span data-ttu-id="40540-121">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="40540-121">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="40540-122">Atualize **um objeto onPremisesAgentGroup.**</span><span class="sxs-lookup"><span data-stu-id="40540-122">Update an **onPremisesAgentGroup** object.</span></span> |
| [<span data-ttu-id="40540-123">Excluir onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="40540-123">Delete  onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-delete.md) | <span data-ttu-id="40540-124">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="40540-124">None</span></span> | <span data-ttu-id="40540-125">**Exclua um objeto onPremisesAgentGroup.**</span><span class="sxs-lookup"><span data-stu-id="40540-125">Delete an **onPremisesAgentGroup** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="40540-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="40540-126">Properties</span></span>

| <span data-ttu-id="40540-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40540-127">Property</span></span>     | <span data-ttu-id="40540-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="40540-128">Type</span></span>        | <span data-ttu-id="40540-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="40540-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="40540-130">displayName</span><span class="sxs-lookup"><span data-stu-id="40540-130">displayName</span></span>|<span data-ttu-id="40540-131">String</span><span class="sxs-lookup"><span data-stu-id="40540-131">String</span></span>|<span data-ttu-id="40540-132">Nome de exibição **do onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="40540-132">Display name of the **onPremisesAgentGroup**.</span></span>|
|<span data-ttu-id="40540-133">id</span><span class="sxs-lookup"><span data-stu-id="40540-133">id</span></span>|<span data-ttu-id="40540-134">String</span><span class="sxs-lookup"><span data-stu-id="40540-134">String</span></span>| <span data-ttu-id="40540-135">A ID de objeto do **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="40540-135">The object ID of the **onPremisesAgentGroup**.</span></span> <span data-ttu-id="40540-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40540-136">Read-only.</span></span>|
|<span data-ttu-id="40540-137">isDefault</span><span class="sxs-lookup"><span data-stu-id="40540-137">isDefault</span></span>|<span data-ttu-id="40540-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="40540-138">Boolean</span></span>|<span data-ttu-id="40540-139">Indica se o **onPremisesAgentGroup é** o grupo de agentes padrão.</span><span class="sxs-lookup"><span data-stu-id="40540-139">Indicates if the **onPremisesAgentGroup** is the default agent group.</span></span> <span data-ttu-id="40540-140">Somente um único grupo de agentes pode ser o **onPremisesAgentGroup** padrão e é definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="40540-140">Only a single agent group can be the default **onPremisesAgentGroup** and is set by the system.</span></span>|
|<span data-ttu-id="40540-141">publishingType</span><span class="sxs-lookup"><span data-stu-id="40540-141">publishingType</span></span>|<span data-ttu-id="40540-142">string</span><span class="sxs-lookup"><span data-stu-id="40540-142">string</span></span>| <span data-ttu-id="40540-143">Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="40540-143">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40540-144">Relações</span><span class="sxs-lookup"><span data-stu-id="40540-144">Relationships</span></span>

| <span data-ttu-id="40540-145">Relação</span><span class="sxs-lookup"><span data-stu-id="40540-145">Relationship</span></span> | <span data-ttu-id="40540-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="40540-146">Type</span></span>        | <span data-ttu-id="40540-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="40540-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="40540-148">agentes</span><span class="sxs-lookup"><span data-stu-id="40540-148">agents</span></span>|<span data-ttu-id="40540-149">[Coleção onPremisesAgent](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="40540-149">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="40540-150">Lista de **onPremisesAgent** que são atribuídos a **um onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="40540-150">List of **onPremisesAgent** that are assigned to an **onPremisesAgentGroup**.</span></span> <span data-ttu-id="40540-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40540-151">Read-only.</span></span> <span data-ttu-id="40540-152">Anulável.</span><span class="sxs-lookup"><span data-stu-id="40540-152">Nullable.</span></span>|
|<span data-ttu-id="40540-153">publishedResources</span><span class="sxs-lookup"><span data-stu-id="40540-153">publishedResources</span></span>|<span data-ttu-id="40540-154">[Coleção publishedResource](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="40540-154">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="40540-155">Lista de **publishedResource** que são atribuídos a **um onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="40540-155">List of **publishedResource** that are assigned to an **onPremisesAgentGroup**.</span></span> <span data-ttu-id="40540-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40540-156">Read-only.</span></span> <span data-ttu-id="40540-157">Anulável.</span><span class="sxs-lookup"><span data-stu-id="40540-157">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="40540-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="40540-158">JSON representation</span></span>

<span data-ttu-id="40540-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="40540-159">The following is a JSON representation of the resource.</span></span>

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



