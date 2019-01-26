---
title: tipo de recurso de teamsTab
description: 'Um teamsTab é uma guia que tem fixados (anexado) a um canal de uma equipe. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 207b9d1d4d27199f07ae22bd47587411f917afae
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574947"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="a48c1-103">tipo de recurso de teamsTab</span><span class="sxs-lookup"><span data-stu-id="a48c1-103">teamsTab resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a48c1-104">Um teamsTab é uma [guia](../resources/teamstab.md) que tem fixados (anexado) a um [canal](channel.md) de dentro de uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="a48c1-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="a48c1-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="a48c1-105">Methods</span></span>

| <span data-ttu-id="a48c1-106">Método</span><span class="sxs-lookup"><span data-stu-id="a48c1-106">Method</span></span>       | <span data-ttu-id="a48c1-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a48c1-107">Return Type</span></span>  |<span data-ttu-id="a48c1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a48c1-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a48c1-109">Guias de lista</span><span class="sxs-lookup"><span data-stu-id="a48c1-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="a48c1-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a48c1-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a48c1-111">Guias de listas fixados em um canal.</span><span class="sxs-lookup"><span data-stu-id="a48c1-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="a48c1-112">Obtenha o guia</span><span class="sxs-lookup"><span data-stu-id="a48c1-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="a48c1-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a48c1-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a48c1-114">Lê uma guia fixada em um canal.</span><span class="sxs-lookup"><span data-stu-id="a48c1-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="a48c1-115">Adicionar guia</span><span class="sxs-lookup"><span data-stu-id="a48c1-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="a48c1-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a48c1-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a48c1-117">Adiciona (pins) uma guia em um canal.</span><span class="sxs-lookup"><span data-stu-id="a48c1-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="a48c1-118">Remover guia</span><span class="sxs-lookup"><span data-stu-id="a48c1-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="a48c1-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a48c1-119">None</span></span> | <span data-ttu-id="a48c1-120">Remove (unpin) uma guia de um canal.</span><span class="sxs-lookup"><span data-stu-id="a48c1-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="a48c1-121">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="a48c1-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="a48c1-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a48c1-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a48c1-123">Atualiza as propriedades da guia.</span><span class="sxs-lookup"><span data-stu-id="a48c1-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="a48c1-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a48c1-124">Properties</span></span>

|<span data-ttu-id="a48c1-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a48c1-125">Property</span></span>|<span data-ttu-id="a48c1-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a48c1-126">Type</span></span>|<span data-ttu-id="a48c1-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a48c1-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="a48c1-128">id</span><span class="sxs-lookup"><span data-stu-id="a48c1-128">id</span></span>              |   <span data-ttu-id="a48c1-129">string</span><span class="sxs-lookup"><span data-stu-id="a48c1-129">string</span></span>                  |  <span data-ttu-id="a48c1-130">Identificador que identifica exclusivamente uma instância específica de um canal na guia leitura apenas.</span><span class="sxs-lookup"><span data-stu-id="a48c1-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="a48c1-131">displayName</span><span class="sxs-lookup"><span data-stu-id="a48c1-131">displayName</span></span>            |   <span data-ttu-id="a48c1-132">string</span><span class="sxs-lookup"><span data-stu-id="a48c1-132">string</span></span>                  |  <span data-ttu-id="a48c1-133">Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="a48c1-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="a48c1-134">name</span><span class="sxs-lookup"><span data-stu-id="a48c1-134">name</span></span>            |   <span data-ttu-id="a48c1-135">string</span><span class="sxs-lookup"><span data-stu-id="a48c1-135">string</span></span>                  |  <span data-ttu-id="a48c1-136">(Obsoleto) Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="a48c1-136">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="a48c1-137">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="a48c1-137">teamsAppId</span></span>           |   <span data-ttu-id="a48c1-138">string</span><span class="sxs-lookup"><span data-stu-id="a48c1-138">string</span></span>             |  <span data-ttu-id="a48c1-139">Identificador de definição de aplicativo da guia. Este valor não pode ser alterado após a criação da guia.</span><span class="sxs-lookup"><span data-stu-id="a48c1-139">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="a48c1-140">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="a48c1-140">sortOrderIndex</span></span>  |   <span data-ttu-id="a48c1-141">string</span><span class="sxs-lookup"><span data-stu-id="a48c1-141">string</span></span>                  |  <span data-ttu-id="a48c1-142">Índice da ordem usada para classificar as guias.</span><span class="sxs-lookup"><span data-stu-id="a48c1-142">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="a48c1-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="a48c1-143">webUrl</span></span>          |   <span data-ttu-id="a48c1-144">string</span><span class="sxs-lookup"><span data-stu-id="a48c1-144">string</span></span>                  |  <span data-ttu-id="a48c1-145">Link profundo url da instância do guia.</span><span class="sxs-lookup"><span data-stu-id="a48c1-145">Deep link url of the tab instance.</span></span> <span data-ttu-id="a48c1-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a48c1-146">Read only.</span></span>     |
|  <span data-ttu-id="a48c1-147">configuration</span><span class="sxs-lookup"><span data-stu-id="a48c1-147">configuration</span></span>        |   [<span data-ttu-id="a48c1-148">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="a48c1-148">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="a48c1-149">Contêiner de configurações personalizadas aplicadas a uma guia. Na guia é considerada configurado somente depois que essa propriedade for definida.</span><span class="sxs-lookup"><span data-stu-id="a48c1-149">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="a48c1-150">Relações</span><span class="sxs-lookup"><span data-stu-id="a48c1-150">Relationships</span></span>

| <span data-ttu-id="a48c1-151">Relação</span><span class="sxs-lookup"><span data-stu-id="a48c1-151">Relationship</span></span> | <span data-ttu-id="a48c1-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="a48c1-152">Type</span></span>   | <span data-ttu-id="a48c1-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="a48c1-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a48c1-154">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a48c1-154">teamsApp</span></span>|[<span data-ttu-id="a48c1-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a48c1-155">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="a48c1-156">O aplicativo que está vinculado à guia.</span><span class="sxs-lookup"><span data-stu-id="a48c1-156">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a48c1-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a48c1-157">JSON representation</span></span>

<span data-ttu-id="a48c1-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a48c1-158">The following is a JSON representation of the resource.</span></span>


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
  "configuration" : "teamsTabConfiguration"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstab.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="a48c1-159">Confira também</span><span class="sxs-lookup"><span data-stu-id="a48c1-159">See also</span></span>

[<span data-ttu-id="a48c1-160">Configurando os tipos de guia interna</span><span class="sxs-lookup"><span data-stu-id="a48c1-160">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
