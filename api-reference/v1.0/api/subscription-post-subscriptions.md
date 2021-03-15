---
title: Criar assinatura
description: Inscreve um aplicativo de ouvinte para receber notificações de alterações quando os dados no Microsoft Graph forem alterados.
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: fb6f04b020fd925d1131f2d8f88afe44b185c5c7
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761427"
---
# <a name="create-subscription"></a><span data-ttu-id="eef34-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="eef34-103">Create subscription</span></span>

<span data-ttu-id="eef34-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eef34-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eef34-105">Inscreve um aplicativo de ouvinte para receber notificações de alterações quando o tipo de alteração solicitado ocorrer no recurso especificado no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="eef34-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

<span data-ttu-id="eef34-106">Consulte a tabela na seção [Permissões](#permissions) para obter a lista de recursos que oferecem suporte à inscrição para alterar notificações.</span><span class="sxs-lookup"><span data-stu-id="eef34-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="eef34-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="eef34-107">Permissions</span></span>

<span data-ttu-id="eef34-108">Criar uma assinatura exige o escopo de leitura do recurso.</span><span class="sxs-lookup"><span data-stu-id="eef34-108">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="eef34-109">Por exemplo, para receber notificações de alterações por mensagens, seu aplicativo precisa da permissão`Mail.Read`.</span><span class="sxs-lookup"><span data-stu-id="eef34-109">For example, to get change notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
<span data-ttu-id="eef34-110">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="eef34-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="eef34-111">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eef34-111">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eef34-112">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="eef34-112">Supported resource</span></span> | <span data-ttu-id="eef34-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eef34-113">Delegated (work or school account)</span></span> | <span data-ttu-id="eef34-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eef34-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eef34-115">Application</span><span class="sxs-lookup"><span data-stu-id="eef34-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="eef34-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="eef34-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="eef34-117">Incompatível</span><span class="sxs-lookup"><span data-stu-id="eef34-117">Not supported</span></span> | <span data-ttu-id="eef34-118">Incompatível</span><span class="sxs-lookup"><span data-stu-id="eef34-118">Not supported</span></span> | <span data-ttu-id="eef34-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="eef34-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="eef34-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="eef34-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="eef34-121">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="eef34-121">ChannelMessage.Read.All</span></span> | <span data-ttu-id="eef34-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="eef34-122">Not supported</span></span> |  <span data-ttu-id="eef34-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="eef34-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="eef34-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="eef34-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="eef34-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="eef34-125">Not supported</span></span> | <span data-ttu-id="eef34-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="eef34-126">Not supported</span></span> | <span data-ttu-id="eef34-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="eef34-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="eef34-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="eef34-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="eef34-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="eef34-129">Not supported</span></span> | <span data-ttu-id="eef34-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="eef34-130">Not supported</span></span> | <span data-ttu-id="eef34-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="eef34-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="eef34-132">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="eef34-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="eef34-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="eef34-133">Not supported</span></span> | <span data-ttu-id="eef34-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="eef34-134">Not supported</span></span> | <span data-ttu-id="eef34-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="eef34-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="eef34-136">contato</span><span class="sxs-lookup"><span data-stu-id="eef34-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="eef34-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="eef34-137">Contacts.Read</span></span> | <span data-ttu-id="eef34-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="eef34-138">Contacts.Read</span></span> | <span data-ttu-id="eef34-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="eef34-139">Contacts.Read</span></span> |
|<span data-ttu-id="eef34-140">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="eef34-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="eef34-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="eef34-141">Not supported</span></span> | <span data-ttu-id="eef34-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eef34-142">Files.ReadWrite</span></span> | <span data-ttu-id="eef34-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="eef34-143">Not supported</span></span> |
|<span data-ttu-id="eef34-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="eef34-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="eef34-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eef34-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="eef34-146">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="eef34-146">Not supported</span></span> | <span data-ttu-id="eef34-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eef34-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="eef34-148">evento</span><span class="sxs-lookup"><span data-stu-id="eef34-148">event</span></span>](../resources/event.md) | <span data-ttu-id="eef34-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="eef34-149">Calendars.Read</span></span> | <span data-ttu-id="eef34-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="eef34-150">Calendars.Read</span></span> | <span data-ttu-id="eef34-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="eef34-151">Calendars.Read</span></span> |
|[<span data-ttu-id="eef34-152">grupo</span><span class="sxs-lookup"><span data-stu-id="eef34-152">group</span></span>](../resources/group.md) | <span data-ttu-id="eef34-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="eef34-153">Group.Read.All</span></span> | <span data-ttu-id="eef34-154">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="eef34-154">Not supported</span></span> | <span data-ttu-id="eef34-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="eef34-155">Group.Read.All</span></span> |
|[<span data-ttu-id="eef34-156">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="eef34-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="eef34-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="eef34-157">Group.Read.All</span></span> | <span data-ttu-id="eef34-158">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="eef34-158">Not supported</span></span> | <span data-ttu-id="eef34-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="eef34-159">Not supported</span></span> |
|[<span data-ttu-id="eef34-160">list</span><span class="sxs-lookup"><span data-stu-id="eef34-160">list</span></span>](../resources/list.md) | <span data-ttu-id="eef34-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eef34-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="eef34-162">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="eef34-162">Not supported</span></span> | <span data-ttu-id="eef34-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eef34-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="eef34-164">message</span><span class="sxs-lookup"><span data-stu-id="eef34-164">message</span></span>](../resources/message.md) | <span data-ttu-id="eef34-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="eef34-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="eef34-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="eef34-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="eef34-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="eef34-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="eef34-168">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="eef34-168">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="eef34-169">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eef34-169">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="eef34-170">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="eef34-170">Not supported</span></span> | <span data-ttu-id="eef34-171">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eef34-171">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="eef34-172">Usuário</span><span class="sxs-lookup"><span data-stu-id="eef34-172">user</span></span>](../resources/user.md) | <span data-ttu-id="eef34-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="eef34-173">User.Read.All</span></span> | <span data-ttu-id="eef34-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="eef34-174">User.Read.All</span></span> | <span data-ttu-id="eef34-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="eef34-175">User.Read.All</span></span> |

