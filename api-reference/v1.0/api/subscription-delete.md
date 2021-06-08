---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 53d835062f004c3f3e98c040eb207f4d22574a49
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787109"
---
# <a name="delete-subscription"></a><span data-ttu-id="95e5d-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="95e5d-103">Delete subscription</span></span>

<span data-ttu-id="95e5d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95e5d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95e5d-105">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="95e5d-105">Delete a subscription.</span></span>

<span data-ttu-id="95e5d-106">Consulte a tabela na seção [Permissões](#permissions) para obter a lista de recursos que oferecem suporte à inscrição para alterar notificações.</span><span class="sxs-lookup"><span data-stu-id="95e5d-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="95e5d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="95e5d-107">Permissions</span></span>

<span data-ttu-id="95e5d-108">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="95e5d-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="95e5d-109">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95e5d-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="95e5d-110">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="95e5d-110">Supported resource</span></span> | <span data-ttu-id="95e5d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95e5d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="95e5d-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95e5d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95e5d-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95e5d-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="95e5d-114">callRecord</span><span class="sxs-lookup"><span data-stu-id="95e5d-114">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="95e5d-115">Incompatível</span><span class="sxs-lookup"><span data-stu-id="95e5d-115">Not supported</span></span> | <span data-ttu-id="95e5d-116">Incompatível</span><span class="sxs-lookup"><span data-stu-id="95e5d-116">Not supported</span></span> | <span data-ttu-id="95e5d-117">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="95e5d-117">CallRecords.Read.All</span></span> |
|<span data-ttu-id="95e5d-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="95e5d-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="95e5d-119">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="95e5d-119">ChannelMessage.Read.All</span></span> | <span data-ttu-id="95e5d-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95e5d-120">Not supported</span></span> |  <span data-ttu-id="95e5d-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="95e5d-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="95e5d-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="95e5d-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="95e5d-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95e5d-123">Not supported</span></span> | <span data-ttu-id="95e5d-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95e5d-124">Not supported</span></span> | <span data-ttu-id="95e5d-125">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="95e5d-125">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="95e5d-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="95e5d-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="95e5d-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95e5d-127">Not supported</span></span> | <span data-ttu-id="95e5d-128">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95e5d-128">Not supported</span></span> | <span data-ttu-id="95e5d-129">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="95e5d-129">Chat.Read.All</span></span>  |
|<span data-ttu-id="95e5d-130">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="95e5d-130">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="95e5d-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95e5d-131">Not supported</span></span> | <span data-ttu-id="95e5d-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95e5d-132">Not supported</span></span> | <span data-ttu-id="95e5d-133">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="95e5d-133">Chat.Read.All</span></span>  |
|[<span data-ttu-id="95e5d-134">contato</span><span class="sxs-lookup"><span data-stu-id="95e5d-134">contact</span></span>](../resources/contact.md) | <span data-ttu-id="95e5d-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="95e5d-135">Contacts.Read</span></span> | <span data-ttu-id="95e5d-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="95e5d-136">Contacts.Read</span></span> | <span data-ttu-id="95e5d-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="95e5d-137">Contacts.Read</span></span> |
|<span data-ttu-id="95e5d-138">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="95e5d-138">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="95e5d-139">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95e5d-139">Not supported</span></span> | <span data-ttu-id="95e5d-140">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95e5d-140">Files.ReadWrite</span></span> | <span data-ttu-id="95e5d-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95e5d-141">Not supported</span></span> |
|<span data-ttu-id="95e5d-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="95e5d-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="95e5d-143">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95e5d-143">Files.ReadWrite.All</span></span> | <span data-ttu-id="95e5d-144">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95e5d-144">Not supported</span></span> | <span data-ttu-id="95e5d-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95e5d-145">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="95e5d-146">evento</span><span class="sxs-lookup"><span data-stu-id="95e5d-146">event</span></span>](../resources/event.md) | <span data-ttu-id="95e5d-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="95e5d-147">Calendars.Read</span></span> | <span data-ttu-id="95e5d-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="95e5d-148">Calendars.Read</span></span> | <span data-ttu-id="95e5d-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="95e5d-149">Calendars.Read</span></span> |
|[<span data-ttu-id="95e5d-150">grupo</span><span class="sxs-lookup"><span data-stu-id="95e5d-150">group</span></span>](../resources/group.md) | <span data-ttu-id="95e5d-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="95e5d-151">Group.Read.All</span></span> | <span data-ttu-id="95e5d-152">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95e5d-152">Not supported</span></span> | <span data-ttu-id="95e5d-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="95e5d-153">Group.Read.All</span></span> |
|[<span data-ttu-id="95e5d-154">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="95e5d-154">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="95e5d-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="95e5d-155">Group.Read.All</span></span> | <span data-ttu-id="95e5d-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95e5d-156">Not supported</span></span> | <span data-ttu-id="95e5d-157">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95e5d-157">Not supported</span></span> |
|[<span data-ttu-id="95e5d-158">list</span><span class="sxs-lookup"><span data-stu-id="95e5d-158">list</span></span>](../resources/list.md) | <span data-ttu-id="95e5d-159">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95e5d-159">Sites.ReadWrite.All</span></span> | <span data-ttu-id="95e5d-160">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95e5d-160">Not supported</span></span> | <span data-ttu-id="95e5d-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95e5d-161">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="95e5d-162">message</span><span class="sxs-lookup"><span data-stu-id="95e5d-162">message</span></span>](../resources/message.md) | <span data-ttu-id="95e5d-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="95e5d-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="95e5d-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="95e5d-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="95e5d-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="95e5d-165">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="95e5d-166">printer</span><span class="sxs-lookup"><span data-stu-id="95e5d-166">printer</span></span>](../resources/printer.md) | <span data-ttu-id="95e5d-167">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95e5d-167">Not supported</span></span> | <span data-ttu-id="95e5d-168">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95e5d-168">Not supported</span></span> | <span data-ttu-id="95e5d-169">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95e5d-169">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="95e5d-170">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="95e5d-170">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="95e5d-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95e5d-171">Not supported</span></span> | <span data-ttu-id="95e5d-172">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95e5d-172">Not supported</span></span> | <span data-ttu-id="95e5d-173">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95e5d-173">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="95e5d-174">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="95e5d-174">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="95e5d-175">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95e5d-175">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="95e5d-176">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95e5d-176">Not supported</span></span> | <span data-ttu-id="95e5d-177">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95e5d-177">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="95e5d-178">Usuário</span><span class="sxs-lookup"><span data-stu-id="95e5d-178">user</span></span>](../resources/user.md) | <span data-ttu-id="95e5d-179">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="95e5d-179">User.Read.All</span></span> | <span data-ttu-id="95e5d-180">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="95e5d-180">User.Read.All</span></span> | <span data-ttu-id="95e5d-181">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="95e5d-181">User.Read.All</span></span> |


