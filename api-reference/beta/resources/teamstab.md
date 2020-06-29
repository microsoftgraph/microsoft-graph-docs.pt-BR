---
title: tipo de recurso teamsTab
description: 'Um teamsTab é uma guia fixa (anexada) a um canal dentro de uma equipe. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c5d73738a24e0ffd21b259c58ce44cbe000c54df
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909727"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="60b62-103">tipo de recurso teamsTab</span><span class="sxs-lookup"><span data-stu-id="60b62-103">teamsTab resource type</span></span>

<span data-ttu-id="60b62-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60b62-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60b62-105">Um teamsTab é uma [guia](../resources/teamstab.md) fixa (anexada) a um [canal](channel.md) dentro de uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="60b62-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="60b62-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="60b62-106">Methods</span></span>

| <span data-ttu-id="60b62-107">Método</span><span class="sxs-lookup"><span data-stu-id="60b62-107">Method</span></span>       | <span data-ttu-id="60b62-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="60b62-108">Return Type</span></span>  |<span data-ttu-id="60b62-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="60b62-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="60b62-110">Listar guias</span><span class="sxs-lookup"><span data-stu-id="60b62-110">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="60b62-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="60b62-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="60b62-112">Listar guias fixadas a um canal.</span><span class="sxs-lookup"><span data-stu-id="60b62-112">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="60b62-113">Obter guia</span><span class="sxs-lookup"><span data-stu-id="60b62-113">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="60b62-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="60b62-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="60b62-115">Ler uma guia fixada a um canal.</span><span class="sxs-lookup"><span data-stu-id="60b62-115">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="60b62-116">Adicionar guia</span><span class="sxs-lookup"><span data-stu-id="60b62-116">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="60b62-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="60b62-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="60b62-118">Adicionar (fixar) uma guia em um canal.</span><span class="sxs-lookup"><span data-stu-id="60b62-118">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="60b62-119">Excluir guia</span><span class="sxs-lookup"><span data-stu-id="60b62-119">Delete tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="60b62-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="60b62-120">None</span></span> | <span data-ttu-id="60b62-121">Remover (desafixar) uma guia de um canal.</span><span class="sxs-lookup"><span data-stu-id="60b62-121">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="60b62-122">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="60b62-122">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="60b62-123">teamsTab</span><span class="sxs-lookup"><span data-stu-id="60b62-123">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="60b62-124">Atualizar as propriedades da guia.</span><span class="sxs-lookup"><span data-stu-id="60b62-124">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="60b62-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="60b62-125">Properties</span></span>

|<span data-ttu-id="60b62-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60b62-126">Property</span></span>|<span data-ttu-id="60b62-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="60b62-127">Type</span></span>|<span data-ttu-id="60b62-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="60b62-128">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="60b62-129">id</span><span class="sxs-lookup"><span data-stu-id="60b62-129">id</span></span>              |   <span data-ttu-id="60b62-130">string</span><span class="sxs-lookup"><span data-stu-id="60b62-130">string</span></span>                  |  <span data-ttu-id="60b62-131">Identificador que identifica exclusivamente uma instância específica de uma guia de canal. somente leitura.</span><span class="sxs-lookup"><span data-stu-id="60b62-131">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="60b62-132">displayName</span><span class="sxs-lookup"><span data-stu-id="60b62-132">displayName</span></span>            |   <span data-ttu-id="60b62-133">string</span><span class="sxs-lookup"><span data-stu-id="60b62-133">string</span></span>                  |  <span data-ttu-id="60b62-134">Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="60b62-134">Name of the tab.</span></span>     |
|  <span data-ttu-id="60b62-135">nome</span><span class="sxs-lookup"><span data-stu-id="60b62-135">name</span></span>            |   <span data-ttu-id="60b62-136">string</span><span class="sxs-lookup"><span data-stu-id="60b62-136">string</span></span>                  |  <span data-ttu-id="60b62-137">Preterido Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="60b62-137">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="60b62-138">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="60b62-138">teamsAppId</span></span>           |   <span data-ttu-id="60b62-139">string</span><span class="sxs-lookup"><span data-stu-id="60b62-139">string</span></span>             |  <span data-ttu-id="60b62-140">Identificador de definição de aplicativo da guia. Este valor não pode ser alterado após a criação de tabulação.</span><span class="sxs-lookup"><span data-stu-id="60b62-140">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="60b62-141">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="60b62-141">sortOrderIndex</span></span>  |   <span data-ttu-id="60b62-142">string</span><span class="sxs-lookup"><span data-stu-id="60b62-142">string</span></span>                  |  <span data-ttu-id="60b62-143">Índice da ordem usada para classificar as guias.</span><span class="sxs-lookup"><span data-stu-id="60b62-143">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="60b62-144">webUrl</span><span class="sxs-lookup"><span data-stu-id="60b62-144">webUrl</span></span>          |   <span data-ttu-id="60b62-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="60b62-145">string</span></span>                  |  <span data-ttu-id="60b62-146">URL de link profundo da instância de guia.</span><span class="sxs-lookup"><span data-stu-id="60b62-146">Deep link URL of the tab instance.</span></span> <span data-ttu-id="60b62-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="60b62-147">Read only.</span></span>     |
|  <span data-ttu-id="60b62-148">configuration</span><span class="sxs-lookup"><span data-stu-id="60b62-148">configuration</span></span>        |   [<span data-ttu-id="60b62-149">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="60b62-149">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="60b62-150">Contêiner para configurações personalizadas aplicadas a uma guia. A guia é considerada configurada somente quando essa propriedade é definida.</span><span class="sxs-lookup"><span data-stu-id="60b62-150">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="60b62-151">Relações</span><span class="sxs-lookup"><span data-stu-id="60b62-151">Relationships</span></span>

| <span data-ttu-id="60b62-152">Relação</span><span class="sxs-lookup"><span data-stu-id="60b62-152">Relationship</span></span> | <span data-ttu-id="60b62-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="60b62-153">Type</span></span>   | <span data-ttu-id="60b62-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="60b62-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="60b62-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="60b62-155">teamsApp</span></span>|[<span data-ttu-id="60b62-156">teamsApp</span><span class="sxs-lookup"><span data-stu-id="60b62-156">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="60b62-157">O aplicativo que está vinculado à guia.</span><span class="sxs-lookup"><span data-stu-id="60b62-157">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="60b62-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="60b62-158">JSON representation</span></span>

<span data-ttu-id="60b62-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="60b62-159">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{
  "id": "string",
  "displayName": "string",
  "teamsAppId": "string",
  "sortOrderIndex": "string",
  "webUrl": "string",
  "configuration": "teamsTabConfiguration",
  "name": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a><span data-ttu-id="60b62-160">Confira também</span><span class="sxs-lookup"><span data-stu-id="60b62-160">See also</span></span>

[<span data-ttu-id="60b62-161">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="60b62-161">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
