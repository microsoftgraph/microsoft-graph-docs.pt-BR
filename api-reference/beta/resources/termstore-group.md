---
author: mohitpcad
title: Tipo de recurso de grupo
doc_type: resourcePageType
description: Representa um grupo usado em um repositório de termos.
localization_priority: Normal
ms.prod: Sharepoint
ms.openlocfilehash: aa86722dfd0a761525a8ec4d142ed27dc93be6c2
ms.sourcegitcommit: b7e82d0d64f640a09f5da76b38d8ed9f13684f95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2020
ms.locfileid: "48258420"
---
# <a name="group-resource-type"></a><span data-ttu-id="b4c7d-103">Tipo de recurso de grupo</span><span class="sxs-lookup"><span data-stu-id="b4c7d-103">Group resource type</span></span>

<span data-ttu-id="b4c7d-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="b4c7d-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="b4c7d-105">Representa um grupo usado em um [repositório](../resources/termstore-store.md)de termos.</span><span class="sxs-lookup"><span data-stu-id="b4c7d-105">Represents a group used in a term [store](../resources/termstore-store.md).</span></span> <span data-ttu-id="b4c7d-106">Um grupo é uma hierarquia lógica que contém uma coleção de conjuntos abaixo dele.</span><span class="sxs-lookup"><span data-stu-id="b4c7d-106">A group is a logical hierarchy that contains a collection of sets under it.</span></span> 

