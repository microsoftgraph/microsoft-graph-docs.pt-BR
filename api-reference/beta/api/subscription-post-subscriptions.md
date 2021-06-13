---
title: Criar assinatura
description: Inscreve um aplicativo ouvinte para receber notificações de alteração quando os dados em um recurso microsoft Graph alterações.
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: b471d13836faa74ba6f77ab395e9a8ad3c87e4ad
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911862"
---
# <a name="create-subscription"></a><span data-ttu-id="7f4e6-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="7f4e6-103">Create subscription</span></span>

<span data-ttu-id="7f4e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f4e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f4e6-105">Inscreve um aplicativo de ouvinte para receber notificações de alterações quando o tipo de alteração solicitado ocorrer no recurso especificado no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

<span data-ttu-id="7f4e6-106">Consulte a tabela na seção [Permissões](#permissions) para obter a lista de recursos que oferecem suporte à inscrição para alterar notificações.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f4e6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f4e6-107">Permissions</span></span>

<span data-ttu-id="7f4e6-108">A criação de uma assinatura requer permissão de leitura para o recurso.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-108">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="7f4e6-109">Por exemplo, para receber notificações de alteração em mensagens, seu aplicativo precisa da permissão Mail.Read.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-109">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 

<span data-ttu-id="7f4e6-110">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="7f4e6-111">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f4e6-111">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f4e6-112">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-112">Supported resource</span></span> | <span data-ttu-id="7f4e6-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f4e6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7f4e6-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f4e6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f4e6-115">Application</span><span class="sxs-lookup"><span data-stu-id="7f4e6-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="7f4e6-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="7f4e6-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="7f4e6-117">Incompatível</span><span class="sxs-lookup"><span data-stu-id="7f4e6-117">Not supported</span></span> | <span data-ttu-id="7f4e6-118">Incompatível</span><span class="sxs-lookup"><span data-stu-id="7f4e6-118">Not supported</span></span> | <span data-ttu-id="7f4e6-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="7f4e6-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="7f4e6-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="7f4e6-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="7f4e6-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-122">Not supported</span></span> | <span data-ttu-id="7f4e6-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="7f4e6-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="7f4e6-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="7f4e6-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-125">Not supported</span></span> | <span data-ttu-id="7f4e6-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-126">Not supported</span></span> | <span data-ttu-id="7f4e6-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="7f4e6-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="7f4e6-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="7f4e6-129">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f4e6-129">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="7f4e6-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-130">Not supported</span></span> | <span data-ttu-id="7f4e6-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="7f4e6-132">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="7f4e6-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="7f4e6-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-133">Not supported</span></span> | <span data-ttu-id="7f4e6-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-134">Not supported</span></span> | <span data-ttu-id="7f4e6-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="7f4e6-136">contato</span><span class="sxs-lookup"><span data-stu-id="7f4e6-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="7f4e6-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7f4e6-137">Contacts.Read</span></span> | <span data-ttu-id="7f4e6-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7f4e6-138">Contacts.Read</span></span> | <span data-ttu-id="7f4e6-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7f4e6-139">Contacts.Read</span></span> |
|<span data-ttu-id="7f4e6-140">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="7f4e6-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="7f4e6-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-141">Not supported</span></span> | <span data-ttu-id="7f4e6-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f4e6-142">Files.ReadWrite</span></span> | <span data-ttu-id="7f4e6-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-143">Not supported</span></span> |
|<span data-ttu-id="7f4e6-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="7f4e6-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="7f4e6-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="7f4e6-146">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-146">Not supported</span></span> | <span data-ttu-id="7f4e6-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="7f4e6-148">evento</span><span class="sxs-lookup"><span data-stu-id="7f4e6-148">event</span></span>](../resources/event.md) | <span data-ttu-id="7f4e6-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7f4e6-149">Calendars.Read</span></span> | <span data-ttu-id="7f4e6-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7f4e6-150">Calendars.Read</span></span> | <span data-ttu-id="7f4e6-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7f4e6-151">Calendars.Read</span></span> |
|[<span data-ttu-id="7f4e6-152">grupo</span><span class="sxs-lookup"><span data-stu-id="7f4e6-152">group</span></span>](../resources/group.md) | <span data-ttu-id="7f4e6-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-153">Group.Read.All</span></span> | <span data-ttu-id="7f4e6-154">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-154">Not supported</span></span> | <span data-ttu-id="7f4e6-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-155">Group.Read.All</span></span> |
|[<span data-ttu-id="7f4e6-156">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="7f4e6-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="7f4e6-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-157">Group.Read.All</span></span> | <span data-ttu-id="7f4e6-158">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-158">Not supported</span></span> | <span data-ttu-id="7f4e6-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-159">Not supported</span></span> |
|[<span data-ttu-id="7f4e6-160">list</span><span class="sxs-lookup"><span data-stu-id="7f4e6-160">list</span></span>](../resources/list.md) | <span data-ttu-id="7f4e6-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="7f4e6-162">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-162">Not supported</span></span> | <span data-ttu-id="7f4e6-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="7f4e6-164">message</span><span class="sxs-lookup"><span data-stu-id="7f4e6-164">message</span></span>](../resources/message.md) | <span data-ttu-id="7f4e6-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7f4e6-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="7f4e6-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7f4e6-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="7f4e6-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7f4e6-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="7f4e6-168">presence</span><span class="sxs-lookup"><span data-stu-id="7f4e6-168">presence</span></span>](../resources/presence.md) | <span data-ttu-id="7f4e6-169">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-169">Presence.Read.All</span></span> | <span data-ttu-id="7f4e6-170">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-170">Not supported</span></span> | <span data-ttu-id="7f4e6-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-171">Not supported</span></span> |
|[<span data-ttu-id="7f4e6-172">printer</span><span class="sxs-lookup"><span data-stu-id="7f4e6-172">printer</span></span>](../resources/printer.md) | <span data-ttu-id="7f4e6-173">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-173">Not supported</span></span> | <span data-ttu-id="7f4e6-174">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-174">Not supported</span></span> | <span data-ttu-id="7f4e6-175">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-175">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="7f4e6-176">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="7f4e6-176">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="7f4e6-177">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-177">Not supported</span></span> | <span data-ttu-id="7f4e6-178">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-178">Not supported</span></span> | <span data-ttu-id="7f4e6-179">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-179">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="7f4e6-180">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="7f4e6-180">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="7f4e6-181">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-181">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="7f4e6-182">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-182">Not supported</span></span> | <span data-ttu-id="7f4e6-183">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-183">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="7f4e6-184">todoTask</span><span class="sxs-lookup"><span data-stu-id="7f4e6-184">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="7f4e6-185">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f4e6-185">Tasks.ReadWrite</span></span> | <span data-ttu-id="7f4e6-186">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f4e6-186">Tasks.ReadWrite</span></span> | <span data-ttu-id="7f4e6-187">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f4e6-187">Not supported</span></span> |
|[<span data-ttu-id="7f4e6-188">Usuário</span><span class="sxs-lookup"><span data-stu-id="7f4e6-188">user</span></span>](../resources/user.md) | <span data-ttu-id="7f4e6-189">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-189">User.Read.All</span></span> | <span data-ttu-id="7f4e6-190">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-190">User.Read.All</span></span> | <span data-ttu-id="7f4e6-191">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f4e6-191">User.Read.All</span></span> |

> <span data-ttu-id="7f4e6-192">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="7f4e6-192">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="7f4e6-193">driveItem</span><span class="sxs-lookup"><span data-stu-id="7f4e6-193">driveItem</span></span>

<span data-ttu-id="7f4e6-194">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-194">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="7f4e6-195">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="7f4e6-195">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="7f4e6-196">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-196">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="7f4e6-197">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-197">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="7f4e6-198">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-198">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="7f4e6-199">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-199">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

<span data-ttu-id="7f4e6-200">OneDrive for Business e SharePoint suporte ao envio de notificações do aplicativo de eventos de segurança que ocorrem em **um driveItem**.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-200">OneDrive for Business and SharePoint support sending your application notifications of security events that occur on a **driveItem**.</span></span> <span data-ttu-id="7f4e6-201">Para assinar esses eventos, adicione o `prefer:includesecuritywebhooks` header à sua solicitação para criar uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-201">To subscribe to these events, add the `prefer:includesecuritywebhooks` header to your request to create a subscription.</span></span> <span data-ttu-id="7f4e6-202">Depois que a assinatura for criada, você receberá notificações quando as permissões em um item mudarem.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-202">After the subscription is created, you will receive notifications when the permissions on an item change.</span></span> <span data-ttu-id="7f4e6-203">Esse header é aplicável a SharePoint e OneDrive for Business, mas não a contas OneDrive clientes.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-203">This header is applicable to SharePoint and OneDrive for Business but not consumer OneDrive accounts.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="7f4e6-204">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="7f4e6-204">contact, event, and message</span></span>

<span data-ttu-id="7f4e6-205">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-205">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="7f4e6-206">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="7f4e6-206">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="7f4e6-207">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-207">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="7f4e6-208">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-208">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="7f4e6-209">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="7f4e6-209">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="7f4e6-210">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-210">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="7f4e6-211">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-211">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="7f4e6-212">presença</span><span class="sxs-lookup"><span data-stu-id="7f4e6-212">presence</span></span>

<span data-ttu-id="7f4e6-213">**assinaturas** de presença exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="7f4e6-213">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="7f4e6-214">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-214">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="7f4e6-215">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f4e6-215">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="7f4e6-216">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f4e6-216">Request headers</span></span>

| <span data-ttu-id="7f4e6-217">Nome</span><span class="sxs-lookup"><span data-stu-id="7f4e6-217">Name</span></span>       | <span data-ttu-id="7f4e6-218">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f4e6-218">Type</span></span> | <span data-ttu-id="7f4e6-219">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f4e6-219">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7f4e6-220">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f4e6-220">Authorization</span></span>  | <span data-ttu-id="7f4e6-221">string</span><span class="sxs-lookup"><span data-stu-id="7f4e6-221">string</span></span>  | <span data-ttu-id="7f4e6-p109">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7f4e6-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f4e6-224">Response</span></span>

<span data-ttu-id="7f4e6-225">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-225">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="7f4e6-226">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="7f4e6-226">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="7f4e6-227">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f4e6-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f4e6-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f4e6-228">Request</span></span>

<span data-ttu-id="7f4e6-229">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="7f4e6-229">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="7f4e6-230">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-230">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="7f4e6-231">Essa solicitação cria uma assinatura para notificações de alteração sobre novos emails recebidos pelo usuário atualmente inscrito.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-231">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f4e6-232">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f4e6-232">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7f4e6-233">C#</span><span class="sxs-lookup"><span data-stu-id="7f4e6-233">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f4e6-234">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f4e6-234">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f4e6-235">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f4e6-235">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f4e6-236">Java</span><span class="sxs-lookup"><span data-stu-id="7f4e6-236">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7f4e6-237">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="7f4e6-237">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="7f4e6-238">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-238">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

#### <a name="resources-examples"></a><span data-ttu-id="7f4e6-239">Exemplos de recursos</span><span class="sxs-lookup"><span data-stu-id="7f4e6-239">Resources examples</span></span>

<span data-ttu-id="7f4e6-240">Os valores a seguir são válidos para a propriedade resource.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-240">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="7f4e6-241">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="7f4e6-241">Resource type</span></span> | <span data-ttu-id="7f4e6-242">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7f4e6-242">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="7f4e6-243">Registros de chamadas</span><span class="sxs-lookup"><span data-stu-id="7f4e6-243">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="7f4e6-244">Mensagem de chat</span><span class="sxs-lookup"><span data-stu-id="7f4e6-244">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="7f4e6-245">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="7f4e6-245">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="7f4e6-246">Contatos</span><span class="sxs-lookup"><span data-stu-id="7f4e6-246">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="7f4e6-247">Conversas</span><span class="sxs-lookup"><span data-stu-id="7f4e6-247">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="7f4e6-248">Unidades</span><span class="sxs-lookup"><span data-stu-id="7f4e6-248">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="7f4e6-249">Eventos</span><span class="sxs-lookup"><span data-stu-id="7f4e6-249">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="7f4e6-250">Grupos</span><span class="sxs-lookup"><span data-stu-id="7f4e6-250">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="7f4e6-251">Lista</span><span class="sxs-lookup"><span data-stu-id="7f4e6-251">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="7f4e6-252">Email</span><span class="sxs-lookup"><span data-stu-id="7f4e6-252">Mail</span></span>](../resources/message.md)|<span data-ttu-id="7f4e6-253">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="7f4e6-253">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="7f4e6-254">Presença</span><span class="sxs-lookup"><span data-stu-id="7f4e6-254">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="7f4e6-255">`/communications/presences/{id}` (usuário único), `/communications/presences?$filter=id in ({id},{id}…)` (vários usuários)</span><span class="sxs-lookup"><span data-stu-id="7f4e6-255">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|[<span data-ttu-id="7f4e6-256">impressora</span><span class="sxs-lookup"><span data-stu-id="7f4e6-256">printer</span></span>](../resources/printer.md) |`print/printers/{id}/jobs`|
|[<span data-ttu-id="7f4e6-257">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="7f4e6-257">PrintTaskDefinition</span></span>](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[<span data-ttu-id="7f4e6-258">Usuários</span><span class="sxs-lookup"><span data-stu-id="7f4e6-258">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="7f4e6-259">todoTask</span><span class="sxs-lookup"><span data-stu-id="7f4e6-259">todoTask</span></span>](../resources/todotask.md) | `/me/todo/lists/{todoTaskListId}/tasks`
|[<span data-ttu-id="7f4e6-260">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="7f4e6-260">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> <span data-ttu-id="7f4e6-261">**Observação:** qualquer caminho iniciado por `me` também pode ser usado com `users/{id}` em vez de `me` para direcionar um usuário específico, em vez de usar o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-261">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="7f4e6-262">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f4e6-262">Response</span></span>

<span data-ttu-id="7f4e6-263">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-263">The following example shows the response.</span></span> 

><span data-ttu-id="7f4e6-264">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-264">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="notification-endpoint-validation"></a><span data-ttu-id="7f4e6-265">Validação de ponto de extremidade da notificação</span><span class="sxs-lookup"><span data-stu-id="7f4e6-265">Notification endpoint validation</span></span>

<span data-ttu-id="7f4e6-266">O ponto de extremidade de notificação de assinatura (especificado na propriedade **notificationUrl)** deve ser capaz de responder a uma solicitação de validação conforme descrito em [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="7f4e6-266">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="7f4e6-267">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="7f4e6-267">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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


