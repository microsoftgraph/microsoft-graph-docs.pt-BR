---
title: tipo de recurso teamsTab
description: 'Um teamsTab é uma guia fixa (anexada) a um canal dentro de uma equipe. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c62905699b8986d9594ccad06d154d93b71313fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533477"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="5271d-103">tipo de recurso teamsTab</span><span class="sxs-lookup"><span data-stu-id="5271d-103">teamsTab resource type</span></span>

<span data-ttu-id="5271d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5271d-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="5271d-105">Um teamsTab é uma [guia](../resources/teamstab.md) fixa (anexada) a um [canal](channel.md) dentro de uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="5271d-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="5271d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="5271d-106">Methods</span></span>

| <span data-ttu-id="5271d-107">Método</span><span class="sxs-lookup"><span data-stu-id="5271d-107">Method</span></span>       | <span data-ttu-id="5271d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5271d-108">Return Type</span></span>  |<span data-ttu-id="5271d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5271d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5271d-110">Listar guias</span><span class="sxs-lookup"><span data-stu-id="5271d-110">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="5271d-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="5271d-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="5271d-112">Listar guias fixadas a um canal.</span><span class="sxs-lookup"><span data-stu-id="5271d-112">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="5271d-113">Obter guia</span><span class="sxs-lookup"><span data-stu-id="5271d-113">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="5271d-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="5271d-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="5271d-115">Ler uma guia fixada a um canal.</span><span class="sxs-lookup"><span data-stu-id="5271d-115">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="5271d-116">Adicionar guia</span><span class="sxs-lookup"><span data-stu-id="5271d-116">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="5271d-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="5271d-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="5271d-118">Adicionar (fixar) uma guia em um canal.</span><span class="sxs-lookup"><span data-stu-id="5271d-118">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="5271d-119">Remover guia</span><span class="sxs-lookup"><span data-stu-id="5271d-119">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="5271d-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5271d-120">None</span></span> | <span data-ttu-id="5271d-121">Remover (desafixar) uma guia de um canal.</span><span class="sxs-lookup"><span data-stu-id="5271d-121">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="5271d-122">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="5271d-122">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="5271d-123">teamsTab</span><span class="sxs-lookup"><span data-stu-id="5271d-123">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="5271d-124">Atualizar as propriedades da guia.</span><span class="sxs-lookup"><span data-stu-id="5271d-124">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="5271d-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5271d-125">Properties</span></span>

|<span data-ttu-id="5271d-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5271d-126">Property</span></span>|<span data-ttu-id="5271d-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="5271d-127">Type</span></span>|<span data-ttu-id="5271d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="5271d-128">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="5271d-129">id</span><span class="sxs-lookup"><span data-stu-id="5271d-129">id</span></span>              |   <span data-ttu-id="5271d-130">string</span><span class="sxs-lookup"><span data-stu-id="5271d-130">string</span></span>                  |  <span data-ttu-id="5271d-131">Identificador que identifica exclusivamente uma instância específica de uma guia de canal. somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5271d-131">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="5271d-132">displayName</span><span class="sxs-lookup"><span data-stu-id="5271d-132">displayName</span></span>            |   <span data-ttu-id="5271d-133">string</span><span class="sxs-lookup"><span data-stu-id="5271d-133">string</span></span>                  |  <span data-ttu-id="5271d-134">Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="5271d-134">Name of the tab.</span></span>     |
|  <span data-ttu-id="5271d-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="5271d-135">webUrl</span></span>          |   <span data-ttu-id="5271d-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5271d-136">string</span></span>                  |  <span data-ttu-id="5271d-137">URL de link profundo da instância de guia.</span><span class="sxs-lookup"><span data-stu-id="5271d-137">Deep link url of the tab instance.</span></span> <span data-ttu-id="5271d-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5271d-138">Read only.</span></span>     |
|  <span data-ttu-id="5271d-139">Configuration</span><span class="sxs-lookup"><span data-stu-id="5271d-139">configuration</span></span>        |   [<span data-ttu-id="5271d-140">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="5271d-140">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="5271d-141">Contêiner para configurações personalizadas aplicadas a uma guia. A guia é considerada configurada somente quando essa propriedade é definida.</span><span class="sxs-lookup"><span data-stu-id="5271d-141">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="5271d-142">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="5271d-142">Relationships</span></span>

| <span data-ttu-id="5271d-143">Relação</span><span class="sxs-lookup"><span data-stu-id="5271d-143">Relationship</span></span> | <span data-ttu-id="5271d-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="5271d-144">Type</span></span>   | <span data-ttu-id="5271d-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="5271d-145">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5271d-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="5271d-146">teamsApp</span></span>|[<span data-ttu-id="5271d-147">teamsApp</span><span class="sxs-lookup"><span data-stu-id="5271d-147">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="5271d-148">O aplicativo que está vinculado à guia. Isso não pode ser alterado após a criação da Tabulação.</span><span class="sxs-lookup"><span data-stu-id="5271d-148">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5271d-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5271d-149">JSON representation</span></span>

<span data-ttu-id="5271d-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5271d-150">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
  "webUrl": "string",
  "configuration" : "teamsTabConfiguration"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="5271d-151">Confira também</span><span class="sxs-lookup"><span data-stu-id="5271d-151">See also</span></span>

[<span data-ttu-id="5271d-152">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="5271d-152">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
