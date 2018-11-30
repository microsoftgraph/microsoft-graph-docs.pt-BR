---
title: tipo de recurso de teamsTab
description: 'Um teamsTab é uma guia que tem fixados (anexado) a um canal de uma equipe. '
ms.openlocfilehash: 4e9773fa2e4ea6a114c1f2695906c09d84b3f043
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005318"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="573ed-103">tipo de recurso de teamsTab</span><span class="sxs-lookup"><span data-stu-id="573ed-103">teamsTab resource type</span></span>



<span data-ttu-id="573ed-104">Um teamsTab é uma [guia](../resources/teamstab.md) que tem fixados (anexado) a um [canal](channel.md) de dentro de uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="573ed-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="573ed-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="573ed-105">Methods</span></span>

| <span data-ttu-id="573ed-106">Método</span><span class="sxs-lookup"><span data-stu-id="573ed-106">Method</span></span>       | <span data-ttu-id="573ed-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="573ed-107">Return Type</span></span>  |<span data-ttu-id="573ed-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="573ed-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="573ed-109">Guias de lista</span><span class="sxs-lookup"><span data-stu-id="573ed-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="573ed-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="573ed-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="573ed-111">Guias de listas fixados em um canal.</span><span class="sxs-lookup"><span data-stu-id="573ed-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="573ed-112">Obtenha o guia</span><span class="sxs-lookup"><span data-stu-id="573ed-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="573ed-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="573ed-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="573ed-114">Lê uma guia fixada em um canal.</span><span class="sxs-lookup"><span data-stu-id="573ed-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="573ed-115">Adicionar guia</span><span class="sxs-lookup"><span data-stu-id="573ed-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="573ed-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="573ed-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="573ed-117">Adiciona (pins) uma guia em um canal.</span><span class="sxs-lookup"><span data-stu-id="573ed-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="573ed-118">Remover guia</span><span class="sxs-lookup"><span data-stu-id="573ed-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="573ed-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="573ed-119">None</span></span> | <span data-ttu-id="573ed-120">Remove (unpin) uma guia de um canal.</span><span class="sxs-lookup"><span data-stu-id="573ed-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="573ed-121">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="573ed-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="573ed-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="573ed-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="573ed-123">Atualiza as propriedades da guia.</span><span class="sxs-lookup"><span data-stu-id="573ed-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="573ed-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="573ed-124">Properties</span></span>

|<span data-ttu-id="573ed-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="573ed-125">Property</span></span>|<span data-ttu-id="573ed-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="573ed-126">Type</span></span>|<span data-ttu-id="573ed-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="573ed-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="573ed-128">id</span><span class="sxs-lookup"><span data-stu-id="573ed-128">id</span></span>              |   <span data-ttu-id="573ed-129">string</span><span class="sxs-lookup"><span data-stu-id="573ed-129">string</span></span>                  |  <span data-ttu-id="573ed-130">Identificador que identifica exclusivamente uma instância específica de um canal na guia leitura apenas.</span><span class="sxs-lookup"><span data-stu-id="573ed-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="573ed-131">displayName</span><span class="sxs-lookup"><span data-stu-id="573ed-131">displayName</span></span>            |   <span data-ttu-id="573ed-132">string</span><span class="sxs-lookup"><span data-stu-id="573ed-132">string</span></span>                  |  <span data-ttu-id="573ed-133">Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="573ed-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="573ed-134">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="573ed-134">sortOrderIndex</span></span>  |   <span data-ttu-id="573ed-135">inteiro</span><span class="sxs-lookup"><span data-stu-id="573ed-135">int</span></span>                     |  <span data-ttu-id="573ed-136">Índice da ordem usada para classificar as guias</span><span class="sxs-lookup"><span data-stu-id="573ed-136">Index of the order used for sorting tabs</span></span>     |
|  <span data-ttu-id="573ed-137">webUrl</span><span class="sxs-lookup"><span data-stu-id="573ed-137">webUrl</span></span>          |   <span data-ttu-id="573ed-138">string</span><span class="sxs-lookup"><span data-stu-id="573ed-138">string</span></span>                  |  <span data-ttu-id="573ed-139">Link profundo url da instância do guia.</span><span class="sxs-lookup"><span data-stu-id="573ed-139">Deep link url of the tab instance.</span></span> <span data-ttu-id="573ed-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="573ed-140">Read only.</span></span>     |
|  <span data-ttu-id="573ed-141">configuration</span><span class="sxs-lookup"><span data-stu-id="573ed-141">configuration</span></span>        |   [<span data-ttu-id="573ed-142">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="573ed-142">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="573ed-143">Contêiner de configurações personalizadas aplicadas a uma guia. Na guia é considerada configurado somente depois que essa propriedade for definida.</span><span class="sxs-lookup"><span data-stu-id="573ed-143">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="573ed-144">Relações</span><span class="sxs-lookup"><span data-stu-id="573ed-144">Relationships</span></span>

| <span data-ttu-id="573ed-145">Relação</span><span class="sxs-lookup"><span data-stu-id="573ed-145">Relationship</span></span> | <span data-ttu-id="573ed-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="573ed-146">Type</span></span>   | <span data-ttu-id="573ed-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="573ed-147">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="573ed-148">teamsApp</span><span class="sxs-lookup"><span data-stu-id="573ed-148">teamsApp</span></span>|[<span data-ttu-id="573ed-149">teamsApp</span><span class="sxs-lookup"><span data-stu-id="573ed-149">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="573ed-150">O aplicativo que está vinculado à guia. Isso não pode ser alterado após a criação da guia.</span><span class="sxs-lookup"><span data-stu-id="573ed-150">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="573ed-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="573ed-151">JSON representation</span></span>

<span data-ttu-id="573ed-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="573ed-152">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
  "sortOrderIndex": "string",
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

## <a name="see-also"></a><span data-ttu-id="573ed-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="573ed-153">See also</span></span>

[<span data-ttu-id="573ed-154">Configurando os tipos de guia interna</span><span class="sxs-lookup"><span data-stu-id="573ed-154">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
