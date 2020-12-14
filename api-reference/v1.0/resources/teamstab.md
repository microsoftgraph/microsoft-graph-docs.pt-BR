---
title: tipo de recurso teamsTab
description: 'Um teamsTab é uma guia fixa (anexada) a um canal dentro de uma equipe. '
localization_priority: Normal
author: AkJo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8314604d6ed15eeb154ff46c8e3b90f4be4f5cde
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658545"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="eacfa-103">tipo de recurso teamsTab</span><span class="sxs-lookup"><span data-stu-id="eacfa-103">teamsTab resource type</span></span>

<span data-ttu-id="eacfa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eacfa-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="eacfa-105">Um teamsTab é uma [guia](../resources/teamstab.md) fixa (anexada) a um [canal](channel.md) dentro de uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="eacfa-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="eacfa-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="eacfa-106">Methods</span></span>

| <span data-ttu-id="eacfa-107">Método</span><span class="sxs-lookup"><span data-stu-id="eacfa-107">Method</span></span>       | <span data-ttu-id="eacfa-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eacfa-108">Return Type</span></span>  |<span data-ttu-id="eacfa-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="eacfa-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eacfa-110">Listar guias</span><span class="sxs-lookup"><span data-stu-id="eacfa-110">List tabs</span></span>](../api/channel-list-tabs.md) | [<span data-ttu-id="eacfa-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="eacfa-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="eacfa-112">Listar guias fixadas a um canal.</span><span class="sxs-lookup"><span data-stu-id="eacfa-112">List tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="eacfa-113">Obter guia</span><span class="sxs-lookup"><span data-stu-id="eacfa-113">Get tab</span></span>](../api/channel-get-tabs.md) | [<span data-ttu-id="eacfa-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="eacfa-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="eacfa-115">Ler uma guia fixada em um canal.</span><span class="sxs-lookup"><span data-stu-id="eacfa-115">Read a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="eacfa-116">Adicionar guia</span><span class="sxs-lookup"><span data-stu-id="eacfa-116">Add tab</span></span>](../api/channel-post-tabs.md) | [<span data-ttu-id="eacfa-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="eacfa-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="eacfa-118">Adicionar (fixar) uma guia a um canal.</span><span class="sxs-lookup"><span data-stu-id="eacfa-118">Add (pin) a tab to a channel.</span></span>|
|[<span data-ttu-id="eacfa-119">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="eacfa-119">Update tab</span></span>](../api/channel-patch-tabs.md) | [<span data-ttu-id="eacfa-120">teamsTab</span><span class="sxs-lookup"><span data-stu-id="eacfa-120">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="eacfa-121">Atualize as propriedades da guia.</span><span class="sxs-lookup"><span data-stu-id="eacfa-121">Update the tab properties.</span></span>|
|[<span data-ttu-id="eacfa-122">Remover guia</span><span class="sxs-lookup"><span data-stu-id="eacfa-122">Remove tab</span></span>](../api/channel-delete-tabs.md) | <span data-ttu-id="eacfa-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eacfa-123">None</span></span> | <span data-ttu-id="eacfa-124">Remover (Desafixar) uma Tabulação de um canal.</span><span class="sxs-lookup"><span data-stu-id="eacfa-124">Remove (unpin) a tab from a channel.</span></span>|


## <a name="properties"></a><span data-ttu-id="eacfa-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eacfa-125">Properties</span></span>

|<span data-ttu-id="eacfa-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eacfa-126">Property</span></span>|<span data-ttu-id="eacfa-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="eacfa-127">Type</span></span>|<span data-ttu-id="eacfa-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="eacfa-128">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="eacfa-129">id</span><span class="sxs-lookup"><span data-stu-id="eacfa-129">id</span></span>              |   <span data-ttu-id="eacfa-130">string</span><span class="sxs-lookup"><span data-stu-id="eacfa-130">string</span></span>                  |  <span data-ttu-id="eacfa-131">Identificador que identifica exclusivamente uma instância específica de uma guia de canal. somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eacfa-131">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="eacfa-132">displayName</span><span class="sxs-lookup"><span data-stu-id="eacfa-132">displayName</span></span>            |   <span data-ttu-id="eacfa-133">string</span><span class="sxs-lookup"><span data-stu-id="eacfa-133">string</span></span>                  |  <span data-ttu-id="eacfa-134">Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="eacfa-134">Name of the tab.</span></span>     |
|  <span data-ttu-id="eacfa-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="eacfa-135">webUrl</span></span>          |   <span data-ttu-id="eacfa-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eacfa-136">string</span></span>                  |  <span data-ttu-id="eacfa-137">URL de link profundo da instância de guia.</span><span class="sxs-lookup"><span data-stu-id="eacfa-137">Deep link URL of the tab instance.</span></span> <span data-ttu-id="eacfa-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eacfa-138">Read only.</span></span>     |
|  <span data-ttu-id="eacfa-139">configuração</span><span class="sxs-lookup"><span data-stu-id="eacfa-139">configuration</span></span>        |   [<span data-ttu-id="eacfa-140">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="eacfa-140">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="eacfa-141">Contêiner para configurações personalizadas aplicadas a uma guia. A guia é considerada configurada somente quando essa propriedade é definida.</span><span class="sxs-lookup"><span data-stu-id="eacfa-141">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="eacfa-142">Relações</span><span class="sxs-lookup"><span data-stu-id="eacfa-142">Relationships</span></span>

| <span data-ttu-id="eacfa-143">Relação</span><span class="sxs-lookup"><span data-stu-id="eacfa-143">Relationship</span></span> | <span data-ttu-id="eacfa-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="eacfa-144">Type</span></span>   | <span data-ttu-id="eacfa-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="eacfa-145">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="eacfa-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="eacfa-146">teamsApp</span></span>|[<span data-ttu-id="eacfa-147">teamsApp</span><span class="sxs-lookup"><span data-stu-id="eacfa-147">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="eacfa-148">O aplicativo que está vinculado à guia. Isso não pode ser alterado após a criação da Tabulação.</span><span class="sxs-lookup"><span data-stu-id="eacfa-148">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eacfa-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eacfa-149">JSON representation</span></span>

<span data-ttu-id="eacfa-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eacfa-150">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="eacfa-151">Confira também</span><span class="sxs-lookup"><span data-stu-id="eacfa-151">See also</span></span>

[<span data-ttu-id="eacfa-152">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="eacfa-152">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

