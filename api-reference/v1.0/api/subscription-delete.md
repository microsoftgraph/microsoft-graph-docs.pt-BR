---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 32a955571e0aca1eabfe899e716d658443db363b
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848195"
---
# <a name="delete-subscription"></a><span data-ttu-id="9208e-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="9208e-103">Delete subscription</span></span>

<span data-ttu-id="9208e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9208e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9208e-105">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="9208e-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="9208e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9208e-106">Permissions</span></span>

<span data-ttu-id="9208e-107">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="9208e-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="9208e-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9208e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9208e-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="9208e-109">Supported resource</span></span> | <span data-ttu-id="9208e-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9208e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9208e-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9208e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9208e-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9208e-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="9208e-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="9208e-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="9208e-114">Incompatível</span><span class="sxs-lookup"><span data-stu-id="9208e-114">Not supported</span></span> | <span data-ttu-id="9208e-115">Incompatível</span><span class="sxs-lookup"><span data-stu-id="9208e-115">Not supported</span></span> | <span data-ttu-id="9208e-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="9208e-116">CallRecords.Read.All</span></span> |
|<span data-ttu-id="9208e-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="9208e-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="9208e-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9208e-118">Not supported</span></span> | <span data-ttu-id="9208e-119">Incompatível</span><span class="sxs-lookup"><span data-stu-id="9208e-119">Not supported</span></span> |  <span data-ttu-id="9208e-120">ChannelMessage. Read. Group \*, ChannelMessage. Read. All</span><span class="sxs-lookup"><span data-stu-id="9208e-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="9208e-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="9208e-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="9208e-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9208e-122">Not supported</span></span> | <span data-ttu-id="9208e-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9208e-123">Not supported</span></span> | <span data-ttu-id="9208e-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="9208e-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="9208e-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="9208e-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="9208e-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9208e-126">Not supported</span></span> | <span data-ttu-id="9208e-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9208e-127">Not supported</span></span> | <span data-ttu-id="9208e-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="9208e-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="9208e-129">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="9208e-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="9208e-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9208e-130">Not supported</span></span> | <span data-ttu-id="9208e-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9208e-131">Not supported</span></span> | <span data-ttu-id="9208e-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="9208e-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="9208e-133">contato</span><span class="sxs-lookup"><span data-stu-id="9208e-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="9208e-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9208e-134">Contacts.Read</span></span> | <span data-ttu-id="9208e-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9208e-135">Contacts.Read</span></span> | <span data-ttu-id="9208e-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9208e-136">Contacts.Read</span></span> |
|<span data-ttu-id="9208e-137">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="9208e-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="9208e-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9208e-138">Not supported</span></span> | <span data-ttu-id="9208e-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9208e-139">Files.ReadWrite</span></span> | <span data-ttu-id="9208e-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9208e-140">Not supported</span></span> |
|<span data-ttu-id="9208e-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="9208e-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="9208e-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9208e-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="9208e-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9208e-143">Not supported</span></span> | <span data-ttu-id="9208e-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9208e-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="9208e-145">evento</span><span class="sxs-lookup"><span data-stu-id="9208e-145">event</span></span>](../resources/event.md) | <span data-ttu-id="9208e-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9208e-146">Calendars.Read</span></span> | <span data-ttu-id="9208e-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9208e-147">Calendars.Read</span></span> | <span data-ttu-id="9208e-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9208e-148">Calendars.Read</span></span> |
|[<span data-ttu-id="9208e-149">grupo</span><span class="sxs-lookup"><span data-stu-id="9208e-149">group</span></span>](../resources/group.md) | <span data-ttu-id="9208e-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9208e-150">Group.Read.All</span></span> | <span data-ttu-id="9208e-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9208e-151">Not supported</span></span> | <span data-ttu-id="9208e-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9208e-152">Group.Read.All</span></span> |
|[<span data-ttu-id="9208e-153">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="9208e-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="9208e-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9208e-154">Group.Read.All</span></span> | <span data-ttu-id="9208e-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9208e-155">Not supported</span></span> | <span data-ttu-id="9208e-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9208e-156">Not supported</span></span> |
|[<span data-ttu-id="9208e-157">list</span><span class="sxs-lookup"><span data-stu-id="9208e-157">list</span></span>](../resources/list.md) | <span data-ttu-id="9208e-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9208e-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="9208e-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9208e-159">Not supported</span></span> | <span data-ttu-id="9208e-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9208e-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="9208e-161">message</span><span class="sxs-lookup"><span data-stu-id="9208e-161">message</span></span>](../resources/message.md) | <span data-ttu-id="9208e-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9208e-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="9208e-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9208e-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="9208e-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9208e-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="9208e-165">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="9208e-165">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="9208e-166">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9208e-166">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="9208e-167">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9208e-167">Not supported</span></span> | <span data-ttu-id="9208e-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9208e-168">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="9208e-169">Usuário</span><span class="sxs-lookup"><span data-stu-id="9208e-169">user</span></span>](../resources/user.md) | <span data-ttu-id="9208e-170">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9208e-170">User.Read.All</span></span> | <span data-ttu-id="9208e-171">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9208e-171">User.Read.All</span></span> | <span data-ttu-id="9208e-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9208e-172">User.Read.All</span></span> |

