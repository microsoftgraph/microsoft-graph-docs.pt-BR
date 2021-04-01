---
author: mohitpcad
title: Tipo de recurso de grupo
doc_type: resourcePageType
description: Representa um grupo usado em um armazenamento de termos.
localization_priority: Normal
ms.prod: Sharepoint
ms.openlocfilehash: 1249f94b96e0c6ff7251a2a97f4885a21258aaeb
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473462"
---
# <a name="group-resource-type"></a><span data-ttu-id="9f161-103">Tipo de recurso de grupo</span><span class="sxs-lookup"><span data-stu-id="9f161-103">Group resource type</span></span>

<span data-ttu-id="9f161-104">Namespace: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="9f161-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="9f161-105">Representa um grupo usado em um armazenamento de [termos.](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="9f161-105">Represents a group used in a term [store](../resources/termstore-store.md).</span></span> <span data-ttu-id="9f161-106">Um grupo é uma hierarquia lógica que contém uma coleção de conjuntos sob ele.</span><span class="sxs-lookup"><span data-stu-id="9f161-106">A group is a logical hierarchy that contains a collection of sets under it.</span></span> 

<span data-ttu-id="9f161-107">Herda da [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="9f161-107">Inherits from [entity](../resources/entity.md).</span></span>


## <a name="methods"></a><span data-ttu-id="9f161-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="9f161-108">Methods</span></span>

| <span data-ttu-id="9f161-109">Método</span><span class="sxs-lookup"><span data-stu-id="9f161-109">Method</span></span>                                                   | <span data-ttu-id="9f161-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9f161-110">Return type</span></span>       |    <span data-ttu-id="9f161-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f161-111">Description</span></span>
|:---------------------------------------------------------|:------------------|:---------------------
| [<span data-ttu-id="9f161-112">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="9f161-112">Create group</span></span>](../api/termstore-group-post.md)                     | <span data-ttu-id="9f161-113">[microsoft.graph.termStore.group]</span><span class="sxs-lookup"><span data-stu-id="9f161-113">[microsoft.graph.termStore.group]</span></span> | <span data-ttu-id="9f161-114">Criar um grupo em um armazenamento de [termos.]</span><span class="sxs-lookup"><span data-stu-id="9f161-114">Create a group in a term [store].</span></span>
| [<span data-ttu-id="9f161-115">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="9f161-115">Get group</span></span>](../api/termstore-store-get-group.md)                           | <span data-ttu-id="9f161-116">[microsoft.graph.termStore.group]</span><span class="sxs-lookup"><span data-stu-id="9f161-116">[microsoft.graph.termStore.group]</span></span> | <span data-ttu-id="9f161-117">Recupere os dados de um grupo em um armazenamento de [termos.]</span><span class="sxs-lookup"><span data-stu-id="9f161-117">Retrieve the data of a group in a term [store].</span></span>
| [<span data-ttu-id="9f161-118">Excluir grupo</span><span class="sxs-lookup"><span data-stu-id="9f161-118">Delete group</span></span>](../api/termstore-group-delete.md)                     | <span data-ttu-id="9f161-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9f161-119">None</span></span> |  <span data-ttu-id="9f161-120">Excluir um grupo em um armazenamento de [termos.]</span><span class="sxs-lookup"><span data-stu-id="9f161-120">Delete a group in a term [store].</span></span>

## <a name="properties"></a><span data-ttu-id="9f161-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f161-121">Properties</span></span>

| <span data-ttu-id="9f161-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f161-122">Property</span></span>             | <span data-ttu-id="9f161-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f161-123">Type</span></span>               | <span data-ttu-id="9f161-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f161-124">Description</span></span>
|:---------------------|:-------------------|:------------------------------------
| <span data-ttu-id="9f161-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f161-125">createdDateTime</span></span>      | <span data-ttu-id="9f161-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f161-126">DateTimeOffset</span></span>     | <span data-ttu-id="9f161-127">Data e hora da criação do grupo.</span><span class="sxs-lookup"><span data-stu-id="9f161-127">Date and time of group creation.</span></span> <span data-ttu-id="9f161-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f161-128">Read-only.</span></span>
| <span data-ttu-id="9f161-129">description</span><span class="sxs-lookup"><span data-stu-id="9f161-129">description</span></span>          | <span data-ttu-id="9f161-130">string</span><span class="sxs-lookup"><span data-stu-id="9f161-130">string</span></span>             | <span data-ttu-id="9f161-131">Descrição que dá detalhes sobre o uso do termo.</span><span class="sxs-lookup"><span data-stu-id="9f161-131">Description giving details on the term usage.</span></span>
| <span data-ttu-id="9f161-132">id</span><span class="sxs-lookup"><span data-stu-id="9f161-132">id</span></span>                   | <span data-ttu-id="9f161-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f161-133">string</span></span>             | <span data-ttu-id="9f161-134">Identificador exclusivo do grupo.</span><span class="sxs-lookup"><span data-stu-id="9f161-134">Unique identifier of group.</span></span> <span data-ttu-id="9f161-135">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="9f161-135">Read-Only.</span></span>
| <span data-ttu-id="9f161-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9f161-136">displayName</span></span>          | <span data-ttu-id="9f161-137">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f161-137">string</span></span>             | <span data-ttu-id="9f161-138">Nome do grupo.</span><span class="sxs-lookup"><span data-stu-id="9f161-138">Name of group.</span></span>
| <span data-ttu-id="9f161-139">escopo</span><span class="sxs-lookup"><span data-stu-id="9f161-139">scope</span></span>                | <span data-ttu-id="9f161-140">string</span><span class="sxs-lookup"><span data-stu-id="9f161-140">string</span></span>              | <span data-ttu-id="9f161-141">Retorna o tipo de grupo.</span><span class="sxs-lookup"><span data-stu-id="9f161-141">Returns type of group.</span></span> <span data-ttu-id="9f161-142">Os valores possíveis são 'global', 'system' e 'siteCollection'.</span><span class="sxs-lookup"><span data-stu-id="9f161-142">Possible values are 'global', 'system' and 'siteCollection'.</span></span>
| <span data-ttu-id="9f161-143">parentSiteId</span><span class="sxs-lookup"><span data-stu-id="9f161-143">parentSiteId</span></span>         | <span data-ttu-id="9f161-144">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f161-144">string</span></span>             | <span data-ttu-id="9f161-145">ID do site pai deste grupo.</span><span class="sxs-lookup"><span data-stu-id="9f161-145">Id of the parent site of this group.</span></span>

## <a name="relationships"></a><span data-ttu-id="9f161-146">Relações</span><span class="sxs-lookup"><span data-stu-id="9f161-146">Relationships</span></span>
| <span data-ttu-id="9f161-147">Relação</span><span class="sxs-lookup"><span data-stu-id="9f161-147">Relationship</span></span>       | <span data-ttu-id="9f161-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f161-148">Type</span></span>                        | <span data-ttu-id="9f161-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f161-149">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="9f161-150">sets</span><span class="sxs-lookup"><span data-stu-id="9f161-150">sets</span></span>           | <span data-ttu-id="9f161-151">[coleção microsoft.graph.termStore.set][]</span><span class="sxs-lookup"><span data-stu-id="9f161-151">[microsoft.graph.termStore.set][] collection</span></span> | <span data-ttu-id="9f161-152">Todos os conjuntos sob o grupo em um armazenamento de [termos].</span><span class="sxs-lookup"><span data-stu-id="9f161-152">All sets under the group in a term [store].</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f161-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f161-153">JSON representation</span></span>

<span data-ttu-id="9f161-154">A seguir está uma representação JSON de um **recurso de** grupo.</span><span class="sxs-lookup"><span data-stu-id="9f161-154">The following is a JSON representation of a **group** resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.group",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
```json
{
  "@odata.type": "#microsoft.graph.termStore.group",
  "id": "string",
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "scope" : "microsoft.graph.termStore.groupScope",
  "displayName": "string",
  "parentSiteId" : "string"
}
```



[identitySet]: identitySet.md
[microsoft.graph.termStore.set]: termstore-set.md
[microsoft.graph.termStore.group]: termstore-group.md
[microsoft.graph.termStore.store]: termstore-store.md
[store]: ../resources/termstore-store.md
[group]: ../resources/termstore-group.md
[set]: ../resources/termstore-set.md
<!--
{
  "type": "#page.annotation",
  "description": "TermGroup is the entity used for managing permissions for the termSets in termStore",
  "keywords": "termGroup,facet,resource",
  "section": "documentation",
  "tocPath": "TermGroup",
  "tocBookmarks": {
    "Resources/termStore.group": "#"
  },
  "suppressions": []
}
-->


