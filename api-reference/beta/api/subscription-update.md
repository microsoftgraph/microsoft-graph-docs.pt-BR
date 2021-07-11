---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 96680ebb1cedf85f7272bc09b8ab1c55a04c7591
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366917"
---
# <a name="update-subscription"></a><span data-ttu-id="b35eb-103">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="b35eb-103">Update subscription</span></span>

<span data-ttu-id="b35eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b35eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b35eb-105">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="b35eb-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="b35eb-106">A tabela na seção [Permissões](#permissions) lista os recursos que suportam a assinatura para alterar notificações.</span><span class="sxs-lookup"><span data-stu-id="b35eb-106">The table in the [Permissions](#permissions) section lists the resources that support subscribing to change notifications.</span></span>

<span data-ttu-id="b35eb-107">As assinaturas expiram após um período de tempo que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="b35eb-107">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="b35eb-108">Para evitar notificações de alteração ausentes, um aplicativo deve renovar suas assinaturas bem antes da data de expiração.</span><span class="sxs-lookup"><span data-stu-id="b35eb-108">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="b35eb-109">Consulte [assinatura](../resources/subscription.md) para o tamanho máximo de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="b35eb-109">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="b35eb-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="b35eb-110">Permissions</span></span>

<span data-ttu-id="b35eb-111">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="b35eb-111">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="b35eb-112">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b35eb-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b35eb-113">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-113">Supported resource</span></span> | <span data-ttu-id="b35eb-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b35eb-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b35eb-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b35eb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b35eb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b35eb-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="b35eb-117">callRecord</span><span class="sxs-lookup"><span data-stu-id="b35eb-117">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="b35eb-118">Incompatível</span><span class="sxs-lookup"><span data-stu-id="b35eb-118">Not supported</span></span> | <span data-ttu-id="b35eb-119">Incompatível</span><span class="sxs-lookup"><span data-stu-id="b35eb-119">Not supported</span></span> | <span data-ttu-id="b35eb-120">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-120">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="b35eb-121">[canais](../resources/channel.md) (/teams/getAllChannels – todos os canais em uma organização)</span><span class="sxs-lookup"><span data-stu-id="b35eb-121">[channels](../resources/channel.md) (/teams/getAllChannels – all channels in an organization)</span></span> | <span data-ttu-id="b35eb-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-122">Not supported</span></span>  | <span data-ttu-id="b35eb-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-123">Not supported</span></span> | <span data-ttu-id="b35eb-124">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-124">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> |
|<span data-ttu-id="b35eb-125">[canais](../resources/channel.md) (/teams/{id}/channels)</span><span class="sxs-lookup"><span data-stu-id="b35eb-125">[channels](../resources/channel.md) (/teams/{id}/channels)</span></span> | <span data-ttu-id="b35eb-126">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-126">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  | <span data-ttu-id="b35eb-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-127">Not supported</span></span> | <span data-ttu-id="b35eb-128">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-128">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  |
|<span data-ttu-id="b35eb-129">[chat](../resources/chat.md) (/chats – todos os chats em uma organização)</span><span class="sxs-lookup"><span data-stu-id="b35eb-129">[chat](../resources/chat.md) (/chats – all chats in an organization)</span></span> | <span data-ttu-id="b35eb-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-130">Not supported</span></span> | <span data-ttu-id="b35eb-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-131">Not supported</span></span> | <span data-ttu-id="b35eb-132">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-132">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="b35eb-133">[chat](../resources/chat.md) (/chats/{id})</span><span class="sxs-lookup"><span data-stu-id="b35eb-133">[chat](../resources/chat.md) (/chats/{id})</span></span> | <span data-ttu-id="b35eb-134">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b35eb-134">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="b35eb-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-135">Not supported</span></span> | <span data-ttu-id="b35eb-136">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-136">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="b35eb-137">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="b35eb-137">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="b35eb-138">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-138">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="b35eb-139">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-139">Not supported</span></span> | <span data-ttu-id="b35eb-140">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-140">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="b35eb-141">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="b35eb-141">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="b35eb-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-142">Not supported</span></span> | <span data-ttu-id="b35eb-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-143">Not supported</span></span> | <span data-ttu-id="b35eb-144">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-144">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="b35eb-145">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="b35eb-145">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="b35eb-146">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b35eb-146">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="b35eb-147">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-147">Not supported</span></span> | <span data-ttu-id="b35eb-148">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-148">Chat.Read.All</span></span>  |
|<span data-ttu-id="b35eb-149">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="b35eb-149">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="b35eb-150">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-150">Not supported</span></span> | <span data-ttu-id="b35eb-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-151">Not supported</span></span> | <span data-ttu-id="b35eb-152">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-152">Chat.Read.All</span></span>  |
|[<span data-ttu-id="b35eb-153">contato</span><span class="sxs-lookup"><span data-stu-id="b35eb-153">contact</span></span>](../resources/contact.md) | <span data-ttu-id="b35eb-154">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b35eb-154">Contacts.Read</span></span> | <span data-ttu-id="b35eb-155">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b35eb-155">Contacts.Read</span></span> | <span data-ttu-id="b35eb-156">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b35eb-156">Contacts.Read</span></span> |
|<span data-ttu-id="b35eb-157">[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers)</span><span class="sxs-lookup"><span data-stu-id="b35eb-157">[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers)</span></span> | <span data-ttu-id="b35eb-158">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-158">Not supported</span></span> | <span data-ttu-id="b35eb-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-159">Not supported</span></span> | <span data-ttu-id="b35eb-160">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-160">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="b35eb-161">[conversationMember](../resources/conversationmember.md) (/chats/{id}/members)</span><span class="sxs-lookup"><span data-stu-id="b35eb-161">[conversationMember](../resources/conversationmember.md) (/chats/{id}/members)</span></span> | <span data-ttu-id="b35eb-162">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b35eb-162">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="b35eb-163">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-163">Not supported</span></span> | <span data-ttu-id="b35eb-164">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-164">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="b35eb-165">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span><span class="sxs-lookup"><span data-stu-id="b35eb-165">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span></span> | <span data-ttu-id="b35eb-166">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-166">TeamMember.Read.All</span></span> | <span data-ttu-id="b35eb-167">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-167">Not supported</span></span> | <span data-ttu-id="b35eb-168">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-168">TeamMember.Read.All</span></span> |
|<span data-ttu-id="b35eb-169">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="b35eb-169">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="b35eb-170">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-170">Not supported</span></span> | <span data-ttu-id="b35eb-171">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b35eb-171">Files.ReadWrite</span></span> | <span data-ttu-id="b35eb-172">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-172">Not supported</span></span> |
|<span data-ttu-id="b35eb-173">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="b35eb-173">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="b35eb-174">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-174">Files.ReadWrite.All</span></span> | <span data-ttu-id="b35eb-175">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-175">Not supported</span></span> | <span data-ttu-id="b35eb-176">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-176">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="b35eb-177">evento</span><span class="sxs-lookup"><span data-stu-id="b35eb-177">event</span></span>](../resources/event.md) | <span data-ttu-id="b35eb-178">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b35eb-178">Calendars.Read</span></span> | <span data-ttu-id="b35eb-179">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b35eb-179">Calendars.Read</span></span> | <span data-ttu-id="b35eb-180">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b35eb-180">Calendars.Read</span></span> |
|[<span data-ttu-id="b35eb-181">grupo</span><span class="sxs-lookup"><span data-stu-id="b35eb-181">group</span></span>](../resources/group.md) | <span data-ttu-id="b35eb-182">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-182">Group.Read.All</span></span> | <span data-ttu-id="b35eb-183">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-183">Not supported</span></span> | <span data-ttu-id="b35eb-184">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-184">Group.Read.All</span></span> |
|[<span data-ttu-id="b35eb-185">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="b35eb-185">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="b35eb-186">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-186">Group.Read.All</span></span> | <span data-ttu-id="b35eb-187">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-187">Not supported</span></span> | <span data-ttu-id="b35eb-188">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-188">Not supported</span></span> |
|[<span data-ttu-id="b35eb-189">list</span><span class="sxs-lookup"><span data-stu-id="b35eb-189">list</span></span>](../resources/list.md) | <span data-ttu-id="b35eb-190">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-190">Sites.ReadWrite.All</span></span> | <span data-ttu-id="b35eb-191">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-191">Not supported</span></span> | <span data-ttu-id="b35eb-192">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-192">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="b35eb-193">message</span><span class="sxs-lookup"><span data-stu-id="b35eb-193">message</span></span>](../resources/message.md) | <span data-ttu-id="b35eb-194">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b35eb-194">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="b35eb-195">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b35eb-195">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="b35eb-196">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b35eb-196">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="b35eb-197">presence</span><span class="sxs-lookup"><span data-stu-id="b35eb-197">presence</span></span>](../resources/presence.md) | <span data-ttu-id="b35eb-198">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-198">Presence.Read.All</span></span> | <span data-ttu-id="b35eb-199">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-199">Not supported</span></span> | <span data-ttu-id="b35eb-200">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-200">Not supported</span></span> |
|[<span data-ttu-id="b35eb-201">printer</span><span class="sxs-lookup"><span data-stu-id="b35eb-201">printer</span></span>](../resources/printer.md) | <span data-ttu-id="b35eb-202">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-202">Not supported</span></span> | <span data-ttu-id="b35eb-203">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-203">Not supported</span></span> | <span data-ttu-id="b35eb-204">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-204">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="b35eb-205">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="b35eb-205">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="b35eb-206">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-206">Not supported</span></span> | <span data-ttu-id="b35eb-207">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-207">Not supported</span></span> | <span data-ttu-id="b35eb-208">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-208">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="b35eb-209">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="b35eb-209">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="b35eb-210">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-210">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="b35eb-211">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-211">Not supported</span></span> | <span data-ttu-id="b35eb-212">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-212">SecurityEvents.ReadWrite.All</span></span> |
|<span data-ttu-id="b35eb-213">[teams](../resources/team.md) (/teams – todas as equipes em uma organização)</span><span class="sxs-lookup"><span data-stu-id="b35eb-213">[teams](../resources/team.md) (/teams – all teams in an organization)</span></span> | <span data-ttu-id="b35eb-214">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-214">Not supported</span></span> | <span data-ttu-id="b35eb-215">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-215">Not supported</span></span> | <span data-ttu-id="b35eb-216">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-216">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|<span data-ttu-id="b35eb-217">[teams](../resources/team.md) (/teams/{id})</span><span class="sxs-lookup"><span data-stu-id="b35eb-217">[teams](../resources/team.md) (/teams/{id})</span></span> | <span data-ttu-id="b35eb-218">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-218">Team.ReadBasic.All, TeamSettings.Read.All</span></span> | <span data-ttu-id="b35eb-219">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-219">Not supported</span></span> | <span data-ttu-id="b35eb-220">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-220">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|[<span data-ttu-id="b35eb-221">todoTask</span><span class="sxs-lookup"><span data-stu-id="b35eb-221">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="b35eb-222">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b35eb-222">Tasks.ReadWrite</span></span> | <span data-ttu-id="b35eb-223">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b35eb-223">Tasks.ReadWrite</span></span> | <span data-ttu-id="b35eb-224">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b35eb-224">Not supported</span></span> |
|[<span data-ttu-id="b35eb-225">Usuário</span><span class="sxs-lookup"><span data-stu-id="b35eb-225">user</span></span>](../resources/user.md) | <span data-ttu-id="b35eb-226">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-226">User.Read.All</span></span> | <span data-ttu-id="b35eb-227">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-227">User.Read.All</span></span> | <span data-ttu-id="b35eb-228">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b35eb-228">User.Read.All</span></span> |

> <span data-ttu-id="b35eb-229">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="b35eb-229">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="b35eb-230">driveItem</span><span class="sxs-lookup"><span data-stu-id="b35eb-230">driveItem</span></span>

<span data-ttu-id="b35eb-231">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b35eb-231">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="b35eb-232">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="b35eb-232">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="b35eb-233">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="b35eb-233">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="b35eb-234">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="b35eb-234">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="b35eb-235">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="b35eb-235">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="b35eb-236">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="b35eb-236">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="b35eb-237">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="b35eb-237">contact, event, and message</span></span>

<span data-ttu-id="b35eb-238">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="b35eb-238">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="b35eb-239">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="b35eb-239">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="b35eb-240">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="b35eb-240">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="b35eb-241">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="b35eb-241">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="b35eb-242">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="b35eb-242">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="b35eb-243">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="b35eb-243">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="b35eb-244">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="b35eb-244">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="b35eb-245">presença</span><span class="sxs-lookup"><span data-stu-id="b35eb-245">presence</span></span>

<span data-ttu-id="b35eb-246">**assinaturas** de presença exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="b35eb-246">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="b35eb-247">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="b35eb-247">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="b35eb-248">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b35eb-248">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b35eb-249">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b35eb-249">Request headers</span></span>

| <span data-ttu-id="b35eb-250">Nome</span><span class="sxs-lookup"><span data-stu-id="b35eb-250">Name</span></span>       | <span data-ttu-id="b35eb-251">Tipo</span><span class="sxs-lookup"><span data-stu-id="b35eb-251">Type</span></span> | <span data-ttu-id="b35eb-252">Descrição</span><span class="sxs-lookup"><span data-stu-id="b35eb-252">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b35eb-253">Autorização</span><span class="sxs-lookup"><span data-stu-id="b35eb-253">Authorization</span></span>  | <span data-ttu-id="b35eb-254">string</span><span class="sxs-lookup"><span data-stu-id="b35eb-254">string</span></span>  | <span data-ttu-id="b35eb-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b35eb-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b35eb-257">Resposta</span><span class="sxs-lookup"><span data-stu-id="b35eb-257">Response</span></span>

<span data-ttu-id="b35eb-258">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b35eb-258">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="b35eb-259">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="b35eb-259">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="b35eb-260">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b35eb-260">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b35eb-261">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b35eb-261">Request</span></span>

<span data-ttu-id="b35eb-262">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b35eb-262">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b35eb-263">HTTP</span><span class="sxs-lookup"><span data-stu-id="b35eb-263">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/beta/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```
# <a name="c"></a>[<span data-ttu-id="b35eb-264">C#</span><span class="sxs-lookup"><span data-stu-id="b35eb-264">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b35eb-265">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b35eb-265">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b35eb-266">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b35eb-266">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b35eb-267">Java</span><span class="sxs-lookup"><span data-stu-id="b35eb-267">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b35eb-268">Resposta</span><span class="sxs-lookup"><span data-stu-id="b35eb-268">Response</span></span>

<span data-ttu-id="b35eb-269">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b35eb-269">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2",
  "encryptionCertificate": "",
  "encryptionCertificateId": "",
  "includeResourceData": false,
  "notificationContentType": "application/json"
}
```

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


