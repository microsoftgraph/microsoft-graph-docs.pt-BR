---
title: tipo de recurso teamsTab
description: 'Um teamsTab é uma guia fixa (anexada) a um canal dentro de uma equipe. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 318e3df2d643011537c5d1d9597910fc6b045362
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007645"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="a551b-103">tipo de recurso teamsTab</span><span class="sxs-lookup"><span data-stu-id="a551b-103">teamsTab resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a551b-104">Um teamsTab é uma [guia](../resources/teamstab.md) fixa (anexada) a um [canal](channel.md) dentro de uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="a551b-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="a551b-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="a551b-105">Methods</span></span>

| <span data-ttu-id="a551b-106">Método</span><span class="sxs-lookup"><span data-stu-id="a551b-106">Method</span></span>       | <span data-ttu-id="a551b-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a551b-107">Return Type</span></span>  |<span data-ttu-id="a551b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a551b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a551b-109">Listar guias</span><span class="sxs-lookup"><span data-stu-id="a551b-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="a551b-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a551b-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a551b-111">Listar guias fixadas a um canal.</span><span class="sxs-lookup"><span data-stu-id="a551b-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="a551b-112">Obter guia</span><span class="sxs-lookup"><span data-stu-id="a551b-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="a551b-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a551b-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a551b-114">Ler uma guia fixada a um canal.</span><span class="sxs-lookup"><span data-stu-id="a551b-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="a551b-115">Adicionar guia</span><span class="sxs-lookup"><span data-stu-id="a551b-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="a551b-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a551b-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a551b-117">Adicionar (fixar) uma guia em um canal.</span><span class="sxs-lookup"><span data-stu-id="a551b-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="a551b-118">Remover guia</span><span class="sxs-lookup"><span data-stu-id="a551b-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="a551b-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a551b-119">None</span></span> | <span data-ttu-id="a551b-120">Remover (desafixar) uma guia de um canal.</span><span class="sxs-lookup"><span data-stu-id="a551b-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="a551b-121">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="a551b-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="a551b-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a551b-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a551b-123">Atualizar as propriedades da guia.</span><span class="sxs-lookup"><span data-stu-id="a551b-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="a551b-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a551b-124">Properties</span></span>

|<span data-ttu-id="a551b-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a551b-125">Property</span></span>|<span data-ttu-id="a551b-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a551b-126">Type</span></span>|<span data-ttu-id="a551b-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a551b-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="a551b-128">id</span><span class="sxs-lookup"><span data-stu-id="a551b-128">id</span></span>              |   <span data-ttu-id="a551b-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a551b-129">string</span></span>                  |  <span data-ttu-id="a551b-130">Identificador que identifica exclusivamente uma instância específica de uma guia de canal. somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a551b-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="a551b-131">displayName</span><span class="sxs-lookup"><span data-stu-id="a551b-131">displayName</span></span>            |   <span data-ttu-id="a551b-132">string</span><span class="sxs-lookup"><span data-stu-id="a551b-132">string</span></span>                  |  <span data-ttu-id="a551b-133">Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="a551b-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="a551b-134">name</span><span class="sxs-lookup"><span data-stu-id="a551b-134">name</span></span>            |   <span data-ttu-id="a551b-135">string</span><span class="sxs-lookup"><span data-stu-id="a551b-135">string</span></span>                  |  <span data-ttu-id="a551b-136">Preterido Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="a551b-136">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="a551b-137">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="a551b-137">teamsAppId</span></span>           |   <span data-ttu-id="a551b-138">string</span><span class="sxs-lookup"><span data-stu-id="a551b-138">string</span></span>             |  <span data-ttu-id="a551b-139">Identificador de definição de aplicativo da guia. Este valor não pode ser alterado após a criação de tabulação.</span><span class="sxs-lookup"><span data-stu-id="a551b-139">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="a551b-140">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="a551b-140">sortOrderIndex</span></span>  |   <span data-ttu-id="a551b-141">string</span><span class="sxs-lookup"><span data-stu-id="a551b-141">string</span></span>                  |  <span data-ttu-id="a551b-142">Índice da ordem usada para classificar as guias.</span><span class="sxs-lookup"><span data-stu-id="a551b-142">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="a551b-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="a551b-143">webUrl</span></span>          |   <span data-ttu-id="a551b-144">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a551b-144">string</span></span>                  |  <span data-ttu-id="a551b-145">URL de link profundo da instância de guia.</span><span class="sxs-lookup"><span data-stu-id="a551b-145">Deep link url of the tab instance.</span></span> <span data-ttu-id="a551b-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a551b-146">Read only.</span></span>     |
|  <span data-ttu-id="a551b-147">Configuration</span><span class="sxs-lookup"><span data-stu-id="a551b-147">configuration</span></span>        |   [<span data-ttu-id="a551b-148">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="a551b-148">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="a551b-149">Contêiner para configurações personalizadas aplicadas a uma guia. A guia é considerada configurada somente quando essa propriedade é definida.</span><span class="sxs-lookup"><span data-stu-id="a551b-149">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="a551b-150">Relações</span><span class="sxs-lookup"><span data-stu-id="a551b-150">Relationships</span></span>

| <span data-ttu-id="a551b-151">Relação</span><span class="sxs-lookup"><span data-stu-id="a551b-151">Relationship</span></span> | <span data-ttu-id="a551b-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="a551b-152">Type</span></span>   | <span data-ttu-id="a551b-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="a551b-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a551b-154">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a551b-154">teamsApp</span></span>|[<span data-ttu-id="a551b-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a551b-155">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="a551b-156">O aplicativo que está vinculado à guia.</span><span class="sxs-lookup"><span data-stu-id="a551b-156">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a551b-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a551b-157">JSON representation</span></span>

<span data-ttu-id="a551b-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a551b-158">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="a551b-159">Confira também</span><span class="sxs-lookup"><span data-stu-id="a551b-159">See also</span></span>

[<span data-ttu-id="a551b-160">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="a551b-160">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
