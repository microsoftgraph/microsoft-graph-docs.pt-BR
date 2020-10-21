---
title: tipo de recurso teamsTab
description: 'Um teamsTab é uma guia fixa (anexada) a um canal dentro de uma equipe. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c60e47a65c9d5b17433891161fe5c16ca182a5ca
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634659"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="68dbe-103">tipo de recurso teamsTab</span><span class="sxs-lookup"><span data-stu-id="68dbe-103">teamsTab resource type</span></span>

<span data-ttu-id="68dbe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68dbe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68dbe-105">Um teamsTab é uma [guia](../resources/teamstab.md) fixa (anexada) a um [canal](channel.md) dentro de uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="68dbe-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="68dbe-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="68dbe-106">Methods</span></span>

| <span data-ttu-id="68dbe-107">Método</span><span class="sxs-lookup"><span data-stu-id="68dbe-107">Method</span></span>       | <span data-ttu-id="68dbe-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="68dbe-108">Return Type</span></span>  |<span data-ttu-id="68dbe-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="68dbe-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="68dbe-110">Listar guias</span><span class="sxs-lookup"><span data-stu-id="68dbe-110">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="68dbe-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="68dbe-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="68dbe-112">Listar guias fixadas a um canal.</span><span class="sxs-lookup"><span data-stu-id="68dbe-112">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="68dbe-113">Obter guia</span><span class="sxs-lookup"><span data-stu-id="68dbe-113">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="68dbe-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="68dbe-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="68dbe-115">Ler uma guia fixada a um canal.</span><span class="sxs-lookup"><span data-stu-id="68dbe-115">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="68dbe-116">Adicionar guia</span><span class="sxs-lookup"><span data-stu-id="68dbe-116">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="68dbe-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="68dbe-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="68dbe-118">Adicionar (fixar) uma guia em um canal.</span><span class="sxs-lookup"><span data-stu-id="68dbe-118">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="68dbe-119">Excluir guia</span><span class="sxs-lookup"><span data-stu-id="68dbe-119">Delete tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="68dbe-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="68dbe-120">None</span></span> | <span data-ttu-id="68dbe-121">Remover (desafixar) uma guia de um canal.</span><span class="sxs-lookup"><span data-stu-id="68dbe-121">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="68dbe-122">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="68dbe-122">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="68dbe-123">teamsTab</span><span class="sxs-lookup"><span data-stu-id="68dbe-123">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="68dbe-124">Atualizar as propriedades da guia.</span><span class="sxs-lookup"><span data-stu-id="68dbe-124">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="68dbe-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68dbe-125">Properties</span></span>

|<span data-ttu-id="68dbe-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68dbe-126">Property</span></span>|<span data-ttu-id="68dbe-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="68dbe-127">Type</span></span>|<span data-ttu-id="68dbe-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="68dbe-128">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="68dbe-129">id</span><span class="sxs-lookup"><span data-stu-id="68dbe-129">id</span></span>              |   <span data-ttu-id="68dbe-130">string</span><span class="sxs-lookup"><span data-stu-id="68dbe-130">string</span></span>                  |  <span data-ttu-id="68dbe-131">Identificador que identifica exclusivamente uma instância específica de uma guia de canal. somente leitura.</span><span class="sxs-lookup"><span data-stu-id="68dbe-131">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="68dbe-132">displayName</span><span class="sxs-lookup"><span data-stu-id="68dbe-132">displayName</span></span>            |   <span data-ttu-id="68dbe-133">string</span><span class="sxs-lookup"><span data-stu-id="68dbe-133">string</span></span>                  |  <span data-ttu-id="68dbe-134">Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="68dbe-134">Name of the tab.</span></span>     |
|  <span data-ttu-id="68dbe-135">nome (preterido)</span><span class="sxs-lookup"><span data-stu-id="68dbe-135">name (deprecated)</span></span>      |   <span data-ttu-id="68dbe-136">string</span><span class="sxs-lookup"><span data-stu-id="68dbe-136">string</span></span>                  |  <span data-ttu-id="68dbe-137">Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="68dbe-137">Name of the tab.</span></span>     |
|  <span data-ttu-id="68dbe-138">teamsAppId (preterido)</span><span class="sxs-lookup"><span data-stu-id="68dbe-138">teamsAppId (deprecated)</span></span>|   <span data-ttu-id="68dbe-139">string</span><span class="sxs-lookup"><span data-stu-id="68dbe-139">string</span></span>             |  <span data-ttu-id="68dbe-140">Identificador de definição de aplicativo da guia. Este valor não pode ser alterado após a criação de tabulação.</span><span class="sxs-lookup"><span data-stu-id="68dbe-140">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span> <span data-ttu-id="68dbe-141">Como essa propriedade foi preterida, recomendamos expandir **teamsApp** para recuperar o aplicativo vinculado à guia.</span><span class="sxs-lookup"><span data-stu-id="68dbe-141">Because this property is deprecated, we recommend expanding **teamsApp** to retrieve the application that is linked to the tab.</span></span> |
|  <span data-ttu-id="68dbe-142">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="68dbe-142">sortOrderIndex</span></span>  |   <span data-ttu-id="68dbe-143">string</span><span class="sxs-lookup"><span data-stu-id="68dbe-143">string</span></span>                  |  <span data-ttu-id="68dbe-144">Índice da ordem usada para classificar as guias.</span><span class="sxs-lookup"><span data-stu-id="68dbe-144">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="68dbe-145">webUrl</span><span class="sxs-lookup"><span data-stu-id="68dbe-145">webUrl</span></span>          |   <span data-ttu-id="68dbe-146">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68dbe-146">string</span></span>                  |  <span data-ttu-id="68dbe-147">URL de link profundo da instância de guia.</span><span class="sxs-lookup"><span data-stu-id="68dbe-147">Deep link URL of the tab instance.</span></span> <span data-ttu-id="68dbe-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="68dbe-148">Read only.</span></span>     |
|  <span data-ttu-id="68dbe-149">configuration</span><span class="sxs-lookup"><span data-stu-id="68dbe-149">configuration</span></span>        |   [<span data-ttu-id="68dbe-150">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="68dbe-150">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="68dbe-151">Contêiner para configurações personalizadas aplicadas a uma guia. A guia é considerada configurada somente quando essa propriedade é definida.</span><span class="sxs-lookup"><span data-stu-id="68dbe-151">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="68dbe-152">Relações</span><span class="sxs-lookup"><span data-stu-id="68dbe-152">Relationships</span></span>

| <span data-ttu-id="68dbe-153">Relação</span><span class="sxs-lookup"><span data-stu-id="68dbe-153">Relationship</span></span> | <span data-ttu-id="68dbe-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="68dbe-154">Type</span></span>   | <span data-ttu-id="68dbe-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="68dbe-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="68dbe-156">teamsApp</span><span class="sxs-lookup"><span data-stu-id="68dbe-156">teamsApp</span></span>|[<span data-ttu-id="68dbe-157">teamsApp</span><span class="sxs-lookup"><span data-stu-id="68dbe-157">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="68dbe-158">O aplicativo que está vinculado à guia.</span><span class="sxs-lookup"><span data-stu-id="68dbe-158">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="68dbe-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68dbe-159">JSON representation</span></span>

<span data-ttu-id="68dbe-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="68dbe-160">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="68dbe-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="68dbe-161">See also</span></span>

[<span data-ttu-id="68dbe-162">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="68dbe-162">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)


