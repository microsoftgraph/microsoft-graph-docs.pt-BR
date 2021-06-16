---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: d2692e1af87fd7449829ab646d14dd6c3d5a067a
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941484"
---
# <a name="delete-subscription"></a><span data-ttu-id="e7d01-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="e7d01-103">Delete subscription</span></span>

<span data-ttu-id="e7d01-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7d01-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7d01-105">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="e7d01-105">Delete a subscription.</span></span>

<span data-ttu-id="e7d01-106">Consulte a tabela na seção [Permissões](#permissions) para obter a lista de recursos que oferecem suporte à inscrição para alterar notificações.</span><span class="sxs-lookup"><span data-stu-id="e7d01-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7d01-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7d01-107">Permissions</span></span>

<span data-ttu-id="e7d01-108">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="e7d01-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="e7d01-109">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7d01-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e7d01-110">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-110">Supported resource</span></span> | <span data-ttu-id="e7d01-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7d01-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e7d01-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7d01-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7d01-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7d01-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="e7d01-114">callRecord</span><span class="sxs-lookup"><span data-stu-id="e7d01-114">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="e7d01-115">Incompatível</span><span class="sxs-lookup"><span data-stu-id="e7d01-115">Not supported</span></span> | <span data-ttu-id="e7d01-116">Incompatível</span><span class="sxs-lookup"><span data-stu-id="e7d01-116">Not supported</span></span> | <span data-ttu-id="e7d01-117">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-117">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="e7d01-118">[canais](../resources/channel.md) (/teams/getAllChannels – todos os canais em uma organização)</span><span class="sxs-lookup"><span data-stu-id="e7d01-118">[channels](../resources/channel.md) (/teams/getAllChannels – all channels in an organization)</span></span> | <span data-ttu-id="e7d01-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-119">Not supported</span></span>  | <span data-ttu-id="e7d01-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-120">Not supported</span></span> | <span data-ttu-id="e7d01-121">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-121">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> |
|<span data-ttu-id="e7d01-122">[canais](../resources/channel.md) (/teams/{id}/channels)</span><span class="sxs-lookup"><span data-stu-id="e7d01-122">[channels](../resources/channel.md) (/teams/{id}/channels)</span></span> | <span data-ttu-id="e7d01-123">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-123">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  | <span data-ttu-id="e7d01-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-124">Not supported</span></span> | <span data-ttu-id="e7d01-125">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-125">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  |
|<span data-ttu-id="e7d01-126">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="e7d01-126">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="e7d01-127">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-127">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="e7d01-128">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-128">Not supported</span></span> | <span data-ttu-id="e7d01-129">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-129">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="e7d01-130">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="e7d01-130">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="e7d01-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-131">Not supported</span></span> | <span data-ttu-id="e7d01-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-132">Not supported</span></span> | <span data-ttu-id="e7d01-133">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-133">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="e7d01-134">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="e7d01-134">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="e7d01-135">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7d01-135">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="e7d01-136">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-136">Not supported</span></span> | <span data-ttu-id="e7d01-137">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-137">Chat.Read.All</span></span>  |
|<span data-ttu-id="e7d01-138">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="e7d01-138">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="e7d01-139">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-139">Not supported</span></span> | <span data-ttu-id="e7d01-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-140">Not supported</span></span> | <span data-ttu-id="e7d01-141">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-141">Chat.Read.All</span></span>  |
|[<span data-ttu-id="e7d01-142">contato</span><span class="sxs-lookup"><span data-stu-id="e7d01-142">contact</span></span>](../resources/contact.md) | <span data-ttu-id="e7d01-143">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e7d01-143">Contacts.Read</span></span> | <span data-ttu-id="e7d01-144">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e7d01-144">Contacts.Read</span></span> | <span data-ttu-id="e7d01-145">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e7d01-145">Contacts.Read</span></span> |
|<span data-ttu-id="e7d01-146">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span><span class="sxs-lookup"><span data-stu-id="e7d01-146">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span></span> | <span data-ttu-id="e7d01-147">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-147">TeamMember.Read.All</span></span> | <span data-ttu-id="e7d01-148">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-148">Not supported</span></span> | <span data-ttu-id="e7d01-149">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-149">TeamMember.Read.All</span></span> |
|<span data-ttu-id="e7d01-150">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="e7d01-150">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="e7d01-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-151">Not supported</span></span> | <span data-ttu-id="e7d01-152">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7d01-152">Files.ReadWrite</span></span> | <span data-ttu-id="e7d01-153">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-153">Not supported</span></span> |
|<span data-ttu-id="e7d01-154">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="e7d01-154">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="e7d01-155">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-155">Files.ReadWrite.All</span></span> | <span data-ttu-id="e7d01-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-156">Not supported</span></span> | <span data-ttu-id="e7d01-157">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-157">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="e7d01-158">evento</span><span class="sxs-lookup"><span data-stu-id="e7d01-158">event</span></span>](../resources/event.md) | <span data-ttu-id="e7d01-159">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e7d01-159">Calendars.Read</span></span> | <span data-ttu-id="e7d01-160">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e7d01-160">Calendars.Read</span></span> | <span data-ttu-id="e7d01-161">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e7d01-161">Calendars.Read</span></span> |
|[<span data-ttu-id="e7d01-162">grupo</span><span class="sxs-lookup"><span data-stu-id="e7d01-162">group</span></span>](../resources/group.md) | <span data-ttu-id="e7d01-163">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-163">Group.Read.All</span></span> | <span data-ttu-id="e7d01-164">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-164">Not supported</span></span> | <span data-ttu-id="e7d01-165">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-165">Group.Read.All</span></span> |
|[<span data-ttu-id="e7d01-166">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="e7d01-166">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="e7d01-167">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-167">Group.Read.All</span></span> | <span data-ttu-id="e7d01-168">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-168">Not supported</span></span> | <span data-ttu-id="e7d01-169">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-169">Not supported</span></span> |
|[<span data-ttu-id="e7d01-170">list</span><span class="sxs-lookup"><span data-stu-id="e7d01-170">list</span></span>](../resources/list.md) | <span data-ttu-id="e7d01-171">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-171">Sites.ReadWrite.All</span></span> | <span data-ttu-id="e7d01-172">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-172">Not supported</span></span> | <span data-ttu-id="e7d01-173">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-173">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="e7d01-174">message</span><span class="sxs-lookup"><span data-stu-id="e7d01-174">message</span></span>](../resources/message.md) | <span data-ttu-id="e7d01-175">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e7d01-175">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="e7d01-176">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e7d01-176">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="e7d01-177">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e7d01-177">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="e7d01-178">presence</span><span class="sxs-lookup"><span data-stu-id="e7d01-178">presence</span></span>](../resources/presence.md) | <span data-ttu-id="e7d01-179">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-179">Presence.Read.All</span></span> | <span data-ttu-id="e7d01-180">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-180">Not supported</span></span> | <span data-ttu-id="e7d01-181">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-181">Not supported</span></span> |
|[<span data-ttu-id="e7d01-182">printer</span><span class="sxs-lookup"><span data-stu-id="e7d01-182">printer</span></span>](../resources/printer.md) | <span data-ttu-id="e7d01-183">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-183">Not supported</span></span> | <span data-ttu-id="e7d01-184">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-184">Not supported</span></span> | <span data-ttu-id="e7d01-185">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-185">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="e7d01-186">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="e7d01-186">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="e7d01-187">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-187">Not supported</span></span> | <span data-ttu-id="e7d01-188">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-188">Not supported</span></span> | <span data-ttu-id="e7d01-189">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-189">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="e7d01-190">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="e7d01-190">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="e7d01-191">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-191">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="e7d01-192">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-192">Not supported</span></span> | <span data-ttu-id="e7d01-193">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-193">SecurityEvents.ReadWrite.All</span></span> |
|<span data-ttu-id="e7d01-194">[teams](../resources/team.md) (/teams – todas as equipes em uma organização)</span><span class="sxs-lookup"><span data-stu-id="e7d01-194">[teams](../resources/team.md) (/teams – all teams in an organization)</span></span> | <span data-ttu-id="e7d01-195">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-195">Not supported</span></span> | <span data-ttu-id="e7d01-196">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-196">Not supported</span></span> | <span data-ttu-id="e7d01-197">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-197">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|<span data-ttu-id="e7d01-198">[teams](../resources/team.md) (/teams/{id})</span><span class="sxs-lookup"><span data-stu-id="e7d01-198">[teams](../resources/team.md) (/teams/{id})</span></span> | <span data-ttu-id="e7d01-199">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-199">Team.ReadBasic.All, TeamSettings.Read.All</span></span> | <span data-ttu-id="e7d01-200">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-200">Not supported</span></span> | <span data-ttu-id="e7d01-201">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-201">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|[<span data-ttu-id="e7d01-202">todoTask</span><span class="sxs-lookup"><span data-stu-id="e7d01-202">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="e7d01-203">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7d01-203">Tasks.ReadWrite</span></span> | <span data-ttu-id="e7d01-204">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7d01-204">Tasks.ReadWrite</span></span> | <span data-ttu-id="e7d01-205">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7d01-205">Not supported</span></span> |
|[<span data-ttu-id="e7d01-206">Usuário</span><span class="sxs-lookup"><span data-stu-id="e7d01-206">user</span></span>](../resources/user.md) | <span data-ttu-id="e7d01-207">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-207">User.Read.All</span></span> | <span data-ttu-id="e7d01-208">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-208">User.Read.All</span></span> | <span data-ttu-id="e7d01-209">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d01-209">User.Read.All</span></span> |

> <span data-ttu-id="e7d01-210">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="e7d01-210">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="e7d01-211">driveItem</span><span class="sxs-lookup"><span data-stu-id="e7d01-211">driveItem</span></span>

<span data-ttu-id="e7d01-212">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e7d01-212">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="e7d01-213">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="e7d01-213">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="e7d01-214">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="e7d01-214">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="e7d01-215">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="e7d01-215">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="e7d01-216">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="e7d01-216">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="e7d01-217">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="e7d01-217">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="e7d01-218">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="e7d01-218">contact, event, and message</span></span>

<span data-ttu-id="e7d01-219">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="e7d01-219">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="e7d01-220">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="e7d01-220">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="e7d01-221">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="e7d01-221">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="e7d01-222">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="e7d01-222">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="e7d01-223">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="e7d01-223">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="e7d01-224">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="e7d01-224">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="e7d01-225">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="e7d01-225">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="e7d01-226">presença</span><span class="sxs-lookup"><span data-stu-id="e7d01-226">presence</span></span>

<span data-ttu-id="e7d01-227">**assinaturas** de presença exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="e7d01-227">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="e7d01-228">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="e7d01-228">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="e7d01-229">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7d01-229">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="e7d01-230">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d01-230">Request headers</span></span>

| <span data-ttu-id="e7d01-231">Nome</span><span class="sxs-lookup"><span data-stu-id="e7d01-231">Name</span></span>       | <span data-ttu-id="e7d01-232">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7d01-232">Type</span></span> | <span data-ttu-id="e7d01-233">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7d01-233">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e7d01-234">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7d01-234">Authorization</span></span>  | <span data-ttu-id="e7d01-235">string</span><span class="sxs-lookup"><span data-stu-id="e7d01-235">string</span></span>  | <span data-ttu-id="e7d01-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7d01-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7d01-238">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d01-238">Request body</span></span>

<span data-ttu-id="e7d01-239">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7d01-239">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7d01-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7d01-240">Response</span></span>

<span data-ttu-id="e7d01-241">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e7d01-241">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="e7d01-242">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="e7d01-242">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="e7d01-243">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7d01-243">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e7d01-244">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d01-244">Request</span></span>

<span data-ttu-id="e7d01-245">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7d01-245">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e7d01-246">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7d01-246">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="e7d01-247">C#</span><span class="sxs-lookup"><span data-stu-id="e7d01-247">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e7d01-248">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7d01-248">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e7d01-249">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7d01-249">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e7d01-250">Java</span><span class="sxs-lookup"><span data-stu-id="e7d01-250">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e7d01-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7d01-251">Response</span></span>

<span data-ttu-id="e7d01-252">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7d01-252">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


