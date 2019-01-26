---
title: tipo de recurso de teamsTab
description: 'Um teamsTab é uma guia que tem fixados (anexado) a um canal de uma equipe. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 181d2fd23ff922709b3e098f6069adf300ad3928
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574667"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="c8456-103">tipo de recurso de teamsTab</span><span class="sxs-lookup"><span data-stu-id="c8456-103">teamsTab resource type</span></span>



<span data-ttu-id="c8456-104">Um teamsTab é uma [guia](../resources/teamstab.md) que tem fixados (anexado) a um [canal](channel.md) de dentro de uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="c8456-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="c8456-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="c8456-105">Methods</span></span>

| <span data-ttu-id="c8456-106">Método</span><span class="sxs-lookup"><span data-stu-id="c8456-106">Method</span></span>       | <span data-ttu-id="c8456-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c8456-107">Return Type</span></span>  |<span data-ttu-id="c8456-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8456-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c8456-109">Guias de lista</span><span class="sxs-lookup"><span data-stu-id="c8456-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="c8456-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c8456-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="c8456-111">Guias de listas fixados em um canal.</span><span class="sxs-lookup"><span data-stu-id="c8456-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="c8456-112">Obtenha o guia</span><span class="sxs-lookup"><span data-stu-id="c8456-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="c8456-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c8456-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="c8456-114">Lê uma guia fixada em um canal.</span><span class="sxs-lookup"><span data-stu-id="c8456-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="c8456-115">Adicionar guia</span><span class="sxs-lookup"><span data-stu-id="c8456-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="c8456-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c8456-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="c8456-117">Adiciona (pins) uma guia em um canal.</span><span class="sxs-lookup"><span data-stu-id="c8456-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="c8456-118">Remover guia</span><span class="sxs-lookup"><span data-stu-id="c8456-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="c8456-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c8456-119">None</span></span> | <span data-ttu-id="c8456-120">Remove (unpin) uma guia de um canal.</span><span class="sxs-lookup"><span data-stu-id="c8456-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="c8456-121">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="c8456-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="c8456-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c8456-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="c8456-123">Atualiza as propriedades da guia.</span><span class="sxs-lookup"><span data-stu-id="c8456-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="c8456-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8456-124">Properties</span></span>

|<span data-ttu-id="c8456-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8456-125">Property</span></span>|<span data-ttu-id="c8456-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8456-126">Type</span></span>|<span data-ttu-id="c8456-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8456-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="c8456-128">id</span><span class="sxs-lookup"><span data-stu-id="c8456-128">id</span></span>              |   <span data-ttu-id="c8456-129">string</span><span class="sxs-lookup"><span data-stu-id="c8456-129">string</span></span>                  |  <span data-ttu-id="c8456-130">Identificador que identifica exclusivamente uma instância específica de um canal na guia leitura apenas.</span><span class="sxs-lookup"><span data-stu-id="c8456-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="c8456-131">displayName</span><span class="sxs-lookup"><span data-stu-id="c8456-131">displayName</span></span>            |   <span data-ttu-id="c8456-132">string</span><span class="sxs-lookup"><span data-stu-id="c8456-132">string</span></span>                  |  <span data-ttu-id="c8456-133">Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="c8456-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="c8456-134">webUrl</span><span class="sxs-lookup"><span data-stu-id="c8456-134">webUrl</span></span>          |   <span data-ttu-id="c8456-135">string</span><span class="sxs-lookup"><span data-stu-id="c8456-135">string</span></span>                  |  <span data-ttu-id="c8456-136">Link profundo url da instância do guia.</span><span class="sxs-lookup"><span data-stu-id="c8456-136">Deep link url of the tab instance.</span></span> <span data-ttu-id="c8456-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c8456-137">Read only.</span></span>     |
|  <span data-ttu-id="c8456-138">configuration</span><span class="sxs-lookup"><span data-stu-id="c8456-138">configuration</span></span>        |   [<span data-ttu-id="c8456-139">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="c8456-139">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="c8456-140">Contêiner de configurações personalizadas aplicadas a uma guia. Na guia é considerada configurado somente depois que essa propriedade for definida.</span><span class="sxs-lookup"><span data-stu-id="c8456-140">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="c8456-141">Relações</span><span class="sxs-lookup"><span data-stu-id="c8456-141">Relationships</span></span>

| <span data-ttu-id="c8456-142">Relação</span><span class="sxs-lookup"><span data-stu-id="c8456-142">Relationship</span></span> | <span data-ttu-id="c8456-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8456-143">Type</span></span>   | <span data-ttu-id="c8456-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8456-144">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c8456-145">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c8456-145">teamsApp</span></span>|[<span data-ttu-id="c8456-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c8456-146">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="c8456-147">O aplicativo que está vinculado à guia. Isso não pode ser alterado após a criação da guia.</span><span class="sxs-lookup"><span data-stu-id="c8456-147">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c8456-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8456-148">JSON representation</span></span>

<span data-ttu-id="c8456-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8456-149">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="c8456-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="c8456-150">See also</span></span>

[<span data-ttu-id="c8456-151">Configurando os tipos de guia interna</span><span class="sxs-lookup"><span data-stu-id="c8456-151">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