<span data-ttu-id="b4c7d-107">Herda de [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="b4c7d-107">Inherits from [entity](../resources/entity.md).</span></span>


## <a name="methods"></a><span data-ttu-id="b4c7d-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="b4c7d-108">Methods</span></span>

| <span data-ttu-id="b4c7d-109">Método</span><span class="sxs-lookup"><span data-stu-id="b4c7d-109">Method</span></span>                                                   | <span data-ttu-id="b4c7d-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b4c7d-110">Return type</span></span>       |    <span data-ttu-id="b4c7d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4c7d-111">Description</span></span>
|:---------------------------------------------------------|:------------------|:---------------------
| [<span data-ttu-id="b4c7d-112">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="b4c7d-112">Create group</span></span>](../api/termstore-group-post.md)                     | <span data-ttu-id="b4c7d-113">[Microsoft. Graph. termos. Group]</span><span class="sxs-lookup"><span data-stu-id="b4c7d-113">[microsoft.graph.termStore.group]</span></span> | <span data-ttu-id="b4c7d-114">Criar um grupo em um [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="b4c7d-114">Create a group in a term [store].</span></span>
| [<span data-ttu-id="b4c7d-115">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="b4c7d-115">Get group</span></span>](../api/termstore-store-get-group.md)                           | <span data-ttu-id="b4c7d-116">[Microsoft. Graph. termos. Group]</span><span class="sxs-lookup"><span data-stu-id="b4c7d-116">[microsoft.graph.termStore.group]</span></span> | <span data-ttu-id="b4c7d-117">Recupere os dados de um grupo em um [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="b4c7d-117">Retrieve the data of a group in a term [store].</span></span>
| [<span data-ttu-id="b4c7d-118">Excluir grupo</span><span class="sxs-lookup"><span data-stu-id="b4c7d-118">Delete group</span></span>](../api/termstore-group-delete.md)                     | <span data-ttu-id="b4c7d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b4c7d-119">None</span></span> |  <span data-ttu-id="b4c7d-120">Excluir um grupo em um [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="b4c7d-120">Delete a group in a term [store].</span></span>

## <a name="properties"></a><span data-ttu-id="b4c7d-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4c7d-121">Properties</span></span>

| <span data-ttu-id="b4c7d-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4c7d-122">Property</span></span>             | <span data-ttu-id="b4c7d-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4c7d-123">Type</span></span>               | <span data-ttu-id="b4c7d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4c7d-124">Description</span></span>
|:---------------------|:-------------------|:------------------------------------
| <span data-ttu-id="b4c7d-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4c7d-125">createdDateTime</span></span>      | <span data-ttu-id="b4c7d-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4c7d-126">DateTimeOffset</span></span>     | <span data-ttu-id="b4c7d-127">Data e hora da criação do grupo.</span><span class="sxs-lookup"><span data-stu-id="b4c7d-127">Date and time of group creation.</span></span> <span data-ttu-id="b4c7d-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b4c7d-128">Read-only.</span></span>
| <span data-ttu-id="b4c7d-129">description</span><span class="sxs-lookup"><span data-stu-id="b4c7d-129">description</span></span>          | <span data-ttu-id="b4c7d-130">string</span><span class="sxs-lookup"><span data-stu-id="b4c7d-130">string</span></span>             | <span data-ttu-id="b4c7d-131">Descrição que oferece detalhes sobre o uso de termos.</span><span class="sxs-lookup"><span data-stu-id="b4c7d-131">Description giving details on the term usage.</span></span>
| <span data-ttu-id="b4c7d-132">id</span><span class="sxs-lookup"><span data-stu-id="b4c7d-132">id</span></span>                   | <span data-ttu-id="b4c7d-133">string</span><span class="sxs-lookup"><span data-stu-id="b4c7d-133">string</span></span>             | <span data-ttu-id="b4c7d-134">Identificador exclusivo do grupo.</span><span class="sxs-lookup"><span data-stu-id="b4c7d-134">Unique identifier of group.</span></span> <span data-ttu-id="b4c7d-135">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="b4c7d-135">Read-Only.</span></span>
| <span data-ttu-id="b4c7d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b4c7d-136">displayName</span></span>          | <span data-ttu-id="b4c7d-137">string</span><span class="sxs-lookup"><span data-stu-id="b4c7d-137">string</span></span>             | <span data-ttu-id="b4c7d-138">Nome do grupo.</span><span class="sxs-lookup"><span data-stu-id="b4c7d-138">Name of group.</span></span>
| <span data-ttu-id="b4c7d-139">escopo</span><span class="sxs-lookup"><span data-stu-id="b4c7d-139">scope</span></span>                | <span data-ttu-id="b4c7d-140">string</span><span class="sxs-lookup"><span data-stu-id="b4c7d-140">string</span></span>              | <span data-ttu-id="b4c7d-141">Retorna o tipo de grupo.</span><span class="sxs-lookup"><span data-stu-id="b4c7d-141">Returns type of group.</span></span> <span data-ttu-id="b4c7d-142">Os valores possíveis são ' global ', ' System ' e ' SiteCollection '.</span><span class="sxs-lookup"><span data-stu-id="b4c7d-142">Possible values are 'global', 'system' and 'siteCollection'.</span></span>

## <a name="relationships"></a><span data-ttu-id="b4c7d-143">Relações</span><span class="sxs-lookup"><span data-stu-id="b4c7d-143">Relationships</span></span>
| <span data-ttu-id="b4c7d-144">Relação</span><span class="sxs-lookup"><span data-stu-id="b4c7d-144">Relationship</span></span>       | <span data-ttu-id="b4c7d-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4c7d-145">Type</span></span>                        | <span data-ttu-id="b4c7d-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4c7d-146">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="b4c7d-147">jogos</span><span class="sxs-lookup"><span data-stu-id="b4c7d-147">sets</span></span>           | <span data-ttu-id="b4c7d-148">coleção [Microsoft. Graph. termos. Set][]</span><span class="sxs-lookup"><span data-stu-id="b4c7d-148">[microsoft.graph.termStore.set][] collection</span></span> | <span data-ttu-id="b4c7d-149">Todos os conjuntos no grupo em um [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="b4c7d-149">All sets under the group in a term [store].</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4c7d-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4c7d-150">JSON representation</span></span>

<span data-ttu-id="b4c7d-151">Veja a seguir uma representação JSON de um recurso de **grupo** .</span><span class="sxs-lookup"><span data-stu-id="b4c7d-151">The following is a JSON representation of a **group** resource.</span></span>
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
  "displayName": "string" 
}
```



[identitySet]: identitySet.md
[Microsoft. Graph. termos. Set]: termstore-set.md
[microsoft.graph.termStore.set]: termstore-set.md
[Microsoft. Graph. termos. Group]: termstore-group.md
[microsoft.graph.termStore.group]: termstore-group.md
[microsoft.graph.termStore.store]: termstore-store.md
[Guarde]: ../resources/termstore-store.md
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


