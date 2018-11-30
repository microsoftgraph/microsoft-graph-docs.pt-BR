---
title: tipo de recurso de canal
description: 'Um canal é uma coleção de chatMessages dentro de uma equipe. '
ms.openlocfilehash: 90a2c6641a79829e340f2487d7f0381998d2a205
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040288"
---
# <a name="channel-resource-type"></a><span data-ttu-id="99f2f-103">tipo de recurso de canal</span><span class="sxs-lookup"><span data-stu-id="99f2f-103">channel resource type</span></span>

> <span data-ttu-id="99f2f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="99f2f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99f2f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="99f2f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99f2f-106">Um canal é uma coleção de [chatMessages](chatmessage.md) dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="99f2f-106">A channel is a collection of [chatMessages](chatmessage.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="99f2f-107">Um canal representa um tópico e, portanto, um isolamento lógico discussão, dentro de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="99f2f-107">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="99f2f-108">Exemplos podem ser canal "Sexta-feira equipe almoço" e "Discussão sobre a arquitetura" channel.</span><span class="sxs-lookup"><span data-stu-id="99f2f-108">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="99f2f-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="99f2f-109">Methods</span></span>

| <span data-ttu-id="99f2f-110">Método</span><span class="sxs-lookup"><span data-stu-id="99f2f-110">Method</span></span>       | <span data-ttu-id="99f2f-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="99f2f-111">Return Type</span></span>  |<span data-ttu-id="99f2f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="99f2f-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="99f2f-113">Canais de lista</span><span class="sxs-lookup"><span data-stu-id="99f2f-113">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="99f2f-114">coleção de [canal](channel.md)</span><span class="sxs-lookup"><span data-stu-id="99f2f-114">[channel](channel.md) collection</span></span> | <span data-ttu-id="99f2f-115">Obter a lista de canais nesse conjunto.</span><span class="sxs-lookup"><span data-stu-id="99f2f-115">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="99f2f-116">Criar canal</span><span class="sxs-lookup"><span data-stu-id="99f2f-116">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="99f2f-117">canal</span><span class="sxs-lookup"><span data-stu-id="99f2f-117">channel</span></span>](channel.md) | <span data-ttu-id="99f2f-118">Crie um novo canal, incluindo o nome para exibição e a descrição.</span><span class="sxs-lookup"><span data-stu-id="99f2f-118">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="99f2f-119">Obtenha o canal</span><span class="sxs-lookup"><span data-stu-id="99f2f-119">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="99f2f-120">canal</span><span class="sxs-lookup"><span data-stu-id="99f2f-120">channel</span></span>](channel.md) | <span data-ttu-id="99f2f-121">Leia as propriedades e os relacionamentos do canal.</span><span class="sxs-lookup"><span data-stu-id="99f2f-121">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="99f2f-122">Canal de atualização</span><span class="sxs-lookup"><span data-stu-id="99f2f-122">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="99f2f-123">canal</span><span class="sxs-lookup"><span data-stu-id="99f2f-123">channel</span></span>](channel.md) | <span data-ttu-id="99f2f-124">Atualize propriedades do canal.</span><span class="sxs-lookup"><span data-stu-id="99f2f-124">Update properties of the channel.</span></span>|
|[<span data-ttu-id="99f2f-125">Excluir um canal</span><span class="sxs-lookup"><span data-stu-id="99f2f-125">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="99f2f-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99f2f-126">None</span></span> | <span data-ttu-id="99f2f-127">Exclua um canal.</span><span class="sxs-lookup"><span data-stu-id="99f2f-127">Delete a channel.</span></span>|
|[<span data-ttu-id="99f2f-128">Lista de mensagens de canal</span><span class="sxs-lookup"><span data-stu-id="99f2f-128">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="99f2f-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="99f2f-129">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="99f2f-130">Obter mensagens em um canal</span><span class="sxs-lookup"><span data-stu-id="99f2f-130">Get messages in a channel</span></span> |
|[<span data-ttu-id="99f2f-131">Criar thread de bate-papo</span><span class="sxs-lookup"><span data-stu-id="99f2f-131">Create chat thread</span></span>](../api/channel-post-chatthreads.md) | <span data-ttu-id="99f2f-132">coleção [chatThread](chatthread.md)</span><span class="sxs-lookup"><span data-stu-id="99f2f-132">[chatThread](chatthread.md) collection</span></span>| <span data-ttu-id="99f2f-133">Crie um segmento de bate-papo no canal especificado.</span><span class="sxs-lookup"><span data-stu-id="99f2f-133">Create a chat thread in the specified channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="99f2f-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99f2f-134">Properties</span></span>
| <span data-ttu-id="99f2f-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99f2f-135">Property</span></span>     | <span data-ttu-id="99f2f-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="99f2f-136">Type</span></span>   |<span data-ttu-id="99f2f-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="99f2f-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99f2f-138">description</span><span class="sxs-lookup"><span data-stu-id="99f2f-138">description</span></span>|<span data-ttu-id="99f2f-139">String</span><span class="sxs-lookup"><span data-stu-id="99f2f-139">String</span></span>|<span data-ttu-id="99f2f-140">Descrição textual opcional para o canal.</span><span class="sxs-lookup"><span data-stu-id="99f2f-140">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="99f2f-141">displayName</span><span class="sxs-lookup"><span data-stu-id="99f2f-141">displayName</span></span>|<span data-ttu-id="99f2f-142">String</span><span class="sxs-lookup"><span data-stu-id="99f2f-142">String</span></span>|<span data-ttu-id="99f2f-143">Nome de canal como ele será exibido ao usuário no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="99f2f-143">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="99f2f-144">id</span><span class="sxs-lookup"><span data-stu-id="99f2f-144">id</span></span>|<span data-ttu-id="99f2f-145">String</span><span class="sxs-lookup"><span data-stu-id="99f2f-145">String</span></span>|<span data-ttu-id="99f2f-146">Identificador exclusivo dos canais.</span><span class="sxs-lookup"><span data-stu-id="99f2f-146">The channels's unique identifier.</span></span> <span data-ttu-id="99f2f-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="99f2f-147">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99f2f-148">Relações</span><span class="sxs-lookup"><span data-stu-id="99f2f-148">Relationships</span></span>
| <span data-ttu-id="99f2f-149">Relação</span><span class="sxs-lookup"><span data-stu-id="99f2f-149">Relationship</span></span> | <span data-ttu-id="99f2f-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="99f2f-150">Type</span></span>   |<span data-ttu-id="99f2f-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="99f2f-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99f2f-152">mensagens</span><span class="sxs-lookup"><span data-stu-id="99f2f-152">messages</span></span>|<span data-ttu-id="99f2f-153">coleção [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="99f2f-153">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="99f2f-154">Uma coleção de todas as mensagens no canal.</span><span class="sxs-lookup"><span data-stu-id="99f2f-154">A collection of all the messages in the channel.</span></span> <span data-ttu-id="99f2f-155">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="99f2f-155">A navigation property.</span></span> <span data-ttu-id="99f2f-156">Anulável.</span><span class="sxs-lookup"><span data-stu-id="99f2f-156">Nullable.</span></span> <span data-ttu-id="99f2f-157">Atualmente, essa API suporta leitura apenas mas eventualmente dará suporte a mensagens de escrita muito.</span><span class="sxs-lookup"><span data-stu-id="99f2f-157">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="99f2f-158">chatThreads</span><span class="sxs-lookup"><span data-stu-id="99f2f-158">chatThreads</span></span>|<span data-ttu-id="99f2f-159">coleção [chatThread](chatthread.md)</span><span class="sxs-lookup"><span data-stu-id="99f2f-159">[chatThread](chatthread.md) collection</span></span>|<span data-ttu-id="99f2f-160">(Isso é sendo substituídos gradualmente à propriedade mensagens) chatThreads oferece suporte à criação de novas mensagens, mas não a leitura de mensagens.</span><span class="sxs-lookup"><span data-stu-id="99f2f-160">(This is being phased out in favor of the messages property) chatThreads supports creating new messages but not reading messages.</span></span> <span data-ttu-id="99f2f-161">ChatThreads é uma propriedade de navegação e é Nullable.</span><span class="sxs-lookup"><span data-stu-id="99f2f-161">ChatThreads is a navigation property, and is Nullable.</span></span>|
|<span data-ttu-id="99f2f-162">guias</span><span class="sxs-lookup"><span data-stu-id="99f2f-162">tabs</span></span>|<span data-ttu-id="99f2f-163">coleção [teamsTab](../resources/teamstab.md)</span><span class="sxs-lookup"><span data-stu-id="99f2f-163">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="99f2f-164">Uma coleção de todas as guias no canal.</span><span class="sxs-lookup"><span data-stu-id="99f2f-164">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="99f2f-165">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="99f2f-165">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="99f2f-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99f2f-166">JSON representation</span></span>

<span data-ttu-id="99f2f-167">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="99f2f-167">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatthreads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
