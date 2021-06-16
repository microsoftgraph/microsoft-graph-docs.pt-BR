---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 592631033cc411e034433d8fe33648b513da403f
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941502"
---
# <a name="update-subscription"></a><span data-ttu-id="e1b30-103">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="e1b30-103">Update subscription</span></span>

<span data-ttu-id="e1b30-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1b30-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1b30-105">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="e1b30-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="e1b30-106">A tabela na seção [Permissões](#permissions) lista os recursos que suportam a assinatura para alterar notificações.</span><span class="sxs-lookup"><span data-stu-id="e1b30-106">The table in the [Permissions](#permissions) section lists the resources that support subscribing to change notifications.</span></span>

<span data-ttu-id="e1b30-107">As assinaturas expiram após um período de tempo que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="e1b30-107">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="e1b30-108">Para evitar notificações de alteração ausentes, um aplicativo deve renovar suas assinaturas bem antes da data de expiração.</span><span class="sxs-lookup"><span data-stu-id="e1b30-108">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="e1b30-109">Consulte [assinatura](../resources/subscription.md) para o tamanho máximo de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="e1b30-109">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1b30-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1b30-110">Permissions</span></span>

<span data-ttu-id="e1b30-111">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="e1b30-111">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="e1b30-112">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1b30-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e1b30-113">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-113">Supported resource</span></span> | <span data-ttu-id="e1b30-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1b30-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e1b30-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1b30-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1b30-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1b30-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="e1b30-117">callRecord</span><span class="sxs-lookup"><span data-stu-id="e1b30-117">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="e1b30-118">Incompatível</span><span class="sxs-lookup"><span data-stu-id="e1b30-118">Not supported</span></span> | <span data-ttu-id="e1b30-119">Incompatível</span><span class="sxs-lookup"><span data-stu-id="e1b30-119">Not supported</span></span> | <span data-ttu-id="e1b30-120">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-120">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="e1b30-121">[canais](../resources/channel.md) (/teams/getAllChannels – todos os canais em uma organização)</span><span class="sxs-lookup"><span data-stu-id="e1b30-121">[channels](../resources/channel.md) (/teams/getAllChannels – all channels in an organization)</span></span> | <span data-ttu-id="e1b30-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-122">Not supported</span></span>  | <span data-ttu-id="e1b30-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-123">Not supported</span></span> | <span data-ttu-id="e1b30-124">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-124">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> |
|<span data-ttu-id="e1b30-125">[canais](../resources/channel.md) (/teams/{id}/channels)</span><span class="sxs-lookup"><span data-stu-id="e1b30-125">[channels](../resources/channel.md) (/teams/{id}/channels)</span></span> | <span data-ttu-id="e1b30-126">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-126">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  | <span data-ttu-id="e1b30-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-127">Not supported</span></span> | <span data-ttu-id="e1b30-128">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-128">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  |
|<span data-ttu-id="e1b30-129">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="e1b30-129">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="e1b30-130">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-130">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="e1b30-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-131">Not supported</span></span> | <span data-ttu-id="e1b30-132">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-132">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="e1b30-133">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="e1b30-133">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="e1b30-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-134">Not supported</span></span> | <span data-ttu-id="e1b30-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-135">Not supported</span></span> | <span data-ttu-id="e1b30-136">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-136">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="e1b30-137">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="e1b30-137">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="e1b30-138">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1b30-138">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="e1b30-139">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-139">Not supported</span></span> | <span data-ttu-id="e1b30-140">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-140">Chat.Read.All</span></span>  |
|<span data-ttu-id="e1b30-141">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="e1b30-141">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="e1b30-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-142">Not supported</span></span> | <span data-ttu-id="e1b30-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-143">Not supported</span></span> | <span data-ttu-id="e1b30-144">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-144">Chat.Read.All</span></span>  |
|[<span data-ttu-id="e1b30-145">contato</span><span class="sxs-lookup"><span data-stu-id="e1b30-145">contact</span></span>](../resources/contact.md) | <span data-ttu-id="e1b30-146">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e1b30-146">Contacts.Read</span></span> | <span data-ttu-id="e1b30-147">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e1b30-147">Contacts.Read</span></span> | <span data-ttu-id="e1b30-148">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e1b30-148">Contacts.Read</span></span> |
|<span data-ttu-id="e1b30-149">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span><span class="sxs-lookup"><span data-stu-id="e1b30-149">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span></span> | <span data-ttu-id="e1b30-150">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-150">TeamMember.Read.All</span></span> | <span data-ttu-id="e1b30-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-151">Not supported</span></span> | <span data-ttu-id="e1b30-152">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-152">TeamMember.Read.All</span></span> |
|<span data-ttu-id="e1b30-153">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="e1b30-153">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="e1b30-154">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-154">Not supported</span></span> | <span data-ttu-id="e1b30-155">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1b30-155">Files.ReadWrite</span></span> | <span data-ttu-id="e1b30-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-156">Not supported</span></span> |
|<span data-ttu-id="e1b30-157">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="e1b30-157">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="e1b30-158">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-158">Files.ReadWrite.All</span></span> | <span data-ttu-id="e1b30-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-159">Not supported</span></span> | <span data-ttu-id="e1b30-160">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-160">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="e1b30-161">evento</span><span class="sxs-lookup"><span data-stu-id="e1b30-161">event</span></span>](../resources/event.md) | <span data-ttu-id="e1b30-162">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e1b30-162">Calendars.Read</span></span> | <span data-ttu-id="e1b30-163">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e1b30-163">Calendars.Read</span></span> | <span data-ttu-id="e1b30-164">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e1b30-164">Calendars.Read</span></span> |
|[<span data-ttu-id="e1b30-165">grupo</span><span class="sxs-lookup"><span data-stu-id="e1b30-165">group</span></span>](../resources/group.md) | <span data-ttu-id="e1b30-166">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-166">Group.Read.All</span></span> | <span data-ttu-id="e1b30-167">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-167">Not supported</span></span> | <span data-ttu-id="e1b30-168">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-168">Group.Read.All</span></span> |
|[<span data-ttu-id="e1b30-169">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="e1b30-169">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="e1b30-170">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-170">Group.Read.All</span></span> | <span data-ttu-id="e1b30-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-171">Not supported</span></span> | <span data-ttu-id="e1b30-172">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-172">Not supported</span></span> |
|[<span data-ttu-id="e1b30-173">list</span><span class="sxs-lookup"><span data-stu-id="e1b30-173">list</span></span>](../resources/list.md) | <span data-ttu-id="e1b30-174">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-174">Sites.ReadWrite.All</span></span> | <span data-ttu-id="e1b30-175">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-175">Not supported</span></span> | <span data-ttu-id="e1b30-176">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-176">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="e1b30-177">message</span><span class="sxs-lookup"><span data-stu-id="e1b30-177">message</span></span>](../resources/message.md) | <span data-ttu-id="e1b30-178">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e1b30-178">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="e1b30-179">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e1b30-179">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="e1b30-180">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e1b30-180">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="e1b30-181">presence</span><span class="sxs-lookup"><span data-stu-id="e1b30-181">presence</span></span>](../resources/presence.md) | <span data-ttu-id="e1b30-182">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-182">Presence.Read.All</span></span> | <span data-ttu-id="e1b30-183">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-183">Not supported</span></span> | <span data-ttu-id="e1b30-184">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-184">Not supported</span></span> |
|[<span data-ttu-id="e1b30-185">printer</span><span class="sxs-lookup"><span data-stu-id="e1b30-185">printer</span></span>](../resources/printer.md) | <span data-ttu-id="e1b30-186">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-186">Not supported</span></span> | <span data-ttu-id="e1b30-187">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-187">Not supported</span></span> | <span data-ttu-id="e1b30-188">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-188">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="e1b30-189">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="e1b30-189">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="e1b30-190">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-190">Not supported</span></span> | <span data-ttu-id="e1b30-191">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-191">Not supported</span></span> | <span data-ttu-id="e1b30-192">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-192">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="e1b30-193">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="e1b30-193">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="e1b30-194">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-194">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="e1b30-195">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-195">Not supported</span></span> | <span data-ttu-id="e1b30-196">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-196">SecurityEvents.ReadWrite.All</span></span> |
|<span data-ttu-id="e1b30-197">[teams](../resources/team.md) (/teams – todas as equipes em uma organização)</span><span class="sxs-lookup"><span data-stu-id="e1b30-197">[teams](../resources/team.md) (/teams – all teams in an organization)</span></span> | <span data-ttu-id="e1b30-198">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-198">Not supported</span></span> | <span data-ttu-id="e1b30-199">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-199">Not supported</span></span> | <span data-ttu-id="e1b30-200">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-200">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|<span data-ttu-id="e1b30-201">[teams](../resources/team.md) (/teams/{id})</span><span class="sxs-lookup"><span data-stu-id="e1b30-201">[teams](../resources/team.md) (/teams/{id})</span></span> | <span data-ttu-id="e1b30-202">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-202">Team.ReadBasic.All, TeamSettings.Read.All</span></span> | <span data-ttu-id="e1b30-203">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-203">Not supported</span></span> | <span data-ttu-id="e1b30-204">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-204">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|[<span data-ttu-id="e1b30-205">todoTask</span><span class="sxs-lookup"><span data-stu-id="e1b30-205">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="e1b30-206">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1b30-206">Tasks.ReadWrite</span></span> | <span data-ttu-id="e1b30-207">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1b30-207">Tasks.ReadWrite</span></span> | <span data-ttu-id="e1b30-208">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1b30-208">Not supported</span></span> |
|[<span data-ttu-id="e1b30-209">Usuário</span><span class="sxs-lookup"><span data-stu-id="e1b30-209">user</span></span>](../resources/user.md) | <span data-ttu-id="e1b30-210">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-210">User.Read.All</span></span> | <span data-ttu-id="e1b30-211">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-211">User.Read.All</span></span> | <span data-ttu-id="e1b30-212">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b30-212">User.Read.All</span></span> |

> <span data-ttu-id="e1b30-213">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="e1b30-213">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="e1b30-214">driveItem</span><span class="sxs-lookup"><span data-stu-id="e1b30-214">driveItem</span></span>

<span data-ttu-id="e1b30-215">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e1b30-215">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="e1b30-216">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="e1b30-216">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="e1b30-217">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="e1b30-217">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="e1b30-218">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="e1b30-218">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="e1b30-219">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="e1b30-219">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="e1b30-220">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="e1b30-220">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="e1b30-221">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="e1b30-221">contact, event, and message</span></span>

<span data-ttu-id="e1b30-222">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="e1b30-222">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="e1b30-223">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="e1b30-223">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="e1b30-224">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="e1b30-224">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="e1b30-225">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="e1b30-225">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="e1b30-226">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="e1b30-226">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="e1b30-227">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="e1b30-227">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="e1b30-228">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="e1b30-228">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="e1b30-229">presença</span><span class="sxs-lookup"><span data-stu-id="e1b30-229">presence</span></span>

<span data-ttu-id="e1b30-230">**assinaturas** de presença exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="e1b30-230">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="e1b30-231">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="e1b30-231">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="e1b30-232">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1b30-232">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e1b30-233">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1b30-233">Request headers</span></span>

| <span data-ttu-id="e1b30-234">Nome</span><span class="sxs-lookup"><span data-stu-id="e1b30-234">Name</span></span>       | <span data-ttu-id="e1b30-235">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1b30-235">Type</span></span> | <span data-ttu-id="e1b30-236">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1b30-236">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e1b30-237">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1b30-237">Authorization</span></span>  | <span data-ttu-id="e1b30-238">string</span><span class="sxs-lookup"><span data-stu-id="e1b30-238">string</span></span>  | <span data-ttu-id="e1b30-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1b30-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e1b30-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1b30-241">Response</span></span>

<span data-ttu-id="e1b30-242">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1b30-242">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="e1b30-243">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="e1b30-243">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="e1b30-244">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1b30-244">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e1b30-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1b30-245">Request</span></span>

<span data-ttu-id="e1b30-246">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1b30-246">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e1b30-247">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1b30-247">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e1b30-248">C#</span><span class="sxs-lookup"><span data-stu-id="e1b30-248">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1b30-249">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1b30-249">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1b30-250">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1b30-250">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1b30-251">Java</span><span class="sxs-lookup"><span data-stu-id="e1b30-251">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e1b30-252">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1b30-252">Response</span></span>

<span data-ttu-id="e1b30-253">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1b30-253">Here is an example of the response.</span></span>
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


