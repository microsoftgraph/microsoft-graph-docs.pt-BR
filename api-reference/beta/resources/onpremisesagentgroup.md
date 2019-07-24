---
title: tipo de recurso onPremisesAgentGroup
description: tipo de recurso onPremisesAgentGroup.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9e74a49a9a8c4b57232ed90cef232fa8b7feb998
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841315"
---
# <a name="onpremisesagentgroup-resource-type"></a><span data-ttu-id="a5589-103">tipo de recurso onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="a5589-103">onPremisesAgentGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5589-104">Representa o grupo de agentes local.</span><span class="sxs-lookup"><span data-stu-id="a5589-104">Represents on-premises agents group.</span></span> <span data-ttu-id="a5589-105">Os grupos de agentes permitem que um administrador de locatários atribua [agentes](onpremisesagent.md) específicos para atender [recursos locais publicados](publishedresource.md)específicos.</span><span class="sxs-lookup"><span data-stu-id="a5589-105">Agent groups enable a tenant admin to assign specific [agents](onpremisesagent.md) to serve specific [published on-premises resources](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a5589-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="a5589-106">Methods</span></span>

| <span data-ttu-id="a5589-107">Método</span><span class="sxs-lookup"><span data-stu-id="a5589-107">Method</span></span>       | <span data-ttu-id="a5589-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a5589-108">Return Type</span></span> | <span data-ttu-id="a5589-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5589-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a5589-110">Listar onPremisesAgentGroups</span><span class="sxs-lookup"><span data-stu-id="a5589-110">List onPremisesAgentGroups</span></span>](../api/onpremisesagentgroup-list.md) | <span data-ttu-id="a5589-111">coleção onPremisesAgentGroups</span><span class="sxs-lookup"><span data-stu-id="a5589-111">onPremisesAgentGroups collection</span></span> | <span data-ttu-id="a5589-112">Obtenha uma coleção de objetos **onPremisesAgentGroup** .</span><span class="sxs-lookup"><span data-stu-id="a5589-112">Get an **onPremisesAgentGroup** objects collection.</span></span> |
| [<span data-ttu-id="a5589-113">Obter onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="a5589-113">Get onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-get.md) | [<span data-ttu-id="a5589-114">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="a5589-114">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="a5589-115">Leia as propriedades e os relacionamentos de um objeto **onPremisesAgentGroup** .</span><span class="sxs-lookup"><span data-stu-id="a5589-115">Read the properties and relationships of an **onPremisesAgentGroup** object.</span></span> |
| [<span data-ttu-id="a5589-116">Criar onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="a5589-116">Create onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-post.md)  | [<span data-ttu-id="a5589-117">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="a5589-117">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="a5589-118">Criar um novo **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="a5589-118">Create a new **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="a5589-119">Atualizar onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="a5589-119">Update onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-update.md) | [<span data-ttu-id="a5589-120">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="a5589-120">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="a5589-121">Atualize um objeto **onPremisesAgentGroup** .</span><span class="sxs-lookup"><span data-stu-id="a5589-121">Update an **onPremisesAgentGroup** object.</span></span> |
| [<span data-ttu-id="a5589-122">Excluir onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="a5589-122">Delete  onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-delete.md) | <span data-ttu-id="a5589-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a5589-123">None</span></span> | <span data-ttu-id="a5589-124">Excluir um objeto **onPremisesAgentGroup** .</span><span class="sxs-lookup"><span data-stu-id="a5589-124">Delete an **onPremisesAgentGroup** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a5589-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a5589-125">Properties</span></span>

| <span data-ttu-id="a5589-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5589-126">Property</span></span>     | <span data-ttu-id="a5589-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5589-127">Type</span></span>        | <span data-ttu-id="a5589-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5589-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a5589-129">displayName</span><span class="sxs-lookup"><span data-stu-id="a5589-129">displayName</span></span>|<span data-ttu-id="a5589-130">String</span><span class="sxs-lookup"><span data-stu-id="a5589-130">String</span></span>|<span data-ttu-id="a5589-131">Nome para exibição do **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="a5589-131">Display name of the **onPremisesAgentGroup**.</span></span>|
|<span data-ttu-id="a5589-132">id</span><span class="sxs-lookup"><span data-stu-id="a5589-132">id</span></span>|<span data-ttu-id="a5589-133">String</span><span class="sxs-lookup"><span data-stu-id="a5589-133">String</span></span>| <span data-ttu-id="a5589-134">A ID de objeto do **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="a5589-134">The object ID of the **onPremisesAgentGroup**.</span></span> <span data-ttu-id="a5589-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a5589-135">Read-only.</span></span>|
|<span data-ttu-id="a5589-136">isDefault</span><span class="sxs-lookup"><span data-stu-id="a5589-136">isDefault</span></span>|<span data-ttu-id="a5589-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="a5589-137">Boolean</span></span>|<span data-ttu-id="a5589-138">Indica se o **onPremisesAgentGroup** é o grupo de agente padrão.</span><span class="sxs-lookup"><span data-stu-id="a5589-138">Indicates if the **onPremisesAgentGroup** is the default agent group.</span></span> <span data-ttu-id="a5589-139">Somente um único grupo de agentes pode ser o padrão **onPremisesAgentGroup** e é definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="a5589-139">Only a single agent group can be the default **onPremisesAgentGroup** and is set by the system.</span></span>|
|<span data-ttu-id="a5589-140">publishingtype</span><span class="sxs-lookup"><span data-stu-id="a5589-140">publishingType</span></span>|<span data-ttu-id="a5589-141">string</span><span class="sxs-lookup"><span data-stu-id="a5589-141">string</span></span>| <span data-ttu-id="a5589-142">Os valores possíveis são: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="a5589-142">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5589-143">Relações</span><span class="sxs-lookup"><span data-stu-id="a5589-143">Relationships</span></span>

| <span data-ttu-id="a5589-144">Relação</span><span class="sxs-lookup"><span data-stu-id="a5589-144">Relationship</span></span> | <span data-ttu-id="a5589-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5589-145">Type</span></span>        | <span data-ttu-id="a5589-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5589-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a5589-147">SNMP</span><span class="sxs-lookup"><span data-stu-id="a5589-147">agents</span></span>|<span data-ttu-id="a5589-148">coleção [onPremisesAgent](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="a5589-148">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="a5589-149">Lista de **onPremisesAgent** que são atribuídas a um **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="a5589-149">List of **onPremisesAgent** that are assigned to an **onPremisesAgentGroup**.</span></span> <span data-ttu-id="a5589-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a5589-150">Read-only.</span></span> <span data-ttu-id="a5589-151">Anulável.</span><span class="sxs-lookup"><span data-stu-id="a5589-151">Nullable.</span></span>|
|<span data-ttu-id="a5589-152">publishedResources</span><span class="sxs-lookup"><span data-stu-id="a5589-152">publishedResources</span></span>|<span data-ttu-id="a5589-153">coleção [publishedResource](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="a5589-153">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="a5589-154">Lista de **publishedResource** que são atribuídas a um **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="a5589-154">List of **publishedResource** that are assigned to an **onPremisesAgentGroup**.</span></span> <span data-ttu-id="a5589-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a5589-155">Read-only.</span></span> <span data-ttu-id="a5589-156">Anulável.</span><span class="sxs-lookup"><span data-stu-id="a5589-156">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5589-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a5589-157">JSON representation</span></span>

<span data-ttu-id="a5589-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a5589-158">The following is a JSON representation of the resource.</span></span>

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
