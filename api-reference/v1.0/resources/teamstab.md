---
title: tipo de recurso teamsTab
description: 'Um teamsTab é uma guia fixa (anexada) a um canal dentro de uma equipe. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: bf07770d920ee05c7856f89e2e099bcc958ad50c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033688"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="6518e-103">tipo de recurso teamsTab</span><span class="sxs-lookup"><span data-stu-id="6518e-103">teamsTab resource type</span></span>



<span data-ttu-id="6518e-104">Um teamsTab é uma [guia](../resources/teamstab.md) fixa (anexada) a um [canal](channel.md) dentro de uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="6518e-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="6518e-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="6518e-105">Methods</span></span>

| <span data-ttu-id="6518e-106">Método</span><span class="sxs-lookup"><span data-stu-id="6518e-106">Method</span></span>       | <span data-ttu-id="6518e-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6518e-107">Return Type</span></span>  |<span data-ttu-id="6518e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6518e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6518e-109">Listar guias</span><span class="sxs-lookup"><span data-stu-id="6518e-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="6518e-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="6518e-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="6518e-111">Listar guias fixadas a um canal.</span><span class="sxs-lookup"><span data-stu-id="6518e-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="6518e-112">Obter guia</span><span class="sxs-lookup"><span data-stu-id="6518e-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="6518e-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="6518e-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="6518e-114">Ler uma guia fixada a um canal.</span><span class="sxs-lookup"><span data-stu-id="6518e-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="6518e-115">Adicionar guia</span><span class="sxs-lookup"><span data-stu-id="6518e-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="6518e-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="6518e-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="6518e-117">Adicionar (fixar) uma guia em um canal.</span><span class="sxs-lookup"><span data-stu-id="6518e-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="6518e-118">Remover guia</span><span class="sxs-lookup"><span data-stu-id="6518e-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="6518e-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6518e-119">None</span></span> | <span data-ttu-id="6518e-120">Remover (desafixar) uma guia de um canal.</span><span class="sxs-lookup"><span data-stu-id="6518e-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="6518e-121">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="6518e-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="6518e-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="6518e-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="6518e-123">Atualizar as propriedades da guia.</span><span class="sxs-lookup"><span data-stu-id="6518e-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="6518e-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6518e-124">Properties</span></span>

|<span data-ttu-id="6518e-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6518e-125">Property</span></span>|<span data-ttu-id="6518e-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="6518e-126">Type</span></span>|<span data-ttu-id="6518e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="6518e-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="6518e-128">id</span><span class="sxs-lookup"><span data-stu-id="6518e-128">id</span></span>              |   <span data-ttu-id="6518e-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6518e-129">string</span></span>                  |  <span data-ttu-id="6518e-130">Identificador que identifica exclusivamente uma instância específica de uma guia de canal. somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6518e-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="6518e-131">displayName</span><span class="sxs-lookup"><span data-stu-id="6518e-131">displayName</span></span>            |   <span data-ttu-id="6518e-132">string</span><span class="sxs-lookup"><span data-stu-id="6518e-132">string</span></span>                  |  <span data-ttu-id="6518e-133">Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="6518e-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="6518e-134">webUrl</span><span class="sxs-lookup"><span data-stu-id="6518e-134">webUrl</span></span>          |   <span data-ttu-id="6518e-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6518e-135">string</span></span>                  |  <span data-ttu-id="6518e-136">URL de link profundo da instância de guia.</span><span class="sxs-lookup"><span data-stu-id="6518e-136">Deep link url of the tab instance.</span></span> <span data-ttu-id="6518e-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6518e-137">Read only.</span></span>     |
|  <span data-ttu-id="6518e-138">Configuration</span><span class="sxs-lookup"><span data-stu-id="6518e-138">configuration</span></span>        |   [<span data-ttu-id="6518e-139">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="6518e-139">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="6518e-140">Contêiner para configurações personalizadas aplicadas a uma guia. A guia é considerada configurada somente quando essa propriedade é definida.</span><span class="sxs-lookup"><span data-stu-id="6518e-140">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="6518e-141">Relações</span><span class="sxs-lookup"><span data-stu-id="6518e-141">Relationships</span></span>

| <span data-ttu-id="6518e-142">Relação</span><span class="sxs-lookup"><span data-stu-id="6518e-142">Relationship</span></span> | <span data-ttu-id="6518e-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="6518e-143">Type</span></span>   | <span data-ttu-id="6518e-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="6518e-144">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6518e-145">teamsApp</span><span class="sxs-lookup"><span data-stu-id="6518e-145">teamsApp</span></span>|[<span data-ttu-id="6518e-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="6518e-146">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="6518e-147">O aplicativo que está vinculado à guia. Isso não pode ser alterado após a criação da Tabulação.</span><span class="sxs-lookup"><span data-stu-id="6518e-147">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6518e-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6518e-148">JSON representation</span></span>

<span data-ttu-id="6518e-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6518e-149">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="6518e-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="6518e-150">See also</span></span>

[<span data-ttu-id="6518e-151">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="6518e-151">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