> <span data-ttu-id="9208e-173">**Observação** : Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="9208e-173">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="9208e-174">chatMessage</span><span class="sxs-lookup"><span data-stu-id="9208e-174">chatMessage</span></span>

<span data-ttu-id="9208e-175">Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="9208e-175">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="9208e-176">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="9208e-176">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="9208e-177">Antes de criar uma assinatura **chatMessage** , você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="9208e-177">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="9208e-178">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="9208e-178">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="9208e-179">**Observação:** `/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para os usuários que têm as [licenças necessárias](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="9208e-179">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="9208e-180">driveItem</span><span class="sxs-lookup"><span data-stu-id="9208e-180">driveItem</span></span>

<span data-ttu-id="9208e-181">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9208e-181">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="9208e-182">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="9208e-182">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="9208e-183">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="9208e-183">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="9208e-184">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="9208e-184">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="9208e-185">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="9208e-185">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="9208e-186">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="9208e-186">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="9208e-187">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="9208e-187">contact, event, and message</span></span>

<span data-ttu-id="9208e-188">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="9208e-188">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="9208e-189">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="9208e-189">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="9208e-190">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="9208e-190">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="9208e-191">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="9208e-191">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="9208e-192">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_ :</span><span class="sxs-lookup"><span data-stu-id="9208e-192">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="9208e-193">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="9208e-193">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="9208e-194">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="9208e-194">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="9208e-195">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9208e-195">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="9208e-196">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9208e-196">Request headers</span></span>

| <span data-ttu-id="9208e-197">Nome</span><span class="sxs-lookup"><span data-stu-id="9208e-197">Name</span></span>       | <span data-ttu-id="9208e-198">Tipo</span><span class="sxs-lookup"><span data-stu-id="9208e-198">Type</span></span> | <span data-ttu-id="9208e-199">Descrição</span><span class="sxs-lookup"><span data-stu-id="9208e-199">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9208e-200">Autorização</span><span class="sxs-lookup"><span data-stu-id="9208e-200">Authorization</span></span>  | <span data-ttu-id="9208e-201">string</span><span class="sxs-lookup"><span data-stu-id="9208e-201">string</span></span>  | <span data-ttu-id="9208e-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9208e-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9208e-204">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9208e-204">Request body</span></span>

<span data-ttu-id="9208e-205">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9208e-205">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9208e-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="9208e-206">Response</span></span>

<span data-ttu-id="9208e-207">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9208e-207">If successful, this method returns a `204 No Content` response code.</span></span>
<span data-ttu-id="9208e-208">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="9208e-208">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="9208e-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9208e-209">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9208e-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9208e-210">Request</span></span>

<span data-ttu-id="9208e-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9208e-211">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9208e-212">HTTP</span><span class="sxs-lookup"><span data-stu-id="9208e-212">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="9208e-213">C#</span><span class="sxs-lookup"><span data-stu-id="9208e-213">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9208e-214">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9208e-214">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9208e-215">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9208e-215">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9208e-216">Java</span><span class="sxs-lookup"><span data-stu-id="9208e-216">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9208e-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="9208e-217">Response</span></span>

<span data-ttu-id="9208e-218">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9208e-218">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
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

