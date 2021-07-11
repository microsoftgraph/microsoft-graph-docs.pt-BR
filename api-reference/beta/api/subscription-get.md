---
title: Obter assinatura
description: Recupere as propriedades e os relacionamentos da uma assinatura.
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 7a87d2c594756e4ee9b71e112e459a4c02deb793
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366944"
---
# <a name="get-subscription"></a><span data-ttu-id="79514-103">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="79514-103">Get subscription</span></span>

<span data-ttu-id="79514-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79514-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79514-105">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="79514-105">Retrieve the properties and relationships of a subscription.</span></span>

<span data-ttu-id="79514-106">Consulte a tabela na seção [Permissões](#permissions) para obter a lista de recursos que oferecem suporte à inscrição para alterar notificações.</span><span class="sxs-lookup"><span data-stu-id="79514-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="79514-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="79514-107">Permissions</span></span>

<span data-ttu-id="79514-108">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="79514-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="79514-109">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79514-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79514-110">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="79514-110">Supported resource</span></span> | <span data-ttu-id="79514-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79514-111">Delegated (work or school account)</span></span> | <span data-ttu-id="79514-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79514-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79514-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79514-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="79514-114">callRecord</span><span class="sxs-lookup"><span data-stu-id="79514-114">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="79514-115">Incompatível</span><span class="sxs-lookup"><span data-stu-id="79514-115">Not supported</span></span> | <span data-ttu-id="79514-116">Incompatível</span><span class="sxs-lookup"><span data-stu-id="79514-116">Not supported</span></span> | <span data-ttu-id="79514-117">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="79514-117">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="79514-118">[canais](../resources/channel.md) (/teams/getAllChannels – todos os canais em uma organização)</span><span class="sxs-lookup"><span data-stu-id="79514-118">[channels](../resources/channel.md) (/teams/getAllChannels – all channels in an organization)</span></span> | <span data-ttu-id="79514-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-119">Not supported</span></span>  | <span data-ttu-id="79514-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-120">Not supported</span></span> | <span data-ttu-id="79514-121">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="79514-121">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> |
|<span data-ttu-id="79514-122">[canais](../resources/channel.md) (/teams/{id}/channels)</span><span class="sxs-lookup"><span data-stu-id="79514-122">[channels](../resources/channel.md) (/teams/{id}/channels)</span></span> | <span data-ttu-id="79514-123">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="79514-123">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  | <span data-ttu-id="79514-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-124">Not supported</span></span> | <span data-ttu-id="79514-125">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="79514-125">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  |
|<span data-ttu-id="79514-126">[chat](../resources/chat.md) (/chats – todos os chats em uma organização)</span><span class="sxs-lookup"><span data-stu-id="79514-126">[chat](../resources/chat.md) (/chats – all chats in an organization)</span></span> | <span data-ttu-id="79514-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-127">Not supported</span></span> | <span data-ttu-id="79514-128">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-128">Not supported</span></span> | <span data-ttu-id="79514-129">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79514-129">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="79514-130">[chat](../resources/chat.md) (/chats/{id})</span><span class="sxs-lookup"><span data-stu-id="79514-130">[chat](../resources/chat.md) (/chats/{id})</span></span> | <span data-ttu-id="79514-131">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79514-131">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="79514-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-132">Not supported</span></span> | <span data-ttu-id="79514-133">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79514-133">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="79514-134">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="79514-134">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="79514-135">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79514-135">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="79514-136">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-136">Not supported</span></span> | <span data-ttu-id="79514-137">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="79514-137">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="79514-138">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="79514-138">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="79514-139">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-139">Not supported</span></span> | <span data-ttu-id="79514-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-140">Not supported</span></span> | <span data-ttu-id="79514-141">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="79514-141">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="79514-142">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="79514-142">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="79514-143">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79514-143">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="79514-144">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-144">Not supported</span></span> | <span data-ttu-id="79514-145">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="79514-145">Chat.Read.All</span></span>  |
|<span data-ttu-id="79514-146">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="79514-146">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="79514-147">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-147">Not supported</span></span> | <span data-ttu-id="79514-148">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-148">Not supported</span></span> | <span data-ttu-id="79514-149">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="79514-149">Chat.Read.All</span></span>  |
|[<span data-ttu-id="79514-150">contato</span><span class="sxs-lookup"><span data-stu-id="79514-150">contact</span></span>](../resources/contact.md) | <span data-ttu-id="79514-151">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="79514-151">Contacts.Read</span></span> | <span data-ttu-id="79514-152">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="79514-152">Contacts.Read</span></span> | <span data-ttu-id="79514-153">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="79514-153">Contacts.Read</span></span> |
|<span data-ttu-id="79514-154">[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers)</span><span class="sxs-lookup"><span data-stu-id="79514-154">[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers)</span></span> | <span data-ttu-id="79514-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-155">Not supported</span></span> | <span data-ttu-id="79514-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-156">Not supported</span></span> | <span data-ttu-id="79514-157">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79514-157">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="79514-158">[conversationMember](../resources/conversationmember.md) (/chats/{id}/members)</span><span class="sxs-lookup"><span data-stu-id="79514-158">[conversationMember](../resources/conversationmember.md) (/chats/{id}/members)</span></span> | <span data-ttu-id="79514-159">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79514-159">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="79514-160">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-160">Not supported</span></span> | <span data-ttu-id="79514-161">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79514-161">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="79514-162">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span><span class="sxs-lookup"><span data-stu-id="79514-162">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span></span> | <span data-ttu-id="79514-163">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="79514-163">TeamMember.Read.All</span></span> | <span data-ttu-id="79514-164">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-164">Not supported</span></span> | <span data-ttu-id="79514-165">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="79514-165">TeamMember.Read.All</span></span> |
|<span data-ttu-id="79514-166">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="79514-166">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="79514-167">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-167">Not supported</span></span> | <span data-ttu-id="79514-168">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79514-168">Files.ReadWrite</span></span> | <span data-ttu-id="79514-169">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-169">Not supported</span></span> |
|<span data-ttu-id="79514-170">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="79514-170">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="79514-171">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79514-171">Files.ReadWrite.All</span></span> | <span data-ttu-id="79514-172">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-172">Not supported</span></span> | <span data-ttu-id="79514-173">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79514-173">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="79514-174">evento</span><span class="sxs-lookup"><span data-stu-id="79514-174">event</span></span>](../resources/event.md) | <span data-ttu-id="79514-175">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="79514-175">Calendars.Read</span></span> | <span data-ttu-id="79514-176">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="79514-176">Calendars.Read</span></span> | <span data-ttu-id="79514-177">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="79514-177">Calendars.Read</span></span> |
|[<span data-ttu-id="79514-178">grupo</span><span class="sxs-lookup"><span data-stu-id="79514-178">group</span></span>](../resources/group.md) | <span data-ttu-id="79514-179">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="79514-179">Group.Read.All</span></span> | <span data-ttu-id="79514-180">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-180">Not supported</span></span> | <span data-ttu-id="79514-181">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="79514-181">Group.Read.All</span></span> |
|[<span data-ttu-id="79514-182">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="79514-182">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="79514-183">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="79514-183">Group.Read.All</span></span> | <span data-ttu-id="79514-184">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-184">Not supported</span></span> | <span data-ttu-id="79514-185">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-185">Not supported</span></span> |
|[<span data-ttu-id="79514-186">list</span><span class="sxs-lookup"><span data-stu-id="79514-186">list</span></span>](../resources/list.md) | <span data-ttu-id="79514-187">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79514-187">Sites.ReadWrite.All</span></span> | <span data-ttu-id="79514-188">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-188">Not supported</span></span> | <span data-ttu-id="79514-189">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79514-189">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="79514-190">message</span><span class="sxs-lookup"><span data-stu-id="79514-190">message</span></span>](../resources/message.md) | <span data-ttu-id="79514-191">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="79514-191">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="79514-192">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="79514-192">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="79514-193">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="79514-193">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="79514-194">presence</span><span class="sxs-lookup"><span data-stu-id="79514-194">presence</span></span>](../resources/presence.md) | <span data-ttu-id="79514-195">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="79514-195">Presence.Read.All</span></span> | <span data-ttu-id="79514-196">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-196">Not supported</span></span> | <span data-ttu-id="79514-197">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-197">Not supported</span></span> |
|[<span data-ttu-id="79514-198">printer</span><span class="sxs-lookup"><span data-stu-id="79514-198">printer</span></span>](../resources/printer.md) | <span data-ttu-id="79514-199">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-199">Not supported</span></span> | <span data-ttu-id="79514-200">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-200">Not supported</span></span> | <span data-ttu-id="79514-201">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79514-201">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="79514-202">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="79514-202">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="79514-203">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-203">Not supported</span></span> | <span data-ttu-id="79514-204">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-204">Not supported</span></span> | <span data-ttu-id="79514-205">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79514-205">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="79514-206">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="79514-206">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="79514-207">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79514-207">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="79514-208">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-208">Not supported</span></span> | <span data-ttu-id="79514-209">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79514-209">SecurityEvents.ReadWrite.All</span></span> |
|<span data-ttu-id="79514-210">[teams](../resources/team.md) (/teams – todas as equipes em uma organização)</span><span class="sxs-lookup"><span data-stu-id="79514-210">[teams](../resources/team.md) (/teams – all teams in an organization)</span></span> | <span data-ttu-id="79514-211">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-211">Not supported</span></span> | <span data-ttu-id="79514-212">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-212">Not supported</span></span> | <span data-ttu-id="79514-213">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="79514-213">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|<span data-ttu-id="79514-214">[teams](../resources/team.md) (/teams/{id})</span><span class="sxs-lookup"><span data-stu-id="79514-214">[teams](../resources/team.md) (/teams/{id})</span></span> | <span data-ttu-id="79514-215">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="79514-215">Team.ReadBasic.All, TeamSettings.Read.All</span></span> | <span data-ttu-id="79514-216">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-216">Not supported</span></span> | <span data-ttu-id="79514-217">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="79514-217">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|[<span data-ttu-id="79514-218">todoTask</span><span class="sxs-lookup"><span data-stu-id="79514-218">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="79514-219">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79514-219">Tasks.ReadWrite</span></span> | <span data-ttu-id="79514-220">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79514-220">Tasks.ReadWrite</span></span> | <span data-ttu-id="79514-221">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79514-221">Not supported</span></span> |
|[<span data-ttu-id="79514-222">Usuário</span><span class="sxs-lookup"><span data-stu-id="79514-222">user</span></span>](../resources/user.md) | <span data-ttu-id="79514-223">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="79514-223">User.Read.All</span></span> | <span data-ttu-id="79514-224">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="79514-224">User.Read.All</span></span> | <span data-ttu-id="79514-225">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="79514-225">User.Read.All</span></span> |

> <span data-ttu-id="79514-226">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="79514-226">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="79514-227">driveItem</span><span class="sxs-lookup"><span data-stu-id="79514-227">driveItem</span></span>

<span data-ttu-id="79514-228">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="79514-228">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="79514-229">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="79514-229">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="79514-230">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="79514-230">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="79514-231">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="79514-231">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="79514-232">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="79514-232">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="79514-233">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="79514-233">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="79514-234">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="79514-234">contact, event, and message</span></span>

<span data-ttu-id="79514-235">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="79514-235">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="79514-236">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="79514-236">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="79514-237">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="79514-237">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="79514-238">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="79514-238">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="79514-239">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="79514-239">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="79514-240">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="79514-240">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="79514-241">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="79514-241">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="79514-242">presença</span><span class="sxs-lookup"><span data-stu-id="79514-242">presence</span></span>

<span data-ttu-id="79514-243">**assinaturas** de presença exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="79514-243">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="79514-244">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="79514-244">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="79514-245">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79514-245">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79514-246">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="79514-246">Optional query parameters</span></span>

<span data-ttu-id="79514-247">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="79514-247">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79514-248">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79514-248">Request headers</span></span>

| <span data-ttu-id="79514-249">Nome</span><span class="sxs-lookup"><span data-stu-id="79514-249">Name</span></span>       | <span data-ttu-id="79514-250">Tipo</span><span class="sxs-lookup"><span data-stu-id="79514-250">Type</span></span> | <span data-ttu-id="79514-251">Descrição</span><span class="sxs-lookup"><span data-stu-id="79514-251">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="79514-252">Autorização</span><span class="sxs-lookup"><span data-stu-id="79514-252">Authorization</span></span>  | <span data-ttu-id="79514-253">string</span><span class="sxs-lookup"><span data-stu-id="79514-253">string</span></span>  | <span data-ttu-id="79514-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79514-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79514-256">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79514-256">Request body</span></span>

<span data-ttu-id="79514-257">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="79514-257">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79514-258">Resposta</span><span class="sxs-lookup"><span data-stu-id="79514-258">Response</span></span>

<span data-ttu-id="79514-259">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79514-259">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79514-260">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79514-260">Example</span></span>

##### <a name="request"></a><span data-ttu-id="79514-261">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79514-261">Request</span></span>

<span data-ttu-id="79514-262">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79514-262">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="79514-263">HTTP</span><span class="sxs-lookup"><span data-stu-id="79514-263">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="79514-264">C#</span><span class="sxs-lookup"><span data-stu-id="79514-264">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79514-265">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79514-265">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79514-266">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79514-266">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79514-267">Java</span><span class="sxs-lookup"><span data-stu-id="79514-267">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="79514-268">Resposta</span><span class="sxs-lookup"><span data-stu-id="79514-268">Response</span></span>

<span data-ttu-id="79514-269">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79514-269">Here is an example of the response.</span></span>
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
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string",
  "latestSupportedTlsVersion": "v1_2",
  "encryptionCertificate": "",
  "encryptionCertificateId": "",
  "includeResourceData": false,
  "notificationContentType": "application/json"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


