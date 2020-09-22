---
title: tipo de recurso teamsTab
description: 'Um teamsTab é uma guia fixa (anexada) a um canal dentro de uma equipe. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5209670c004da2b58d41444c0bfa31f12891b8d2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074843"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="8651e-103">tipo de recurso teamsTab</span><span class="sxs-lookup"><span data-stu-id="8651e-103">teamsTab resource type</span></span>

<span data-ttu-id="8651e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8651e-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="8651e-105">Um teamsTab é uma [guia](../resources/teamstab.md) fixa (anexada) a um [canal](channel.md) dentro de uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="8651e-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="8651e-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8651e-106">Methods</span></span>

| <span data-ttu-id="8651e-107">Método</span><span class="sxs-lookup"><span data-stu-id="8651e-107">Method</span></span>       | <span data-ttu-id="8651e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8651e-108">Return Type</span></span>  |<span data-ttu-id="8651e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8651e-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8651e-110">Listar guias</span><span class="sxs-lookup"><span data-stu-id="8651e-110">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="8651e-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8651e-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="8651e-112">Listar guias fixadas a um canal.</span><span class="sxs-lookup"><span data-stu-id="8651e-112">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="8651e-113">Obter guia</span><span class="sxs-lookup"><span data-stu-id="8651e-113">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="8651e-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8651e-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="8651e-115">Ler uma guia fixada a um canal.</span><span class="sxs-lookup"><span data-stu-id="8651e-115">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="8651e-116">Adicionar guia</span><span class="sxs-lookup"><span data-stu-id="8651e-116">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="8651e-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8651e-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="8651e-118">Adicionar (fixar) uma guia em um canal.</span><span class="sxs-lookup"><span data-stu-id="8651e-118">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="8651e-119">Remover guia</span><span class="sxs-lookup"><span data-stu-id="8651e-119">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="8651e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8651e-120">None</span></span> | <span data-ttu-id="8651e-121">Remover (desafixar) uma guia de um canal.</span><span class="sxs-lookup"><span data-stu-id="8651e-121">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="8651e-122">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="8651e-122">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="8651e-123">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8651e-123">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="8651e-124">Atualizar as propriedades da guia.</span><span class="sxs-lookup"><span data-stu-id="8651e-124">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="8651e-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8651e-125">Properties</span></span>

|<span data-ttu-id="8651e-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8651e-126">Property</span></span>|<span data-ttu-id="8651e-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="8651e-127">Type</span></span>|<span data-ttu-id="8651e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="8651e-128">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="8651e-129">id</span><span class="sxs-lookup"><span data-stu-id="8651e-129">id</span></span>              |   <span data-ttu-id="8651e-130">string</span><span class="sxs-lookup"><span data-stu-id="8651e-130">string</span></span>                  |  <span data-ttu-id="8651e-131">Identificador que identifica exclusivamente uma instância específica de uma guia de canal. somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8651e-131">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="8651e-132">displayName</span><span class="sxs-lookup"><span data-stu-id="8651e-132">displayName</span></span>            |   <span data-ttu-id="8651e-133">string</span><span class="sxs-lookup"><span data-stu-id="8651e-133">string</span></span>                  |  <span data-ttu-id="8651e-134">Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="8651e-134">Name of the tab.</span></span>     |
|  <span data-ttu-id="8651e-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="8651e-135">webUrl</span></span>          |   <span data-ttu-id="8651e-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8651e-136">string</span></span>                  |  <span data-ttu-id="8651e-137">URL de link profundo da instância de guia.</span><span class="sxs-lookup"><span data-stu-id="8651e-137">Deep link URL of the tab instance.</span></span> <span data-ttu-id="8651e-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8651e-138">Read only.</span></span>     |
|  <span data-ttu-id="8651e-139">configuration</span><span class="sxs-lookup"><span data-stu-id="8651e-139">configuration</span></span>        |   [<span data-ttu-id="8651e-140">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="8651e-140">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="8651e-141">Contêiner para configurações personalizadas aplicadas a uma guia. A guia é considerada configurada somente quando essa propriedade é definida.</span><span class="sxs-lookup"><span data-stu-id="8651e-141">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="8651e-142">Relações</span><span class="sxs-lookup"><span data-stu-id="8651e-142">Relationships</span></span>

| <span data-ttu-id="8651e-143">Relação</span><span class="sxs-lookup"><span data-stu-id="8651e-143">Relationship</span></span> | <span data-ttu-id="8651e-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="8651e-144">Type</span></span>   | <span data-ttu-id="8651e-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="8651e-145">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8651e-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8651e-146">teamsApp</span></span>|[<span data-ttu-id="8651e-147">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8651e-147">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="8651e-148">O aplicativo que está vinculado à guia. Isso não pode ser alterado após a criação da Tabulação.</span><span class="sxs-lookup"><span data-stu-id="8651e-148">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8651e-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8651e-149">JSON representation</span></span>

<span data-ttu-id="8651e-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8651e-150">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="8651e-151">Confira também</span><span class="sxs-lookup"><span data-stu-id="8651e-151">See also</span></span>

[<span data-ttu-id="8651e-152">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="8651e-152">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

