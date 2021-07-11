---
title: Criar assinatura
description: Inscreve um aplicativo ouvinte para receber notificações de alteração quando os dados em um recurso microsoft Graph alterações.
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 8f2e1524c63ceb77b092f0699f7bf1002a8420b0
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366916"
---
# <a name="create-subscription"></a><span data-ttu-id="d4a71-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="d4a71-103">Create subscription</span></span>

<span data-ttu-id="d4a71-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4a71-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4a71-105">Inscreve um aplicativo de ouvinte para receber notificações de alterações quando o tipo de alteração solicitado ocorrer no recurso especificado no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d4a71-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

<span data-ttu-id="d4a71-106">Consulte a tabela na seção [Permissões](#permissions) para obter a lista de recursos que oferecem suporte à inscrição para alterar notificações.</span><span class="sxs-lookup"><span data-stu-id="d4a71-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4a71-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4a71-107">Permissions</span></span>

<span data-ttu-id="d4a71-108">A criação de uma assinatura requer permissão de leitura para o recurso.</span><span class="sxs-lookup"><span data-stu-id="d4a71-108">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="d4a71-109">Por exemplo, para receber notificações de alteração em mensagens, seu aplicativo precisa da permissão Mail.Read.</span><span class="sxs-lookup"><span data-stu-id="d4a71-109">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 

<span data-ttu-id="d4a71-110">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="d4a71-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="d4a71-111">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4a71-111">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4a71-112">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-112">Supported resource</span></span> | <span data-ttu-id="d4a71-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4a71-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d4a71-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4a71-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4a71-115">Application</span><span class="sxs-lookup"><span data-stu-id="d4a71-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="d4a71-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="d4a71-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="d4a71-117">Incompatível</span><span class="sxs-lookup"><span data-stu-id="d4a71-117">Not supported</span></span> | <span data-ttu-id="d4a71-118">Incompatível</span><span class="sxs-lookup"><span data-stu-id="d4a71-118">Not supported</span></span> | <span data-ttu-id="d4a71-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="d4a71-120">[canais](../resources/channel.md) (/teams/getAllChannels – todos os canais em uma organização)</span><span class="sxs-lookup"><span data-stu-id="d4a71-120">[channels](../resources/channel.md) (/teams/getAllChannels – all channels in an organization)</span></span> | <span data-ttu-id="d4a71-121">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-121">Not supported</span></span>  | <span data-ttu-id="d4a71-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-122">Not supported</span></span> | <span data-ttu-id="d4a71-123">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-123">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> |
|<span data-ttu-id="d4a71-124">[canais](../resources/channel.md) (/teams/{id}/channels)</span><span class="sxs-lookup"><span data-stu-id="d4a71-124">[channels](../resources/channel.md) (/teams/{id}/channels)</span></span> | <span data-ttu-id="d4a71-125">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-125">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  | <span data-ttu-id="d4a71-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-126">Not supported</span></span> | <span data-ttu-id="d4a71-127">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-127">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  |
|<span data-ttu-id="d4a71-128">[chat](../resources/chat.md) (/chats – todos os chats em uma organização)</span><span class="sxs-lookup"><span data-stu-id="d4a71-128">[chat](../resources/chat.md) (/chats – all chats in an organization)</span></span> | <span data-ttu-id="d4a71-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-129">Not supported</span></span> | <span data-ttu-id="d4a71-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-130">Not supported</span></span> | <span data-ttu-id="d4a71-131">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-131">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="d4a71-132">[chat](../resources/chat.md) (/chats/{id})</span><span class="sxs-lookup"><span data-stu-id="d4a71-132">[chat](../resources/chat.md) (/chats/{id})</span></span> | <span data-ttu-id="d4a71-133">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4a71-133">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="d4a71-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-134">Not supported</span></span> | <span data-ttu-id="d4a71-135">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-135">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="d4a71-136">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="d4a71-136">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="d4a71-137">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-137">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="d4a71-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-138">Not supported</span></span> | <span data-ttu-id="d4a71-139">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-139">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="d4a71-140">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="d4a71-140">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="d4a71-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-141">Not supported</span></span> | <span data-ttu-id="d4a71-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-142">Not supported</span></span> | <span data-ttu-id="d4a71-143">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-143">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="d4a71-144">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="d4a71-144">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="d4a71-145">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4a71-145">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="d4a71-146">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-146">Not supported</span></span> | <span data-ttu-id="d4a71-147">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-147">Chat.Read.All</span></span>  |
|<span data-ttu-id="d4a71-148">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="d4a71-148">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="d4a71-149">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-149">Not supported</span></span> | <span data-ttu-id="d4a71-150">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-150">Not supported</span></span> | <span data-ttu-id="d4a71-151">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-151">Chat.Read.All</span></span>  |
|[<span data-ttu-id="d4a71-152">contato</span><span class="sxs-lookup"><span data-stu-id="d4a71-152">contact</span></span>](../resources/contact.md) | <span data-ttu-id="d4a71-153">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d4a71-153">Contacts.Read</span></span> | <span data-ttu-id="d4a71-154">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d4a71-154">Contacts.Read</span></span> | <span data-ttu-id="d4a71-155">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d4a71-155">Contacts.Read</span></span> |
|<span data-ttu-id="d4a71-156">[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers)</span><span class="sxs-lookup"><span data-stu-id="d4a71-156">[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers)</span></span> | <span data-ttu-id="d4a71-157">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-157">Not supported</span></span> | <span data-ttu-id="d4a71-158">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-158">Not supported</span></span> | <span data-ttu-id="d4a71-159">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-159">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="d4a71-160">[conversationMember](../resources/conversationmember.md) (/chats/{id}/members)</span><span class="sxs-lookup"><span data-stu-id="d4a71-160">[conversationMember](../resources/conversationmember.md) (/chats/{id}/members)</span></span> | <span data-ttu-id="d4a71-161">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4a71-161">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="d4a71-162">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-162">Not supported</span></span> | <span data-ttu-id="d4a71-163">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-163">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="d4a71-164">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span><span class="sxs-lookup"><span data-stu-id="d4a71-164">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span></span> | <span data-ttu-id="d4a71-165">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-165">TeamMember.Read.All</span></span> | <span data-ttu-id="d4a71-166">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-166">Not supported</span></span> | <span data-ttu-id="d4a71-167">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-167">TeamMember.Read.All</span></span> |
|<span data-ttu-id="d4a71-168">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="d4a71-168">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="d4a71-169">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-169">Not supported</span></span> | <span data-ttu-id="d4a71-170">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4a71-170">Files.ReadWrite</span></span> | <span data-ttu-id="d4a71-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-171">Not supported</span></span> |
|<span data-ttu-id="d4a71-172">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="d4a71-172">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="d4a71-173">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-173">Files.ReadWrite.All</span></span> | <span data-ttu-id="d4a71-174">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-174">Not supported</span></span> | <span data-ttu-id="d4a71-175">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-175">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="d4a71-176">evento</span><span class="sxs-lookup"><span data-stu-id="d4a71-176">event</span></span>](../resources/event.md) | <span data-ttu-id="d4a71-177">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d4a71-177">Calendars.Read</span></span> | <span data-ttu-id="d4a71-178">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d4a71-178">Calendars.Read</span></span> | <span data-ttu-id="d4a71-179">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d4a71-179">Calendars.Read</span></span> |
|[<span data-ttu-id="d4a71-180">grupo</span><span class="sxs-lookup"><span data-stu-id="d4a71-180">group</span></span>](../resources/group.md) | <span data-ttu-id="d4a71-181">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-181">Group.Read.All</span></span> | <span data-ttu-id="d4a71-182">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-182">Not supported</span></span> | <span data-ttu-id="d4a71-183">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-183">Group.Read.All</span></span> |
|[<span data-ttu-id="d4a71-184">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="d4a71-184">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="d4a71-185">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-185">Group.Read.All</span></span> | <span data-ttu-id="d4a71-186">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-186">Not supported</span></span> | <span data-ttu-id="d4a71-187">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-187">Not supported</span></span> |
|[<span data-ttu-id="d4a71-188">list</span><span class="sxs-lookup"><span data-stu-id="d4a71-188">list</span></span>](../resources/list.md) | <span data-ttu-id="d4a71-189">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-189">Sites.ReadWrite.All</span></span> | <span data-ttu-id="d4a71-190">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-190">Not supported</span></span> | <span data-ttu-id="d4a71-191">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-191">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="d4a71-192">message</span><span class="sxs-lookup"><span data-stu-id="d4a71-192">message</span></span>](../resources/message.md) | <span data-ttu-id="d4a71-193">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d4a71-193">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="d4a71-194">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d4a71-194">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="d4a71-195">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d4a71-195">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="d4a71-196">presence</span><span class="sxs-lookup"><span data-stu-id="d4a71-196">presence</span></span>](../resources/presence.md) | <span data-ttu-id="d4a71-197">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-197">Presence.Read.All</span></span> | <span data-ttu-id="d4a71-198">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-198">Not supported</span></span> | <span data-ttu-id="d4a71-199">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-199">Not supported</span></span> |
|[<span data-ttu-id="d4a71-200">printer</span><span class="sxs-lookup"><span data-stu-id="d4a71-200">printer</span></span>](../resources/printer.md) | <span data-ttu-id="d4a71-201">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-201">Not supported</span></span> | <span data-ttu-id="d4a71-202">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-202">Not supported</span></span> | <span data-ttu-id="d4a71-203">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-203">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="d4a71-204">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="d4a71-204">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="d4a71-205">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-205">Not supported</span></span> | <span data-ttu-id="d4a71-206">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-206">Not supported</span></span> | <span data-ttu-id="d4a71-207">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-207">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="d4a71-208">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="d4a71-208">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="d4a71-209">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-209">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="d4a71-210">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-210">Not supported</span></span> | <span data-ttu-id="d4a71-211">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-211">SecurityEvents.ReadWrite.All</span></span> |
|<span data-ttu-id="d4a71-212">[teams](../resources/team.md) (/teams – todas as equipes em uma organização)</span><span class="sxs-lookup"><span data-stu-id="d4a71-212">[teams](../resources/team.md) (/teams – all teams in an organization)</span></span> | <span data-ttu-id="d4a71-213">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-213">Not supported</span></span> | <span data-ttu-id="d4a71-214">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-214">Not supported</span></span> | <span data-ttu-id="d4a71-215">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-215">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|<span data-ttu-id="d4a71-216">[teams](../resources/team.md) (/teams/{id})</span><span class="sxs-lookup"><span data-stu-id="d4a71-216">[teams](../resources/team.md) (/teams/{id})</span></span> | <span data-ttu-id="d4a71-217">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-217">Team.ReadBasic.All, TeamSettings.Read.All</span></span> | <span data-ttu-id="d4a71-218">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-218">Not supported</span></span> | <span data-ttu-id="d4a71-219">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-219">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|[<span data-ttu-id="d4a71-220">todoTask</span><span class="sxs-lookup"><span data-stu-id="d4a71-220">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="d4a71-221">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4a71-221">Tasks.ReadWrite</span></span> | <span data-ttu-id="d4a71-222">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4a71-222">Tasks.ReadWrite</span></span> | <span data-ttu-id="d4a71-223">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4a71-223">Not supported</span></span> |
|[<span data-ttu-id="d4a71-224">Usuário</span><span class="sxs-lookup"><span data-stu-id="d4a71-224">user</span></span>](../resources/user.md) | <span data-ttu-id="d4a71-225">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-225">User.Read.All</span></span> | <span data-ttu-id="d4a71-226">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-226">User.Read.All</span></span> | <span data-ttu-id="d4a71-227">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a71-227">User.Read.All</span></span> |

> <span data-ttu-id="d4a71-228">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="d4a71-228">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="d4a71-229">driveItem</span><span class="sxs-lookup"><span data-stu-id="d4a71-229">driveItem</span></span>

<span data-ttu-id="d4a71-230">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d4a71-230">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="d4a71-231">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="d4a71-231">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="d4a71-232">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="d4a71-232">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="d4a71-233">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="d4a71-233">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="d4a71-234">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="d4a71-234">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="d4a71-235">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="d4a71-235">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

<span data-ttu-id="d4a71-236">OneDrive for Business e Microsoft Office SharePoint Online suportam o envio de notificações de aplicações de eventos de segurança que ocorrem em um **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="d4a71-236">OneDrive for Business and SharePoint support sending your application notifications of security events that occur on a **driveItem**.</span></span> <span data-ttu-id="d4a71-237">Para se inscrever nestes eventos, adicionar o cabeçalho `prefer:includesecuritywebhooks` a sua solicitação para criar uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="d4a71-237">To subscribe to these events, add the `prefer:includesecuritywebhooks` header to your request to create a subscription.</span></span> <span data-ttu-id="d4a71-238">Após a criação da assinatura, você receberá notificações quando as permissões sobre uma mudança de item forem alteradas.</span><span class="sxs-lookup"><span data-stu-id="d4a71-238">After the subscription is created, you will receive notifications when the permissions on an item change.</span></span> <span data-ttu-id="d4a71-239">Este cabeçalho é aplicável às contas Microsoft Office SharePoint Online e OneDrive for Business, mas não às contas OneDrive de consumo.</span><span class="sxs-lookup"><span data-stu-id="d4a71-239">This header is applicable to SharePoint and OneDrive for Business but not consumer OneDrive accounts.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="d4a71-240">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="d4a71-240">contact, event, and message</span></span>

<span data-ttu-id="d4a71-241">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="d4a71-241">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="d4a71-242">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="d4a71-242">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="d4a71-243">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="d4a71-243">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="d4a71-244">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="d4a71-244">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="d4a71-245">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="d4a71-245">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="d4a71-246">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="d4a71-246">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="d4a71-247">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="d4a71-247">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="d4a71-248">presença</span><span class="sxs-lookup"><span data-stu-id="d4a71-248">presence</span></span>

<span data-ttu-id="d4a71-249">**assinaturas** de presença exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="d4a71-249">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="d4a71-250">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="d4a71-250">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="d4a71-251">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4a71-251">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="d4a71-252">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4a71-252">Request headers</span></span>

| <span data-ttu-id="d4a71-253">Nome</span><span class="sxs-lookup"><span data-stu-id="d4a71-253">Name</span></span>       | <span data-ttu-id="d4a71-254">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4a71-254">Type</span></span> | <span data-ttu-id="d4a71-255">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4a71-255">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d4a71-256">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4a71-256">Authorization</span></span>  | <span data-ttu-id="d4a71-257">string</span><span class="sxs-lookup"><span data-stu-id="d4a71-257">string</span></span>  | <span data-ttu-id="d4a71-p109">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4a71-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d4a71-260">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4a71-260">Response</span></span>

<span data-ttu-id="d4a71-261">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4a71-261">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="d4a71-262">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="d4a71-262">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="d4a71-263">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4a71-263">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4a71-264">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4a71-264">Request</span></span>

<span data-ttu-id="d4a71-265">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="d4a71-265">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="d4a71-266">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="d4a71-266">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="d4a71-267">Essa solicitação cria uma assinatura para notificações de alteração sobre novos emails recebidos pelo usuário atualmente inscrito.</span><span class="sxs-lookup"><span data-stu-id="d4a71-267">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="d4a71-268">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4a71-268">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue",
   "latestSupportedTlsVersion": "v1_2"
}
```
# <a name="c"></a>[<span data-ttu-id="d4a71-269">C#</span><span class="sxs-lookup"><span data-stu-id="d4a71-269">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4a71-270">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4a71-270">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4a71-271">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4a71-271">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d4a71-272">Java</span><span class="sxs-lookup"><span data-stu-id="d4a71-272">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="d4a71-273">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="d4a71-273">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="d4a71-274">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="d4a71-274">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

#### <a name="resources-examples"></a><span data-ttu-id="d4a71-275">Exemplos de recursos</span><span class="sxs-lookup"><span data-stu-id="d4a71-275">Resources examples</span></span>

<span data-ttu-id="d4a71-276">Os valores a seguir são válidos para a propriedade resource.</span><span class="sxs-lookup"><span data-stu-id="d4a71-276">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="d4a71-277">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="d4a71-277">Resource type</span></span> | <span data-ttu-id="d4a71-278">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d4a71-278">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="d4a71-279">Registros de chamadas</span><span class="sxs-lookup"><span data-stu-id="d4a71-279">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="d4a71-280">Canais</span><span class="sxs-lookup"><span data-stu-id="d4a71-280">Channels</span></span>](../resources/channel.md)|<span data-ttu-id="d4a71-281">`/teams/getAllChannels`, `/teams/{id}/channels`</span><span class="sxs-lookup"><span data-stu-id="d4a71-281">`/teams/getAllChannels`, `/teams/{id}/channels`</span></span>|
|[<span data-ttu-id="d4a71-282">Chat</span><span class="sxs-lookup"><span data-stu-id="d4a71-282">Chat</span></span>](../resources/chat.md)|<span data-ttu-id="d4a71-283">`/chats`, `/chats/{id}`</span><span class="sxs-lookup"><span data-stu-id="d4a71-283">`/chats`, `/chats/{id}`</span></span>|
|[<span data-ttu-id="d4a71-284">Mensagem de chat</span><span class="sxs-lookup"><span data-stu-id="d4a71-284">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="d4a71-285">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="d4a71-285">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="d4a71-286">Contatos</span><span class="sxs-lookup"><span data-stu-id="d4a71-286">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="d4a71-287">ConversationMember</span><span class="sxs-lookup"><span data-stu-id="d4a71-287">ConversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="d4a71-288">`/chats/{id}/members`, `/chats/getAllMembers`, `/teams/{id}/members`</span><span class="sxs-lookup"><span data-stu-id="d4a71-288">`/chats/{id}/members`, `/chats/getAllMembers`, `/teams/{id}/members`</span></span>|
|[<span data-ttu-id="d4a71-289">Conversas</span><span class="sxs-lookup"><span data-stu-id="d4a71-289">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="d4a71-290">Unidades</span><span class="sxs-lookup"><span data-stu-id="d4a71-290">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="d4a71-291">Eventos</span><span class="sxs-lookup"><span data-stu-id="d4a71-291">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="d4a71-292">Grupos</span><span class="sxs-lookup"><span data-stu-id="d4a71-292">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="d4a71-293">Lista</span><span class="sxs-lookup"><span data-stu-id="d4a71-293">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="d4a71-294">Email</span><span class="sxs-lookup"><span data-stu-id="d4a71-294">Mail</span></span>](../resources/message.md)|<span data-ttu-id="d4a71-295">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="d4a71-295">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="d4a71-296">Presença</span><span class="sxs-lookup"><span data-stu-id="d4a71-296">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="d4a71-297">`/communications/presences/{id}` (usuário único), `/communications/presences?$filter=id in ({id},{id}…)` (vários usuários)</span><span class="sxs-lookup"><span data-stu-id="d4a71-297">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|[<span data-ttu-id="d4a71-298">impressora</span><span class="sxs-lookup"><span data-stu-id="d4a71-298">printer</span></span>](../resources/printer.md) |`print/printers/{id}/jobs`|
|[<span data-ttu-id="d4a71-299">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="d4a71-299">PrintTaskDefinition</span></span>](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[<span data-ttu-id="d4a71-300">Teams</span><span class="sxs-lookup"><span data-stu-id="d4a71-300">Teams</span></span>](../resources/team.md)|<span data-ttu-id="d4a71-301">`/teams`, `/teams/{id}`</span><span class="sxs-lookup"><span data-stu-id="d4a71-301">`/teams`, `/teams/{id}`</span></span>|
|[<span data-ttu-id="d4a71-302">Usuários</span><span class="sxs-lookup"><span data-stu-id="d4a71-302">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="d4a71-303">todoTask</span><span class="sxs-lookup"><span data-stu-id="d4a71-303">todoTask</span></span>](../resources/todotask.md) | `/me/todo/lists/{todoTaskListId}/tasks`
|[<span data-ttu-id="d4a71-304">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="d4a71-304">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> <span data-ttu-id="d4a71-305">**Observação:** qualquer caminho iniciado por `me` também pode ser usado com `users/{id}` em vez de `me` para direcionar um usuário específico, em vez de usar o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="d4a71-305">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="d4a71-306">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4a71-306">Response</span></span>

<span data-ttu-id="d4a71-307">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="d4a71-307">The following example shows the response.</span></span> 

><span data-ttu-id="d4a71-308">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d4a71-308">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2",
  "notificationContentType": "application/json"
}
```

### <a name="notification-endpoint-validation"></a><span data-ttu-id="d4a71-309">Validação de ponto de extremidade de notificação</span><span class="sxs-lookup"><span data-stu-id="d4a71-309">Notification endpoint validation</span></span>

<span data-ttu-id="d4a71-310">O ponto de extremidade de notificação de assinatura (especificado na propriedade **notificationUrl)** deve ser capaz de responder a uma solicitação de validação conforme descrito em [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="d4a71-310">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="d4a71-311">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="d4a71-311">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

[error-response]: /graph/errors

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


