---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: c2f5e7aa89b68c911e79b5d2a9909d398d3f58b6
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034169"
---
# <a name="update-subscription"></a><span data-ttu-id="e04bb-103">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="e04bb-103">Update subscription</span></span>

<span data-ttu-id="e04bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e04bb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e04bb-105">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="e04bb-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="e04bb-106">As assinaturas expiram após um período que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="e04bb-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="e04bb-107">Para evitar notificações de alteração ausentes, um aplicativo deve renovar suas assinaturas bem antes de sua data de vencimento.</span><span class="sxs-lookup"><span data-stu-id="e04bb-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="e04bb-108">Consulte [a assinatura](../resources/subscription.md) para a duração máxima de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="e04bb-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="e04bb-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="e04bb-109">Permissions</span></span>

<span data-ttu-id="e04bb-110">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="e04bb-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="e04bb-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e04bb-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e04bb-112">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="e04bb-112">Supported resource</span></span> | <span data-ttu-id="e04bb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e04bb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e04bb-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e04bb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e04bb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e04bb-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="e04bb-116">callRecord</span><span class="sxs-lookup"><span data-stu-id="e04bb-116">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="e04bb-117">Incompatível</span><span class="sxs-lookup"><span data-stu-id="e04bb-117">Not supported</span></span> | <span data-ttu-id="e04bb-118">Incompatível</span><span class="sxs-lookup"><span data-stu-id="e04bb-118">Not supported</span></span> | <span data-ttu-id="e04bb-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="e04bb-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="e04bb-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="e04bb-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="e04bb-121">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e04bb-121">Not supported</span></span> | <span data-ttu-id="e04bb-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e04bb-122">Not supported</span></span> |  <span data-ttu-id="e04bb-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="e04bb-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="e04bb-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="e04bb-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="e04bb-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e04bb-125">Not supported</span></span> | <span data-ttu-id="e04bb-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e04bb-126">Not supported</span></span> | <span data-ttu-id="e04bb-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="e04bb-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="e04bb-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="e04bb-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="e04bb-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e04bb-129">Not supported</span></span> | <span data-ttu-id="e04bb-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e04bb-130">Not supported</span></span> | <span data-ttu-id="e04bb-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="e04bb-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="e04bb-132">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="e04bb-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="e04bb-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e04bb-133">Not supported</span></span> | <span data-ttu-id="e04bb-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e04bb-134">Not supported</span></span> | <span data-ttu-id="e04bb-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="e04bb-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="e04bb-136">contato</span><span class="sxs-lookup"><span data-stu-id="e04bb-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="e04bb-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e04bb-137">Contacts.Read</span></span> | <span data-ttu-id="e04bb-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e04bb-138">Contacts.Read</span></span> | <span data-ttu-id="e04bb-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e04bb-139">Contacts.Read</span></span> |
|<span data-ttu-id="e04bb-140">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="e04bb-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="e04bb-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e04bb-141">Not supported</span></span> | <span data-ttu-id="e04bb-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e04bb-142">Files.ReadWrite</span></span> | <span data-ttu-id="e04bb-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e04bb-143">Not supported</span></span> |
|<span data-ttu-id="e04bb-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="e04bb-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="e04bb-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e04bb-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="e04bb-146">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e04bb-146">Not supported</span></span> | <span data-ttu-id="e04bb-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e04bb-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="e04bb-148">evento</span><span class="sxs-lookup"><span data-stu-id="e04bb-148">event</span></span>](../resources/event.md) | <span data-ttu-id="e04bb-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e04bb-149">Calendars.Read</span></span> | <span data-ttu-id="e04bb-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e04bb-150">Calendars.Read</span></span> | <span data-ttu-id="e04bb-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e04bb-151">Calendars.Read</span></span> |
|[<span data-ttu-id="e04bb-152">grupo</span><span class="sxs-lookup"><span data-stu-id="e04bb-152">group</span></span>](../resources/group.md) | <span data-ttu-id="e04bb-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e04bb-153">Group.Read.All</span></span> | <span data-ttu-id="e04bb-154">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e04bb-154">Not supported</span></span> | <span data-ttu-id="e04bb-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e04bb-155">Group.Read.All</span></span> |
|[<span data-ttu-id="e04bb-156">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="e04bb-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="e04bb-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e04bb-157">Group.Read.All</span></span> | <span data-ttu-id="e04bb-158">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e04bb-158">Not supported</span></span> | <span data-ttu-id="e04bb-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e04bb-159">Not supported</span></span> |
|[<span data-ttu-id="e04bb-160">list</span><span class="sxs-lookup"><span data-stu-id="e04bb-160">list</span></span>](../resources/list.md) | <span data-ttu-id="e04bb-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e04bb-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="e04bb-162">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e04bb-162">Not supported</span></span> | <span data-ttu-id="e04bb-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e04bb-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="e04bb-164">message</span><span class="sxs-lookup"><span data-stu-id="e04bb-164">message</span></span>](../resources/message.md) | <span data-ttu-id="e04bb-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e04bb-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="e04bb-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e04bb-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="e04bb-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e04bb-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="e04bb-168">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="e04bb-168">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="e04bb-169">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e04bb-169">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="e04bb-170">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e04bb-170">Not supported</span></span> | <span data-ttu-id="e04bb-171">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e04bb-171">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="e04bb-172">Usuário</span><span class="sxs-lookup"><span data-stu-id="e04bb-172">user</span></span>](../resources/user.md) | <span data-ttu-id="e04bb-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e04bb-173">User.Read.All</span></span> | <span data-ttu-id="e04bb-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e04bb-174">User.Read.All</span></span> | <span data-ttu-id="e04bb-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e04bb-175">User.Read.All</span></span> |

> <span data-ttu-id="e04bb-176">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="e04bb-176">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [beta-disclaimer](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="e04bb-177">driveItem</span><span class="sxs-lookup"><span data-stu-id="e04bb-177">driveItem</span></span>

<span data-ttu-id="e04bb-178">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e04bb-178">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="e04bb-179">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="e04bb-179">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="e04bb-180">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="e04bb-180">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="e04bb-181">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="e04bb-181">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="e04bb-182">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="e04bb-182">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="e04bb-183">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="e04bb-183">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="e04bb-184">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="e04bb-184">contact, event, and message</span></span>

<span data-ttu-id="e04bb-185">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="e04bb-185">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="e04bb-186">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="e04bb-186">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="e04bb-187">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="e04bb-187">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="e04bb-188">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="e04bb-188">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="e04bb-189">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="e04bb-189">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="e04bb-190">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="e04bb-190">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="e04bb-191">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="e04bb-191">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="e04bb-192">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e04bb-192">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e04bb-193">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e04bb-193">Request headers</span></span>

| <span data-ttu-id="e04bb-194">Nome</span><span class="sxs-lookup"><span data-stu-id="e04bb-194">Name</span></span>       | <span data-ttu-id="e04bb-195">Tipo</span><span class="sxs-lookup"><span data-stu-id="e04bb-195">Type</span></span> | <span data-ttu-id="e04bb-196">Descrição</span><span class="sxs-lookup"><span data-stu-id="e04bb-196">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e04bb-197">Autorização</span><span class="sxs-lookup"><span data-stu-id="e04bb-197">Authorization</span></span>  | <span data-ttu-id="e04bb-198">string</span><span class="sxs-lookup"><span data-stu-id="e04bb-198">string</span></span>  | <span data-ttu-id="e04bb-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e04bb-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e04bb-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="e04bb-201">Response</span></span>

<span data-ttu-id="e04bb-202">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e04bb-202">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="e04bb-203">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="e04bb-203">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="e04bb-204">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e04bb-204">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e04bb-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e04bb-205">Request</span></span>

<span data-ttu-id="e04bb-206">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e04bb-206">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e04bb-207">HTTP</span><span class="sxs-lookup"><span data-stu-id="e04bb-207">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```
# <a name="c"></a>[<span data-ttu-id="e04bb-208">C#</span><span class="sxs-lookup"><span data-stu-id="e04bb-208">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e04bb-209">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e04bb-209">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e04bb-210">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e04bb-210">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e04bb-211">Java</span><span class="sxs-lookup"><span data-stu-id="e04bb-211">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e04bb-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="e04bb-212">Response</span></span>

<span data-ttu-id="e04bb-213">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e04bb-213">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
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
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2",
  "encryptionCertificate": "",
  "encryptionCertificateId": "",
  "includeResourceData": false
}
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

