---
title: tipo de recurso teamsTab
description: 'Um teamsTab é uma guia fixa (anexada) a um canal dentro de uma equipe. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5684c98f15ed039fbba36b1df517a6d7d1d5d8c9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046444"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="2760e-103">tipo de recurso teamsTab</span><span class="sxs-lookup"><span data-stu-id="2760e-103">teamsTab resource type</span></span>

<span data-ttu-id="2760e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2760e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2760e-105">Um teamsTab é uma [guia](../resources/teamstab.md) fixa (anexada) a um [canal](channel.md) dentro de uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="2760e-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="2760e-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="2760e-106">Methods</span></span>

| <span data-ttu-id="2760e-107">Método</span><span class="sxs-lookup"><span data-stu-id="2760e-107">Method</span></span>       | <span data-ttu-id="2760e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2760e-108">Return Type</span></span>  |<span data-ttu-id="2760e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2760e-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2760e-110">Listar guias</span><span class="sxs-lookup"><span data-stu-id="2760e-110">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="2760e-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="2760e-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="2760e-112">Listar guias fixadas a um canal.</span><span class="sxs-lookup"><span data-stu-id="2760e-112">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="2760e-113">Obter guia</span><span class="sxs-lookup"><span data-stu-id="2760e-113">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="2760e-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="2760e-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="2760e-115">Ler uma guia fixada a um canal.</span><span class="sxs-lookup"><span data-stu-id="2760e-115">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="2760e-116">Adicionar guia</span><span class="sxs-lookup"><span data-stu-id="2760e-116">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="2760e-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="2760e-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="2760e-118">Adicionar (fixar) uma guia em um canal.</span><span class="sxs-lookup"><span data-stu-id="2760e-118">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="2760e-119">Excluir guia</span><span class="sxs-lookup"><span data-stu-id="2760e-119">Delete tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="2760e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2760e-120">None</span></span> | <span data-ttu-id="2760e-121">Remover (desafixar) uma guia de um canal.</span><span class="sxs-lookup"><span data-stu-id="2760e-121">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="2760e-122">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="2760e-122">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="2760e-123">teamsTab</span><span class="sxs-lookup"><span data-stu-id="2760e-123">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="2760e-124">Atualizar as propriedades da guia.</span><span class="sxs-lookup"><span data-stu-id="2760e-124">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="2760e-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2760e-125">Properties</span></span>

|<span data-ttu-id="2760e-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2760e-126">Property</span></span>|<span data-ttu-id="2760e-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="2760e-127">Type</span></span>|<span data-ttu-id="2760e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="2760e-128">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="2760e-129">id</span><span class="sxs-lookup"><span data-stu-id="2760e-129">id</span></span>              |   <span data-ttu-id="2760e-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2760e-130">string</span></span>                  |  <span data-ttu-id="2760e-131">Identificador que identifica exclusivamente uma instância específica de uma guia de canal. somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2760e-131">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="2760e-132">displayName</span><span class="sxs-lookup"><span data-stu-id="2760e-132">displayName</span></span>            |   <span data-ttu-id="2760e-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2760e-133">string</span></span>                  |  <span data-ttu-id="2760e-134">Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="2760e-134">Name of the tab.</span></span>     |
|  <span data-ttu-id="2760e-135">nome</span><span class="sxs-lookup"><span data-stu-id="2760e-135">name</span></span>            |   <span data-ttu-id="2760e-136">string</span><span class="sxs-lookup"><span data-stu-id="2760e-136">string</span></span>                  |  <span data-ttu-id="2760e-137">Preterido Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="2760e-137">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="2760e-138">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="2760e-138">teamsAppId</span></span>           |   <span data-ttu-id="2760e-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2760e-139">string</span></span>             |  <span data-ttu-id="2760e-140">Identificador de definição de aplicativo da guia. Este valor não pode ser alterado após a criação de tabulação.</span><span class="sxs-lookup"><span data-stu-id="2760e-140">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="2760e-141">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="2760e-141">sortOrderIndex</span></span>  |   <span data-ttu-id="2760e-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2760e-142">string</span></span>                  |  <span data-ttu-id="2760e-143">Índice da ordem usada para classificar as guias.</span><span class="sxs-lookup"><span data-stu-id="2760e-143">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="2760e-144">webUrl</span><span class="sxs-lookup"><span data-stu-id="2760e-144">webUrl</span></span>          |   <span data-ttu-id="2760e-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2760e-145">string</span></span>                  |  <span data-ttu-id="2760e-146">URL de link profundo da instância de guia.</span><span class="sxs-lookup"><span data-stu-id="2760e-146">Deep link URL of the tab instance.</span></span> <span data-ttu-id="2760e-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2760e-147">Read only.</span></span>     |
|  <span data-ttu-id="2760e-148">configuration</span><span class="sxs-lookup"><span data-stu-id="2760e-148">configuration</span></span>        |   [<span data-ttu-id="2760e-149">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="2760e-149">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="2760e-150">Contêiner para configurações personalizadas aplicadas a uma guia. A guia é considerada configurada somente quando essa propriedade é definida.</span><span class="sxs-lookup"><span data-stu-id="2760e-150">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="2760e-151">Relações</span><span class="sxs-lookup"><span data-stu-id="2760e-151">Relationships</span></span>

| <span data-ttu-id="2760e-152">Relação</span><span class="sxs-lookup"><span data-stu-id="2760e-152">Relationship</span></span> | <span data-ttu-id="2760e-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="2760e-153">Type</span></span>   | <span data-ttu-id="2760e-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="2760e-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2760e-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2760e-155">teamsApp</span></span>|[<span data-ttu-id="2760e-156">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2760e-156">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="2760e-157">O aplicativo que está vinculado à guia.</span><span class="sxs-lookup"><span data-stu-id="2760e-157">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2760e-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2760e-158">JSON representation</span></span>

<span data-ttu-id="2760e-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2760e-159">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="2760e-160">Confira também</span><span class="sxs-lookup"><span data-stu-id="2760e-160">See also</span></span>

[<span data-ttu-id="2760e-161">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="2760e-161">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)


