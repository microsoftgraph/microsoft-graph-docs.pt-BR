---
title: tipo de recurso de canal
description: 'Um canal é uma coleção de chatMessages dentro de uma equipe. '
author: nkramer
localization_priority: Priority
ms.openlocfilehash: 058632c9f56462195db0cd268fd0af262d4292f3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842682"
---
# <a name="channel-resource-type"></a><span data-ttu-id="ca5f4-103">tipo de recurso de canal</span><span class="sxs-lookup"><span data-stu-id="ca5f4-103">channel resource type</span></span>

> <span data-ttu-id="ca5f4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca5f4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca5f4-106">Um canal é uma coleção de [chatMessages](chatmessage.md) dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="ca5f4-106">A channel is a collection of [chatMessages](chatmessage.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="ca5f4-107">Um canal representa um tópico e, portanto, um isolamento lógico discussão, dentro de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-107">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="ca5f4-108">Exemplos podem ser canal "Sexta-feira equipe almoço" e "Discussão sobre a arquitetura" channel.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-108">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="ca5f4-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="ca5f4-109">Methods</span></span>

| <span data-ttu-id="ca5f4-110">Método</span><span class="sxs-lookup"><span data-stu-id="ca5f4-110">Method</span></span>       | <span data-ttu-id="ca5f4-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ca5f4-111">Return Type</span></span>  |<span data-ttu-id="ca5f4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca5f4-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ca5f4-113">Canais de lista</span><span class="sxs-lookup"><span data-stu-id="ca5f4-113">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="ca5f4-114">coleção de [canal](channel.md)</span><span class="sxs-lookup"><span data-stu-id="ca5f4-114">[channel](channel.md) collection</span></span> | <span data-ttu-id="ca5f4-115">Obter a lista de canais nesse conjunto.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-115">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="ca5f4-116">Criar canal</span><span class="sxs-lookup"><span data-stu-id="ca5f4-116">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="ca5f4-117">canal</span><span class="sxs-lookup"><span data-stu-id="ca5f4-117">channel</span></span>](channel.md) | <span data-ttu-id="ca5f4-118">Crie um novo canal, incluindo o nome para exibição e a descrição.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-118">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="ca5f4-119">Obtenha o canal</span><span class="sxs-lookup"><span data-stu-id="ca5f4-119">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="ca5f4-120">canal</span><span class="sxs-lookup"><span data-stu-id="ca5f4-120">channel</span></span>](channel.md) | <span data-ttu-id="ca5f4-121">Leia as propriedades e os relacionamentos do canal.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-121">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="ca5f4-122">Canal de atualização</span><span class="sxs-lookup"><span data-stu-id="ca5f4-122">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="ca5f4-123">canal</span><span class="sxs-lookup"><span data-stu-id="ca5f4-123">channel</span></span>](channel.md) | <span data-ttu-id="ca5f4-124">Atualize propriedades do canal.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-124">Update properties of the channel.</span></span>|
|[<span data-ttu-id="ca5f4-125">Excluir um canal</span><span class="sxs-lookup"><span data-stu-id="ca5f4-125">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="ca5f4-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ca5f4-126">None</span></span> | <span data-ttu-id="ca5f4-127">Exclua um canal.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-127">Delete a channel.</span></span>|
|[<span data-ttu-id="ca5f4-128">Lista de mensagens de canal</span><span class="sxs-lookup"><span data-stu-id="ca5f4-128">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="ca5f4-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="ca5f4-129">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="ca5f4-130">Obter mensagens em um canal</span><span class="sxs-lookup"><span data-stu-id="ca5f4-130">Get messages in a channel</span></span> |
|[<span data-ttu-id="ca5f4-131">Criar thread de bate-papo</span><span class="sxs-lookup"><span data-stu-id="ca5f4-131">Create chat thread</span></span>](../api/channel-post-chatthreads.md) | <span data-ttu-id="ca5f4-132">coleção [chatThread](chatthread.md)</span><span class="sxs-lookup"><span data-stu-id="ca5f4-132">[chatThread](chatthread.md) collection</span></span>| <span data-ttu-id="ca5f4-133">Crie um segmento de bate-papo no canal especificado.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-133">Create a chat thread in the specified channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="ca5f4-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ca5f4-134">Properties</span></span>
| <span data-ttu-id="ca5f4-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca5f4-135">Property</span></span>     | <span data-ttu-id="ca5f4-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca5f4-136">Type</span></span>   |<span data-ttu-id="ca5f4-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca5f4-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca5f4-138">description</span><span class="sxs-lookup"><span data-stu-id="ca5f4-138">description</span></span>|<span data-ttu-id="ca5f4-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca5f4-139">String</span></span>|<span data-ttu-id="ca5f4-140">Descrição textual opcional para o canal.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-140">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="ca5f4-141">displayName</span><span class="sxs-lookup"><span data-stu-id="ca5f4-141">displayName</span></span>|<span data-ttu-id="ca5f4-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca5f4-142">String</span></span>|<span data-ttu-id="ca5f4-143">Nome de canal como ele será exibido ao usuário no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-143">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="ca5f4-144">id</span><span class="sxs-lookup"><span data-stu-id="ca5f4-144">id</span></span>|<span data-ttu-id="ca5f4-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca5f4-145">String</span></span>|<span data-ttu-id="ca5f4-146">Identificador exclusivo dos canais.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-146">The channels's unique identifier.</span></span> <span data-ttu-id="ca5f4-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-147">Read-only.</span></span>|
|<span data-ttu-id="ca5f4-148">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="ca5f4-148">isFavoriteByDefault</span></span>|<span data-ttu-id="ca5f4-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca5f4-149">Boolean</span></span>|<span data-ttu-id="ca5f4-150">Se o canal deve ser marcado automaticamente 'favorito' para todos os membros da equipe.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-150">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="ca5f4-151">Padrão: `false`.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-151">Default: `false`.</span></span>|
|<span data-ttu-id="ca5f4-152">email</span><span class="sxs-lookup"><span data-stu-id="ca5f4-152">email</span></span>|<span data-ttu-id="ca5f4-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca5f4-153">Boolean</span></span>| <span data-ttu-id="ca5f4-154">O endereço de email de mensagens enviadas para o canal.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-154">The email address for sending messages to the channel.</span></span> <span data-ttu-id="ca5f4-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-155">Read-only.</span></span>|
|<span data-ttu-id="ca5f4-156">webUrl</span><span class="sxs-lookup"><span data-stu-id="ca5f4-156">webUrl</span></span>|<span data-ttu-id="ca5f4-157">String</span><span class="sxs-lookup"><span data-stu-id="ca5f4-157">String</span></span>|<span data-ttu-id="ca5f4-158">Um hiperlink que irá navegar até o canal de Teams da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-158">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="ca5f4-159">Esta é a URL que você obtém quando você um canal em Microsoft Teams do mouse em e selecione o link de Get para canal.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-159">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="ca5f4-160">Essa URL deve ser tratado como um blob opaco e não analisado.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-160">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="ca5f4-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-161">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="ca5f4-162">Relações</span><span class="sxs-lookup"><span data-stu-id="ca5f4-162">Relationships</span></span>
| <span data-ttu-id="ca5f4-163">Relação</span><span class="sxs-lookup"><span data-stu-id="ca5f4-163">Relationship</span></span> | <span data-ttu-id="ca5f4-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca5f4-164">Type</span></span>   |<span data-ttu-id="ca5f4-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca5f4-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca5f4-166">mensagens</span><span class="sxs-lookup"><span data-stu-id="ca5f4-166">messages</span></span>|<span data-ttu-id="ca5f4-167">coleção [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="ca5f4-167">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="ca5f4-168">Uma coleção de todas as mensagens no canal.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-168">A collection of all the messages in the channel.</span></span> <span data-ttu-id="ca5f4-169">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-169">A navigation property.</span></span> <span data-ttu-id="ca5f4-170">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-170">Nullable.</span></span> <span data-ttu-id="ca5f4-171">Atualmente, essa API suporta leitura apenas mas eventualmente dará suporte a mensagens de escrita muito.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-171">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="ca5f4-172">chatThreads</span><span class="sxs-lookup"><span data-stu-id="ca5f4-172">chatThreads</span></span>|<span data-ttu-id="ca5f4-173">coleção [chatThread](chatthread.md)</span><span class="sxs-lookup"><span data-stu-id="ca5f4-173">[chatThread](chatthread.md) collection</span></span>|<span data-ttu-id="ca5f4-174">(Isso é sendo substituídos gradualmente à propriedade mensagens) chatThreads oferece suporte à criação de novas mensagens, mas não a leitura de mensagens.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-174">(This is being phased out in favor of the messages property) chatThreads supports creating new messages but not reading messages.</span></span> <span data-ttu-id="ca5f4-175">ChatThreads é uma propriedade de navegação e é Nullable.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-175">ChatThreads is a navigation property, and is Nullable.</span></span>|
|<span data-ttu-id="ca5f4-176">guias</span><span class="sxs-lookup"><span data-stu-id="ca5f4-176">tabs</span></span>|<span data-ttu-id="ca5f4-177">coleção [teamsTab](../resources/teamstab.md)</span><span class="sxs-lookup"><span data-stu-id="ca5f4-177">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="ca5f4-178">Uma coleção de todas as guias no canal.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-178">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="ca5f4-179">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="ca5f4-179">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ca5f4-180">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ca5f4-180">JSON representation</span></span>

<span data-ttu-id="ca5f4-181">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ca5f4-181">Here is a JSON representation of the resource</span></span>

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
