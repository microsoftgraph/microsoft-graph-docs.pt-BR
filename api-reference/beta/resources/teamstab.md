---
title: tipo de recurso teamsTab
description: 'Um teamsTab é uma guia fixa (anexada) a um canal dentro de uma equipe. '
localization_priority: Normal
author: AkJo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 38351b0bde174b03f0e01392e7c8ec9c4df0db44
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660111"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="42a0f-103">tipo de recurso teamsTab</span><span class="sxs-lookup"><span data-stu-id="42a0f-103">teamsTab resource type</span></span>

<span data-ttu-id="42a0f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42a0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42a0f-105">Um teamsTab é uma [guia](../resources/teamstab.md) fixa (anexada) a um [canal](channel.md) dentro de uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="42a0f-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="42a0f-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="42a0f-106">Methods</span></span>

| <span data-ttu-id="42a0f-107">Método</span><span class="sxs-lookup"><span data-stu-id="42a0f-107">Method</span></span>       | <span data-ttu-id="42a0f-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="42a0f-108">Return Type</span></span>  |<span data-ttu-id="42a0f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="42a0f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="42a0f-110">Listar guias no canal</span><span class="sxs-lookup"><span data-stu-id="42a0f-110">List tabs in channel</span></span>](../api/channel-list-tabs.md) | [<span data-ttu-id="42a0f-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="42a0f-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="42a0f-112">Listar guias fixadas a um canal.</span><span class="sxs-lookup"><span data-stu-id="42a0f-112">List tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="42a0f-113">Guia obter no canal</span><span class="sxs-lookup"><span data-stu-id="42a0f-113">Get tab in channel</span></span>](../api/channel-get-tabs.md) | [<span data-ttu-id="42a0f-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="42a0f-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="42a0f-115">Ler uma guia fixada a um canal.</span><span class="sxs-lookup"><span data-stu-id="42a0f-115">Get a specific tab pinned to a channel.</span></span>|
|[<span data-ttu-id="42a0f-116">Adicionar uma guia ao canal</span><span class="sxs-lookup"><span data-stu-id="42a0f-116">Add tab to channel</span></span>](../api/channel-post-tabs.md) | [<span data-ttu-id="42a0f-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="42a0f-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="42a0f-118">Adicionar (fixar) uma guia a um canal.</span><span class="sxs-lookup"><span data-stu-id="42a0f-118">Add (pin) a tab to a channel.</span></span>|
|[<span data-ttu-id="42a0f-119">Guia atualizar no canal</span><span class="sxs-lookup"><span data-stu-id="42a0f-119">Update tab in channel</span></span>](../api/channel-patch-tabs.md) | [<span data-ttu-id="42a0f-120">teamsTab</span><span class="sxs-lookup"><span data-stu-id="42a0f-120">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="42a0f-121">Atualiza as propriedades de uma guia em um canal.</span><span class="sxs-lookup"><span data-stu-id="42a0f-121">Updates the properties of a tab in a channel.</span></span>|
|[<span data-ttu-id="42a0f-122">Remover guia do canal</span><span class="sxs-lookup"><span data-stu-id="42a0f-122">Remove tab from channel</span></span>](../api/channel-delete-tabs.md) | <span data-ttu-id="42a0f-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="42a0f-123">None</span></span> | <span data-ttu-id="42a0f-124">Remover (Desafixar) uma Tabulação de um canal.</span><span class="sxs-lookup"><span data-stu-id="42a0f-124">Remove (unpin) a tab from a channel.</span></span>|
|[<span data-ttu-id="42a0f-125">Guias de lista no chat</span><span class="sxs-lookup"><span data-stu-id="42a0f-125">List tabs in chat</span></span>](../api/chat-list-tabs.md) | [<span data-ttu-id="42a0f-126">teamsTab</span><span class="sxs-lookup"><span data-stu-id="42a0f-126">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="42a0f-127">Listar guias fixadas a um chat.</span><span class="sxs-lookup"><span data-stu-id="42a0f-127">List tabs pinned to a chat.</span></span>|
|[<span data-ttu-id="42a0f-128">Guia obter no chat</span><span class="sxs-lookup"><span data-stu-id="42a0f-128">Get tab in chat</span></span>](../api/chat-get-tabs.md) | [<span data-ttu-id="42a0f-129">teamsTab</span><span class="sxs-lookup"><span data-stu-id="42a0f-129">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="42a0f-130">Obtenha uma guia específica fixada para um chat.</span><span class="sxs-lookup"><span data-stu-id="42a0f-130">Get a specific tab pinned to a chat.</span></span>|
|[<span data-ttu-id="42a0f-131">Adicionar guia ao chat</span><span class="sxs-lookup"><span data-stu-id="42a0f-131">Add tab to chat</span></span>](../api/chat-post-tabs.md) | [<span data-ttu-id="42a0f-132">teamsTab</span><span class="sxs-lookup"><span data-stu-id="42a0f-132">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="42a0f-133">Adicionar (fixar) uma guia a um chat.</span><span class="sxs-lookup"><span data-stu-id="42a0f-133">Add (pin) a tab to a chat.</span></span>|
|[<span data-ttu-id="42a0f-134">Guia atualizar no chat</span><span class="sxs-lookup"><span data-stu-id="42a0f-134">Update tab in chat</span></span>](../api/chat-patch-tabs.md) | [<span data-ttu-id="42a0f-135">teamsTab</span><span class="sxs-lookup"><span data-stu-id="42a0f-135">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="42a0f-136">Atualizar as propriedades de uma guia em um chat.</span><span class="sxs-lookup"><span data-stu-id="42a0f-136">Update the properties of a tab in a chat.</span></span>|
|[<span data-ttu-id="42a0f-137">Guia remover do chat</span><span class="sxs-lookup"><span data-stu-id="42a0f-137">Remove tab from chat</span></span>](../api/chat-delete-tabs.md) | <span data-ttu-id="42a0f-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="42a0f-138">None</span></span> | <span data-ttu-id="42a0f-139">Remover (Desafixar) uma guia de um chat.</span><span class="sxs-lookup"><span data-stu-id="42a0f-139">Remove (unpin) a tab from a chat.</span></span>|



## <a name="properties"></a><span data-ttu-id="42a0f-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42a0f-140">Properties</span></span>

|<span data-ttu-id="42a0f-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42a0f-141">Property</span></span>|<span data-ttu-id="42a0f-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="42a0f-142">Type</span></span>|<span data-ttu-id="42a0f-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="42a0f-143">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="42a0f-144">id</span><span class="sxs-lookup"><span data-stu-id="42a0f-144">id</span></span>              |   <span data-ttu-id="42a0f-145">string</span><span class="sxs-lookup"><span data-stu-id="42a0f-145">string</span></span>                  |  <span data-ttu-id="42a0f-146">Identificador que identifica exclusivamente uma instância específica de uma guia de canal. somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42a0f-146">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="42a0f-147">displayName</span><span class="sxs-lookup"><span data-stu-id="42a0f-147">displayName</span></span>            |   <span data-ttu-id="42a0f-148">string</span><span class="sxs-lookup"><span data-stu-id="42a0f-148">string</span></span>                  |  <span data-ttu-id="42a0f-149">Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="42a0f-149">Name of the tab.</span></span>     |
|  <span data-ttu-id="42a0f-150">nome (preterido)</span><span class="sxs-lookup"><span data-stu-id="42a0f-150">name (deprecated)</span></span>      |   <span data-ttu-id="42a0f-151">string</span><span class="sxs-lookup"><span data-stu-id="42a0f-151">string</span></span>                  |  <span data-ttu-id="42a0f-152">Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="42a0f-152">Name of the tab.</span></span>     |
|  <span data-ttu-id="42a0f-153">teamsAppId (preterido)</span><span class="sxs-lookup"><span data-stu-id="42a0f-153">teamsAppId (deprecated)</span></span>|   <span data-ttu-id="42a0f-154">string</span><span class="sxs-lookup"><span data-stu-id="42a0f-154">string</span></span>             |  <span data-ttu-id="42a0f-155">Identificador de definição de aplicativo da guia. Este valor não pode ser alterado após a criação de tabulação.</span><span class="sxs-lookup"><span data-stu-id="42a0f-155">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span> <span data-ttu-id="42a0f-156">Como essa propriedade foi preterida, recomendamos expandir **teamsApp** para recuperar o aplicativo vinculado à guia.</span><span class="sxs-lookup"><span data-stu-id="42a0f-156">Because this property is deprecated, we recommend expanding **teamsApp** to retrieve the application that is linked to the tab.</span></span> |
|  <span data-ttu-id="42a0f-157">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="42a0f-157">sortOrderIndex</span></span>  |   <span data-ttu-id="42a0f-158">string</span><span class="sxs-lookup"><span data-stu-id="42a0f-158">string</span></span>                  |  <span data-ttu-id="42a0f-159">Índice da ordem usada para classificar as guias.</span><span class="sxs-lookup"><span data-stu-id="42a0f-159">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="42a0f-160">webUrl</span><span class="sxs-lookup"><span data-stu-id="42a0f-160">webUrl</span></span>          |   <span data-ttu-id="42a0f-161">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42a0f-161">string</span></span>                  |  <span data-ttu-id="42a0f-162">URL de link profundo da instância de guia.</span><span class="sxs-lookup"><span data-stu-id="42a0f-162">Deep link URL of the tab instance.</span></span> <span data-ttu-id="42a0f-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42a0f-163">Read only.</span></span>     |
|  <span data-ttu-id="42a0f-164">configuração</span><span class="sxs-lookup"><span data-stu-id="42a0f-164">configuration</span></span>        |   [<span data-ttu-id="42a0f-165">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="42a0f-165">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="42a0f-166">Contêiner para configurações personalizadas aplicadas a uma guia. A guia é considerada configurada somente quando essa propriedade é definida.</span><span class="sxs-lookup"><span data-stu-id="42a0f-166">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="42a0f-167">Relações</span><span class="sxs-lookup"><span data-stu-id="42a0f-167">Relationships</span></span>

| <span data-ttu-id="42a0f-168">Relação</span><span class="sxs-lookup"><span data-stu-id="42a0f-168">Relationship</span></span> | <span data-ttu-id="42a0f-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="42a0f-169">Type</span></span>   | <span data-ttu-id="42a0f-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="42a0f-170">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="42a0f-171">teamsApp</span><span class="sxs-lookup"><span data-stu-id="42a0f-171">teamsApp</span></span>|[<span data-ttu-id="42a0f-172">teamsApp</span><span class="sxs-lookup"><span data-stu-id="42a0f-172">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="42a0f-173">O aplicativo que está vinculado à guia.</span><span class="sxs-lookup"><span data-stu-id="42a0f-173">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="42a0f-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42a0f-174">JSON representation</span></span>

<span data-ttu-id="42a0f-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42a0f-175">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="42a0f-176">Confira também</span><span class="sxs-lookup"><span data-stu-id="42a0f-176">See also</span></span>

[<span data-ttu-id="42a0f-177">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="42a0f-177">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)


