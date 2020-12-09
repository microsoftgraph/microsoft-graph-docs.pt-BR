---
title: tipo de recurso teamsTab
description: 'Um teamsTab é uma guia fixa (anexada) a um canal dentro de uma equipe. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fa675992401c8953b5611739ba69cb0d5688f833
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606948"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="8e9fd-103">tipo de recurso teamsTab</span><span class="sxs-lookup"><span data-stu-id="8e9fd-103">teamsTab resource type</span></span>

<span data-ttu-id="8e9fd-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8e9fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e9fd-105">Um teamsTab é uma [guia](../resources/teamstab.md) fixa (anexada) a um [canal](channel.md) dentro de uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="8e9fd-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="8e9fd-106">Methods</span><span class="sxs-lookup"><span data-stu-id="8e9fd-106">Methods</span></span>

| <span data-ttu-id="8e9fd-107">Método</span><span class="sxs-lookup"><span data-stu-id="8e9fd-107">Method</span></span>       | <span data-ttu-id="8e9fd-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8e9fd-108">Return Type</span></span>  |<span data-ttu-id="8e9fd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e9fd-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8e9fd-110">Listar guias no canal</span><span class="sxs-lookup"><span data-stu-id="8e9fd-110">List tabs in channel</span></span>](../api/channel-list-tabs.md) | [<span data-ttu-id="8e9fd-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8e9fd-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="8e9fd-112">Listar guias fixadas a um canal.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-112">List tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="8e9fd-113">Guia obter no canal</span><span class="sxs-lookup"><span data-stu-id="8e9fd-113">Get tab in channel</span></span>](../api/channel-get-tabs.md) | [<span data-ttu-id="8e9fd-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8e9fd-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="8e9fd-115">Obtenha uma guia específica fixada a um canal.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-115">Get a specific tab pinned to a channel.</span></span>|
|[<span data-ttu-id="8e9fd-116">Adicionar uma guia ao canal</span><span class="sxs-lookup"><span data-stu-id="8e9fd-116">Add tab to channel</span></span>](../api/channel-post-tabs.md) | [<span data-ttu-id="8e9fd-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8e9fd-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="8e9fd-118">Adicionar (fixar) uma guia a um canal.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-118">Add (pin) a tab to a channel.</span></span>|
|[<span data-ttu-id="8e9fd-119">Guia atualizar no canal</span><span class="sxs-lookup"><span data-stu-id="8e9fd-119">Update tab in channel</span></span>](../api/channel-patch-tabs.md) | [<span data-ttu-id="8e9fd-120">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8e9fd-120">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="8e9fd-121">Atualiza as propriedades de uma guia em um canal.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-121">Updates the properties of a tab in a channel.</span></span>|
|[<span data-ttu-id="8e9fd-122">Remover guia do canal</span><span class="sxs-lookup"><span data-stu-id="8e9fd-122">Remove tab from channel</span></span>](../api/channel-delete-tabs.md) | <span data-ttu-id="8e9fd-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e9fd-123">None</span></span> | <span data-ttu-id="8e9fd-124">Remover (Desafixar) uma Tabulação de um canal.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-124">Remove (unpin) a tab from a channel.</span></span>|
|[<span data-ttu-id="8e9fd-125">Guias de lista no chat</span><span class="sxs-lookup"><span data-stu-id="8e9fd-125">List tabs in chat</span></span>](../api/chat-list-tabs.md) | [<span data-ttu-id="8e9fd-126">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8e9fd-126">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="8e9fd-127">Listar guias fixadas a um chat.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-127">List tabs pinned to a chat.</span></span>|
|[<span data-ttu-id="8e9fd-128">Guia obter no chat</span><span class="sxs-lookup"><span data-stu-id="8e9fd-128">Get tab in chat</span></span>](../api/chat-get-tabs.md) | [<span data-ttu-id="8e9fd-129">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8e9fd-129">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="8e9fd-130">Obtenha uma guia específica fixada para um chat.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-130">Get a specific tab pinned to a chat.</span></span>|
|[<span data-ttu-id="8e9fd-131">Adicionar guia ao chat</span><span class="sxs-lookup"><span data-stu-id="8e9fd-131">Add tab to chat</span></span>](../api/chat-post-tabs.md) | [<span data-ttu-id="8e9fd-132">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8e9fd-132">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="8e9fd-133">Adicionar (fixar) uma guia a um chat.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-133">Add (pin) a tab to a chat.</span></span>|
|[<span data-ttu-id="8e9fd-134">Guia atualizar no chat</span><span class="sxs-lookup"><span data-stu-id="8e9fd-134">Update tab in chat</span></span>](../api/chat-patch-tabs.md) | [<span data-ttu-id="8e9fd-135">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8e9fd-135">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="8e9fd-136">Atualiza as propriedades de uma guia em um chat.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-136">Updates the properties of a tab in a chat.</span></span>|
|[<span data-ttu-id="8e9fd-137">Guia remover do chat</span><span class="sxs-lookup"><span data-stu-id="8e9fd-137">Remove tab from chat</span></span>](../api/chat-delete-tabs.md) | <span data-ttu-id="8e9fd-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e9fd-138">None</span></span> | <span data-ttu-id="8e9fd-139">Remover (Desafixar) uma guia de um chat.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-139">Remove (unpin) a tab from a chat.</span></span>|



## <a name="properties"></a><span data-ttu-id="8e9fd-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e9fd-140">Properties</span></span>

|<span data-ttu-id="8e9fd-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e9fd-141">Property</span></span>|<span data-ttu-id="8e9fd-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e9fd-142">Type</span></span>|<span data-ttu-id="8e9fd-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e9fd-143">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="8e9fd-144">id</span><span class="sxs-lookup"><span data-stu-id="8e9fd-144">id</span></span>              |   <span data-ttu-id="8e9fd-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e9fd-145">string</span></span>                  |  <span data-ttu-id="8e9fd-146">Identificador que identifica exclusivamente uma instância específica de uma guia de canal. somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-146">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="8e9fd-147">displayName</span><span class="sxs-lookup"><span data-stu-id="8e9fd-147">displayName</span></span>            |   <span data-ttu-id="8e9fd-148">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e9fd-148">string</span></span>                  |  <span data-ttu-id="8e9fd-149">Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-149">Name of the tab.</span></span>     |
|  <span data-ttu-id="8e9fd-150">nome (preterido)</span><span class="sxs-lookup"><span data-stu-id="8e9fd-150">name (deprecated)</span></span>      |   <span data-ttu-id="8e9fd-151">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e9fd-151">string</span></span>                  |  <span data-ttu-id="8e9fd-152">Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-152">Name of the tab.</span></span>     |
|  <span data-ttu-id="8e9fd-153">teamsAppId (preterido)</span><span class="sxs-lookup"><span data-stu-id="8e9fd-153">teamsAppId (deprecated)</span></span>|   <span data-ttu-id="8e9fd-154">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e9fd-154">string</span></span>             |  <span data-ttu-id="8e9fd-155">Identificador de definição de aplicativo da guia. Este valor não pode ser alterado após a criação de tabulação.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-155">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span> <span data-ttu-id="8e9fd-156">Como essa propriedade foi preterida, recomendamos expandir **teamsApp** para recuperar o aplicativo vinculado à guia.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-156">Because this property is deprecated, we recommend expanding **teamsApp** to retrieve the application that is linked to the tab.</span></span> |
|  <span data-ttu-id="8e9fd-157">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="8e9fd-157">sortOrderIndex</span></span>  |   <span data-ttu-id="8e9fd-158">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e9fd-158">string</span></span>                  |  <span data-ttu-id="8e9fd-159">Índice da ordem usada para classificar as guias.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-159">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="8e9fd-160">webUrl</span><span class="sxs-lookup"><span data-stu-id="8e9fd-160">webUrl</span></span>          |   <span data-ttu-id="8e9fd-161">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e9fd-161">string</span></span>                  |  <span data-ttu-id="8e9fd-162">URL de link profundo da instância de guia.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-162">Deep link URL of the tab instance.</span></span> <span data-ttu-id="8e9fd-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-163">Read only.</span></span>     |
|  <span data-ttu-id="8e9fd-164">configuration</span><span class="sxs-lookup"><span data-stu-id="8e9fd-164">configuration</span></span>        |   [<span data-ttu-id="8e9fd-165">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="8e9fd-165">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="8e9fd-166">Contêiner para configurações personalizadas aplicadas a uma guia. A guia é considerada configurada somente quando essa propriedade é definida.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-166">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="8e9fd-167">Relações</span><span class="sxs-lookup"><span data-stu-id="8e9fd-167">Relationships</span></span>

| <span data-ttu-id="8e9fd-168">Relação</span><span class="sxs-lookup"><span data-stu-id="8e9fd-168">Relationship</span></span> | <span data-ttu-id="8e9fd-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e9fd-169">Type</span></span>   | <span data-ttu-id="8e9fd-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e9fd-170">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8e9fd-171">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8e9fd-171">teamsApp</span></span>|[<span data-ttu-id="8e9fd-172">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8e9fd-172">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="8e9fd-173">O aplicativo que está vinculado à guia.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-173">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8e9fd-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e9fd-174">JSON representation</span></span>

<span data-ttu-id="8e9fd-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e9fd-175">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="8e9fd-176">Confira também</span><span class="sxs-lookup"><span data-stu-id="8e9fd-176">See also</span></span>

[<span data-ttu-id="8e9fd-177">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="8e9fd-177">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)


