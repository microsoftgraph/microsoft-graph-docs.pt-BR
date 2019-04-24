---
title: tipo de recurso teamsTab
description: 'Um teamsTab é uma guia fixa (anexada) a um canal dentro de uma equipe. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 181d2fd23ff922709b3e098f6069adf300ad3928
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456974"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="0263a-103">tipo de recurso teamsTab</span><span class="sxs-lookup"><span data-stu-id="0263a-103">teamsTab resource type</span></span>



<span data-ttu-id="0263a-104">Um teamsTab é uma [guia](../resources/teamstab.md) fixa (anexada) a um [canal](channel.md) dentro de uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="0263a-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="0263a-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="0263a-105">Methods</span></span>

| <span data-ttu-id="0263a-106">Método</span><span class="sxs-lookup"><span data-stu-id="0263a-106">Method</span></span>       | <span data-ttu-id="0263a-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0263a-107">Return Type</span></span>  |<span data-ttu-id="0263a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0263a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0263a-109">Listar guias</span><span class="sxs-lookup"><span data-stu-id="0263a-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="0263a-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="0263a-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="0263a-111">Lista guias fixadas a um canal.</span><span class="sxs-lookup"><span data-stu-id="0263a-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="0263a-112">Obter guia</span><span class="sxs-lookup"><span data-stu-id="0263a-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="0263a-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="0263a-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="0263a-114">Lê uma guia fixada a um canal.</span><span class="sxs-lookup"><span data-stu-id="0263a-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="0263a-115">Adicionar guia</span><span class="sxs-lookup"><span data-stu-id="0263a-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="0263a-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="0263a-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="0263a-117">Adiciona (fixa) uma guia a um canal.</span><span class="sxs-lookup"><span data-stu-id="0263a-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="0263a-118">Guia remover</span><span class="sxs-lookup"><span data-stu-id="0263a-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="0263a-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0263a-119">None</span></span> | <span data-ttu-id="0263a-120">Remove (desfixa) uma guia de um canal.</span><span class="sxs-lookup"><span data-stu-id="0263a-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="0263a-121">Atualizar guia</span><span class="sxs-lookup"><span data-stu-id="0263a-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="0263a-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="0263a-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="0263a-123">Atualiza as propriedades da guia.</span><span class="sxs-lookup"><span data-stu-id="0263a-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="0263a-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0263a-124">Properties</span></span>

|<span data-ttu-id="0263a-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0263a-125">Property</span></span>|<span data-ttu-id="0263a-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="0263a-126">Type</span></span>|<span data-ttu-id="0263a-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="0263a-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="0263a-128">id</span><span class="sxs-lookup"><span data-stu-id="0263a-128">id</span></span>              |   <span data-ttu-id="0263a-129">string</span><span class="sxs-lookup"><span data-stu-id="0263a-129">string</span></span>                  |  <span data-ttu-id="0263a-130">Identificador que identifica exclusivamente uma instância específica de uma guia de canal. somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0263a-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="0263a-131">displayName</span><span class="sxs-lookup"><span data-stu-id="0263a-131">displayName</span></span>            |   <span data-ttu-id="0263a-132">string</span><span class="sxs-lookup"><span data-stu-id="0263a-132">string</span></span>                  |  <span data-ttu-id="0263a-133">Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="0263a-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="0263a-134">webUrl</span><span class="sxs-lookup"><span data-stu-id="0263a-134">webUrl</span></span>          |   <span data-ttu-id="0263a-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0263a-135">string</span></span>                  |  <span data-ttu-id="0263a-136">URL de link profundo da instância de guia.</span><span class="sxs-lookup"><span data-stu-id="0263a-136">Deep link url of the tab instance.</span></span> <span data-ttu-id="0263a-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0263a-137">Read only.</span></span>     |
|  <span data-ttu-id="0263a-138">Configuration</span><span class="sxs-lookup"><span data-stu-id="0263a-138">configuration</span></span>        |   [<span data-ttu-id="0263a-139">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="0263a-139">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="0263a-140">Contêiner para configurações personalizadas aplicadas a uma guia. A guia é considerada configurada somente quando essa propriedade é definida.</span><span class="sxs-lookup"><span data-stu-id="0263a-140">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="0263a-141">Relações</span><span class="sxs-lookup"><span data-stu-id="0263a-141">Relationships</span></span>

| <span data-ttu-id="0263a-142">Relação</span><span class="sxs-lookup"><span data-stu-id="0263a-142">Relationship</span></span> | <span data-ttu-id="0263a-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="0263a-143">Type</span></span>   | <span data-ttu-id="0263a-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="0263a-144">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0263a-145">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0263a-145">teamsApp</span></span>|[<span data-ttu-id="0263a-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0263a-146">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="0263a-147">O aplicativo que está vinculado à guia. Isso não pode ser alterado após a criação da Tabulação.</span><span class="sxs-lookup"><span data-stu-id="0263a-147">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0263a-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0263a-148">JSON representation</span></span>

<span data-ttu-id="0263a-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0263a-149">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="0263a-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="0263a-150">See also</span></span>

[<span data-ttu-id="0263a-151">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="0263a-151">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