> <span data-ttu-id="eef34-176">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="eef34-176">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="eef34-177">driveItem</span><span class="sxs-lookup"><span data-stu-id="eef34-177">driveItem</span></span>

<span data-ttu-id="eef34-178">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="eef34-178">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="eef34-179">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="eef34-179">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="eef34-180">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="eef34-180">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="eef34-181">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="eef34-181">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="eef34-182">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="eef34-182">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="eef34-183">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="eef34-183">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="eef34-184">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="eef34-184">contact, event, and message</span></span>

<span data-ttu-id="eef34-185">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="eef34-185">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="eef34-186">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="eef34-186">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="eef34-187">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="eef34-187">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="eef34-188">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="eef34-188">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="eef34-189">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="eef34-189">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="eef34-190">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="eef34-190">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="eef34-191">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="eef34-191">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="eef34-192">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eef34-192">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="eef34-193">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eef34-193">Request headers</span></span>

| <span data-ttu-id="eef34-194">Nome</span><span class="sxs-lookup"><span data-stu-id="eef34-194">Name</span></span>       | <span data-ttu-id="eef34-195">Tipo</span><span class="sxs-lookup"><span data-stu-id="eef34-195">Type</span></span> | <span data-ttu-id="eef34-196">Descrição</span><span class="sxs-lookup"><span data-stu-id="eef34-196">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="eef34-197">Autorização</span><span class="sxs-lookup"><span data-stu-id="eef34-197">Authorization</span></span>  | <span data-ttu-id="eef34-198">string</span><span class="sxs-lookup"><span data-stu-id="eef34-198">string</span></span>  | <span data-ttu-id="eef34-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eef34-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="eef34-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="eef34-201">Response</span></span>

<span data-ttu-id="eef34-202">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eef34-202">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>
<span data-ttu-id="eef34-203">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="eef34-203">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="eef34-204">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eef34-204">Example</span></span>

##### <a name="request"></a><span data-ttu-id="eef34-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eef34-205">Request</span></span>

<span data-ttu-id="eef34-206">Veja a seguir um exemplo da solicitação de envio de uma notificação quando o usuário receber um novo email.</span><span class="sxs-lookup"><span data-stu-id="eef34-206">Here is an example of the request to send a change notification when the user receives a new mail.</span></span>

# <a name="http"></a>[<span data-ttu-id="eef34-207">HTTP</span><span class="sxs-lookup"><span data-stu-id="eef34-207">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
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
# <a name="c"></a>[<span data-ttu-id="eef34-208">C#</span><span class="sxs-lookup"><span data-stu-id="eef34-208">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eef34-209">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eef34-209">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eef34-210">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eef34-210">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eef34-211">Java</span><span class="sxs-lookup"><span data-stu-id="eef34-211">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="eef34-212">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="eef34-212">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="eef34-213">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="eef34-213">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="eef34-214">Exemplos de recursos</span><span class="sxs-lookup"><span data-stu-id="eef34-214">Resources examples</span></span>

<span data-ttu-id="eef34-215">Estes são os valores válidos da propriedade de recurso da assinatura:</span><span class="sxs-lookup"><span data-stu-id="eef34-215">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="eef34-216">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="eef34-216">Resource type</span></span> | <span data-ttu-id="eef34-217">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eef34-217">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="eef34-218">Registros de chamadas</span><span class="sxs-lookup"><span data-stu-id="eef34-218">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="eef34-219">Mensagem de chat</span><span class="sxs-lookup"><span data-stu-id="eef34-219">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="eef34-220">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="eef34-220">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="eef34-221">Contatos</span><span class="sxs-lookup"><span data-stu-id="eef34-221">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="eef34-222">Conversas</span><span class="sxs-lookup"><span data-stu-id="eef34-222">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="eef34-223">Unidades</span><span class="sxs-lookup"><span data-stu-id="eef34-223">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="eef34-224">Eventos</span><span class="sxs-lookup"><span data-stu-id="eef34-224">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="eef34-225">Grupos</span><span class="sxs-lookup"><span data-stu-id="eef34-225">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="eef34-226">Lista</span><span class="sxs-lookup"><span data-stu-id="eef34-226">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="eef34-227">Email</span><span class="sxs-lookup"><span data-stu-id="eef34-227">Mail</span></span>](../resources/message.md)|<span data-ttu-id="eef34-228">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="eef34-228">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="eef34-229">Usuários</span><span class="sxs-lookup"><span data-stu-id="eef34-229">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="eef34-230">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="eef34-230">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'New'`|

> <span data-ttu-id="eef34-231">**Observação:** qualquer caminho iniciado por `me` também pode ser usado com `users/{id}` em vez de `me` para direcionar um usuário específico, em vez de usar o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="eef34-231">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

##### <a name="response"></a><span data-ttu-id="eef34-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="eef34-232">Response</span></span>

<span data-ttu-id="eef34-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eef34-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="eef34-236">Validação de ponto de extremidade da notificação</span><span class="sxs-lookup"><span data-stu-id="eef34-236">Notification endpoint validation</span></span>

<span data-ttu-id="eef34-237">O ponto de extremidade da notificação da assinatura (especificado na `notificationUrl` propriedade) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [Configurar notificações para alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="eef34-237">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="eef34-238">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="eef34-238">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

[error-response]: /graph/errors

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