> <span data-ttu-id="95e5d-182">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="95e5d-182">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="95e5d-183">driveItem</span><span class="sxs-lookup"><span data-stu-id="95e5d-183">driveItem</span></span>

<span data-ttu-id="95e5d-184">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="95e5d-184">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="95e5d-185">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="95e5d-185">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="95e5d-186">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="95e5d-186">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="95e5d-187">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="95e5d-187">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="95e5d-188">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="95e5d-188">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="95e5d-189">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="95e5d-189">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="95e5d-190">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="95e5d-190">contact, event, and message</span></span>

<span data-ttu-id="95e5d-191">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="95e5d-191">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="95e5d-192">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="95e5d-192">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="95e5d-193">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="95e5d-193">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="95e5d-194">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="95e5d-194">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="95e5d-195">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="95e5d-195">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="95e5d-196">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="95e5d-196">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="95e5d-197">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="95e5d-197">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="95e5d-198">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95e5d-198">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="95e5d-199">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95e5d-199">Request headers</span></span>

| <span data-ttu-id="95e5d-200">Nome</span><span class="sxs-lookup"><span data-stu-id="95e5d-200">Name</span></span>       | <span data-ttu-id="95e5d-201">Tipo</span><span class="sxs-lookup"><span data-stu-id="95e5d-201">Type</span></span> | <span data-ttu-id="95e5d-202">Descrição</span><span class="sxs-lookup"><span data-stu-id="95e5d-202">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="95e5d-203">Autorização</span><span class="sxs-lookup"><span data-stu-id="95e5d-203">Authorization</span></span>  | <span data-ttu-id="95e5d-204">string</span><span class="sxs-lookup"><span data-stu-id="95e5d-204">string</span></span>  | <span data-ttu-id="95e5d-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95e5d-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95e5d-207">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95e5d-207">Request body</span></span>

<span data-ttu-id="95e5d-208">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="95e5d-208">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95e5d-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="95e5d-209">Response</span></span>

<span data-ttu-id="95e5d-210">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="95e5d-210">If successful, this method returns a `204 No Content` response code.</span></span>
<span data-ttu-id="95e5d-211">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="95e5d-211">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="95e5d-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95e5d-212">Example</span></span>

##### <a name="request"></a><span data-ttu-id="95e5d-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95e5d-213">Request</span></span>

<span data-ttu-id="95e5d-214">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95e5d-214">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="95e5d-215">HTTP</span><span class="sxs-lookup"><span data-stu-id="95e5d-215">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="95e5d-216">C#</span><span class="sxs-lookup"><span data-stu-id="95e5d-216">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95e5d-217">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95e5d-217">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95e5d-218">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95e5d-218">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="95e5d-219">Java</span><span class="sxs-lookup"><span data-stu-id="95e5d-219">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="95e5d-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="95e5d-220">Response</span></span>

<span data-ttu-id="95e5d-221">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95e5d-221">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

