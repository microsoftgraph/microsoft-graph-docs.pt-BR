---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: e63f810e6e11d18d2e03fb702a629cee74d768fe
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759500"
---
# <a name="update-subscription"></a><span data-ttu-id="e767a-103">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="e767a-103">Update subscription</span></span>

<span data-ttu-id="e767a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e767a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e767a-105">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="e767a-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="e767a-106">A tabela na seção [Permissões](#permissions) lista os recursos que suportam a assinatura para alterar notificações.</span><span class="sxs-lookup"><span data-stu-id="e767a-106">The table in the [Permissions](#permissions) section lists the resources that support subscribing to change notifications.</span></span>

<span data-ttu-id="e767a-107">As assinaturas expiram após um período de tempo que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="e767a-107">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="e767a-108">Para evitar notificações de alteração ausentes, um aplicativo deve renovar suas assinaturas bem antes da data de expiração.</span><span class="sxs-lookup"><span data-stu-id="e767a-108">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="e767a-109">Consulte [assinatura](../resources/subscription.md) para o tamanho máximo de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="e767a-109">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="e767a-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="e767a-110">Permissions</span></span>

<span data-ttu-id="e767a-111">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="e767a-111">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="e767a-112">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e767a-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e767a-113">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="e767a-113">Supported resource</span></span> | <span data-ttu-id="e767a-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e767a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e767a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e767a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e767a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e767a-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="e767a-117">callRecord</span><span class="sxs-lookup"><span data-stu-id="e767a-117">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="e767a-118">Incompatível</span><span class="sxs-lookup"><span data-stu-id="e767a-118">Not supported</span></span> | <span data-ttu-id="e767a-119">Incompatível</span><span class="sxs-lookup"><span data-stu-id="e767a-119">Not supported</span></span> | <span data-ttu-id="e767a-120">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="e767a-120">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="e767a-121">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="e767a-121">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="e767a-122">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="e767a-122">ChannelMessage.Read.All</span></span> | <span data-ttu-id="e767a-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e767a-123">Not supported</span></span> |  <span data-ttu-id="e767a-124">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="e767a-124">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="e767a-125">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="e767a-125">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="e767a-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e767a-126">Not supported</span></span> | <span data-ttu-id="e767a-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e767a-127">Not supported</span></span> | <span data-ttu-id="e767a-128">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="e767a-128">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="e767a-129">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="e767a-129">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="e767a-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e767a-130">Not supported</span></span> | <span data-ttu-id="e767a-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e767a-131">Not supported</span></span> | <span data-ttu-id="e767a-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="e767a-132">Chat.Read.All</span></span>  |
|<span data-ttu-id="e767a-133">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="e767a-133">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="e767a-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e767a-134">Not supported</span></span> | <span data-ttu-id="e767a-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e767a-135">Not supported</span></span> | <span data-ttu-id="e767a-136">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="e767a-136">Chat.Read.All</span></span>  |
|[<span data-ttu-id="e767a-137">contato</span><span class="sxs-lookup"><span data-stu-id="e767a-137">contact</span></span>](../resources/contact.md) | <span data-ttu-id="e767a-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e767a-138">Contacts.Read</span></span> | <span data-ttu-id="e767a-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e767a-139">Contacts.Read</span></span> | <span data-ttu-id="e767a-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e767a-140">Contacts.Read</span></span> |
|<span data-ttu-id="e767a-141">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="e767a-141">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="e767a-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e767a-142">Not supported</span></span> | <span data-ttu-id="e767a-143">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e767a-143">Files.ReadWrite</span></span> | <span data-ttu-id="e767a-144">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e767a-144">Not supported</span></span> |
|<span data-ttu-id="e767a-145">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="e767a-145">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="e767a-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e767a-146">Files.ReadWrite.All</span></span> | <span data-ttu-id="e767a-147">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e767a-147">Not supported</span></span> | <span data-ttu-id="e767a-148">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e767a-148">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="e767a-149">evento</span><span class="sxs-lookup"><span data-stu-id="e767a-149">event</span></span>](../resources/event.md) | <span data-ttu-id="e767a-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e767a-150">Calendars.Read</span></span> | <span data-ttu-id="e767a-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e767a-151">Calendars.Read</span></span> | <span data-ttu-id="e767a-152">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e767a-152">Calendars.Read</span></span> |
|[<span data-ttu-id="e767a-153">grupo</span><span class="sxs-lookup"><span data-stu-id="e767a-153">group</span></span>](../resources/group.md) | <span data-ttu-id="e767a-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e767a-154">Group.Read.All</span></span> | <span data-ttu-id="e767a-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e767a-155">Not supported</span></span> | <span data-ttu-id="e767a-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e767a-156">Group.Read.All</span></span> |
|[<span data-ttu-id="e767a-157">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="e767a-157">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="e767a-158">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e767a-158">Group.Read.All</span></span> | <span data-ttu-id="e767a-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e767a-159">Not supported</span></span> | <span data-ttu-id="e767a-160">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e767a-160">Not supported</span></span> |
|[<span data-ttu-id="e767a-161">list</span><span class="sxs-lookup"><span data-stu-id="e767a-161">list</span></span>](../resources/list.md) | <span data-ttu-id="e767a-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e767a-162">Sites.ReadWrite.All</span></span> | <span data-ttu-id="e767a-163">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e767a-163">Not supported</span></span> | <span data-ttu-id="e767a-164">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e767a-164">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="e767a-165">message</span><span class="sxs-lookup"><span data-stu-id="e767a-165">message</span></span>](../resources/message.md) | <span data-ttu-id="e767a-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e767a-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="e767a-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e767a-167">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="e767a-168">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e767a-168">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="e767a-169">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="e767a-169">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="e767a-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e767a-170">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="e767a-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e767a-171">Not supported</span></span> | <span data-ttu-id="e767a-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e767a-172">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="e767a-173">Usuário</span><span class="sxs-lookup"><span data-stu-id="e767a-173">user</span></span>](../resources/user.md) | <span data-ttu-id="e767a-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e767a-174">User.Read.All</span></span> | <span data-ttu-id="e767a-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e767a-175">User.Read.All</span></span> | <span data-ttu-id="e767a-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e767a-176">User.Read.All</span></span> |

