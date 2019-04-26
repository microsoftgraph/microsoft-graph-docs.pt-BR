---
title: tipo de recurso teamsTab
description: 'Um teamsTab é uma guia fixa (anexada) a um canal dentro de uma equipe. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 207b9d1d4d27199f07ae22bd47587411f917afae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553642"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="48c92-103">tipo de recurso teamsTab</span><span class="sxs-lookup"><span data-stu-id="48c92-103">teamsTab resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48c92-104">Um teamsTab é uma [guia](../resources/teamstab.md) fixa (anexada) a um [canal](channel.md) dentro de uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="48c92-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="48c92-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="48c92-105">Methods</span></span>

| <span data-ttu-id="48c92-106">Método</span><span class="sxs-lookup"><span data-stu-id="48c92-106">Method</span></span>       | <span data-ttu-id="48c92-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="48c92-107">Return Type</span></span>  |<span data-ttu-id="48c92-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="48c92-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="48c92-109">Listar guias</span><span class="sxs-lookup"><span data-stu-id="48c92-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="48c92-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="48c92-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="48c92-111">Lista guias fixadas a um canal.</span><span class="sxs-lookup"><span data-stu-id="48c92-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="48c92-112">Obter guia</span><span class="sxs-lookup"><span data-stu-id="48c92-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="48c92-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="48c92-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="48c92-114">Lê uma guia fixada a um canal.</span><span class="sxs-lookup"><span data-stu-id="48c92-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="48c92-115">Adicionar guia</span><span class="sxs-lookup"><span data-stu-id="48c92-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="48c92-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="48c92-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="48c92-117">Adiciona (fixa) uma guia a um canal.</span><span class="sxs-lookup"><span data-stu-id="48c92-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="48c92-118">Guia remover</span><span class="sxs-lookup"><span data-stu-id="48c92-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="48c92-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="48c92-119">None</span></span> | <span data-ttu-id="48c92-120">Remove (desfixa) uma guia de um canal.</span><span class="sxs-lookup"><span data-stu-id="48c92-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="48c92-121">Atualizar guia</span><span class="sxs-lookup"><span data-stu-id="48c92-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="48c92-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="48c92-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="48c92-123">Atualiza as propriedades da guia.</span><span class="sxs-lookup"><span data-stu-id="48c92-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="48c92-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48c92-124">Properties</span></span>

|<span data-ttu-id="48c92-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48c92-125">Property</span></span>|<span data-ttu-id="48c92-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="48c92-126">Type</span></span>|<span data-ttu-id="48c92-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="48c92-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="48c92-128">id</span><span class="sxs-lookup"><span data-stu-id="48c92-128">id</span></span>              |   <span data-ttu-id="48c92-129">string</span><span class="sxs-lookup"><span data-stu-id="48c92-129">string</span></span>                  |  <span data-ttu-id="48c92-130">Identificador que identifica exclusivamente uma instância específica de uma guia de canal. somente leitura.</span><span class="sxs-lookup"><span data-stu-id="48c92-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="48c92-131">displayName</span><span class="sxs-lookup"><span data-stu-id="48c92-131">displayName</span></span>            |   <span data-ttu-id="48c92-132">string</span><span class="sxs-lookup"><span data-stu-id="48c92-132">string</span></span>                  |  <span data-ttu-id="48c92-133">Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="48c92-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="48c92-134">name</span><span class="sxs-lookup"><span data-stu-id="48c92-134">name</span></span>            |   <span data-ttu-id="48c92-135">string</span><span class="sxs-lookup"><span data-stu-id="48c92-135">string</span></span>                  |  <span data-ttu-id="48c92-136">Preterido Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="48c92-136">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="48c92-137">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="48c92-137">teamsAppId</span></span>           |   <span data-ttu-id="48c92-138">string</span><span class="sxs-lookup"><span data-stu-id="48c92-138">string</span></span>             |  <span data-ttu-id="48c92-139">Identificador de definição de aplicativo da guia. Este valor não pode ser alterado após a criação de tabulação.</span><span class="sxs-lookup"><span data-stu-id="48c92-139">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="48c92-140">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="48c92-140">sortOrderIndex</span></span>  |   <span data-ttu-id="48c92-141">string</span><span class="sxs-lookup"><span data-stu-id="48c92-141">string</span></span>                  |  <span data-ttu-id="48c92-142">Índice da ordem usada para classificar as guias.</span><span class="sxs-lookup"><span data-stu-id="48c92-142">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="48c92-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="48c92-143">webUrl</span></span>          |   <span data-ttu-id="48c92-144">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48c92-144">string</span></span>                  |  <span data-ttu-id="48c92-145">URL de link profundo da instância de guia.</span><span class="sxs-lookup"><span data-stu-id="48c92-145">Deep link url of the tab instance.</span></span> <span data-ttu-id="48c92-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="48c92-146">Read only.</span></span>     |
|  <span data-ttu-id="48c92-147">Configuration</span><span class="sxs-lookup"><span data-stu-id="48c92-147">configuration</span></span>        |   [<span data-ttu-id="48c92-148">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="48c92-148">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="48c92-149">Contêiner para configurações personalizadas aplicadas a uma guia. A guia é considerada configurada somente quando essa propriedade é definida.</span><span class="sxs-lookup"><span data-stu-id="48c92-149">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="48c92-150">Relações</span><span class="sxs-lookup"><span data-stu-id="48c92-150">Relationships</span></span>

| <span data-ttu-id="48c92-151">Relação</span><span class="sxs-lookup"><span data-stu-id="48c92-151">Relationship</span></span> | <span data-ttu-id="48c92-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="48c92-152">Type</span></span>   | <span data-ttu-id="48c92-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="48c92-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="48c92-154">teamsApp</span><span class="sxs-lookup"><span data-stu-id="48c92-154">teamsApp</span></span>|[<span data-ttu-id="48c92-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="48c92-155">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="48c92-156">O aplicativo que está vinculado à guia.</span><span class="sxs-lookup"><span data-stu-id="48c92-156">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="48c92-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48c92-157">JSON representation</span></span>

<span data-ttu-id="48c92-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48c92-158">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="48c92-159">Confira também</span><span class="sxs-lookup"><span data-stu-id="48c92-159">See also</span></span>

[<span data-ttu-id="48c92-160">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="48c92-160">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