> <span data-ttu-id="e767a-177">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="e767a-177">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="e767a-178">driveItem</span><span class="sxs-lookup"><span data-stu-id="e767a-178">driveItem</span></span>

<span data-ttu-id="e767a-179">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e767a-179">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="e767a-180">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="e767a-180">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="e767a-181">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="e767a-181">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="e767a-182">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="e767a-182">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="e767a-183">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="e767a-183">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="e767a-184">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="e767a-184">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="e767a-185">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="e767a-185">contact, event, and message</span></span>

<span data-ttu-id="e767a-186">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="e767a-186">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="e767a-187">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="e767a-187">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="e767a-188">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="e767a-188">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="e767a-189">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="e767a-189">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="e767a-190">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="e767a-190">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="e767a-191">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="e767a-191">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="e767a-192">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="e767a-192">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="e767a-193">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e767a-193">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e767a-194">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e767a-194">Request headers</span></span>

| <span data-ttu-id="e767a-195">Nome</span><span class="sxs-lookup"><span data-stu-id="e767a-195">Name</span></span>       | <span data-ttu-id="e767a-196">Tipo</span><span class="sxs-lookup"><span data-stu-id="e767a-196">Type</span></span> | <span data-ttu-id="e767a-197">Descrição</span><span class="sxs-lookup"><span data-stu-id="e767a-197">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e767a-198">Autorização</span><span class="sxs-lookup"><span data-stu-id="e767a-198">Authorization</span></span>  | <span data-ttu-id="e767a-199">string</span><span class="sxs-lookup"><span data-stu-id="e767a-199">string</span></span>  | <span data-ttu-id="e767a-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e767a-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e767a-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="e767a-202">Response</span></span>

<span data-ttu-id="e767a-203">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e767a-203">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="e767a-204">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="e767a-204">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="e767a-205">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e767a-205">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e767a-206">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e767a-206">Request</span></span>

<span data-ttu-id="e767a-207">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e767a-207">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e767a-208">HTTP</span><span class="sxs-lookup"><span data-stu-id="e767a-208">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e767a-209">C#</span><span class="sxs-lookup"><span data-stu-id="e767a-209">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e767a-210">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e767a-210">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e767a-211">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e767a-211">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e767a-212">Java</span><span class="sxs-lookup"><span data-stu-id="e767a-212">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e767a-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="e767a-213">Response</span></span>

<span data-ttu-id="e767a-214">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e767a-214">Here is an example of the response.</span></span>
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

