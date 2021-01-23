---
title: Obter assinatura
description: Recupere as propriedades e os relacionamentos da uma assinatura.
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 28955a79cd6ce435e10ef73abc3c6e8e5e6f2252
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934888"
---
# <a name="get-subscription"></a><span data-ttu-id="5a568-103">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="5a568-103">Get subscription</span></span>

<span data-ttu-id="5a568-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a568-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a568-105">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="5a568-105">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a568-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a568-106">Permissions</span></span>

<span data-ttu-id="5a568-107">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="5a568-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="5a568-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a568-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a568-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="5a568-109">Supported resource</span></span> | <span data-ttu-id="5a568-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a568-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5a568-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a568-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a568-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a568-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="5a568-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="5a568-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="5a568-114">Incompatível</span><span class="sxs-lookup"><span data-stu-id="5a568-114">Not supported</span></span> | <span data-ttu-id="5a568-115">Incompatível</span><span class="sxs-lookup"><span data-stu-id="5a568-115">Not supported</span></span> | <span data-ttu-id="5a568-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a568-116">CallRecords.Read.All</span></span> |
|<span data-ttu-id="5a568-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="5a568-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="5a568-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a568-118">Not supported</span></span> | <span data-ttu-id="5a568-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a568-119">Not supported</span></span> |  <span data-ttu-id="5a568-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a568-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="5a568-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="5a568-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="5a568-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a568-122">Not supported</span></span> | <span data-ttu-id="5a568-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a568-123">Not supported</span></span> | <span data-ttu-id="5a568-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a568-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="5a568-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="5a568-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="5a568-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a568-126">Not supported</span></span> | <span data-ttu-id="5a568-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a568-127">Not supported</span></span> | <span data-ttu-id="5a568-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a568-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="5a568-129">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="5a568-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="5a568-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a568-130">Not supported</span></span> | <span data-ttu-id="5a568-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a568-131">Not supported</span></span> | <span data-ttu-id="5a568-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a568-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="5a568-133">contato</span><span class="sxs-lookup"><span data-stu-id="5a568-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="5a568-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5a568-134">Contacts.Read</span></span> | <span data-ttu-id="5a568-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5a568-135">Contacts.Read</span></span> | <span data-ttu-id="5a568-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5a568-136">Contacts.Read</span></span> |
|<span data-ttu-id="5a568-137">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="5a568-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="5a568-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a568-138">Not supported</span></span> | <span data-ttu-id="5a568-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a568-139">Files.ReadWrite</span></span> | <span data-ttu-id="5a568-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a568-140">Not supported</span></span> |
|<span data-ttu-id="5a568-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="5a568-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="5a568-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a568-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="5a568-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a568-143">Not supported</span></span> | <span data-ttu-id="5a568-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a568-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="5a568-145">evento</span><span class="sxs-lookup"><span data-stu-id="5a568-145">event</span></span>](../resources/event.md) | <span data-ttu-id="5a568-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5a568-146">Calendars.Read</span></span> | <span data-ttu-id="5a568-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5a568-147">Calendars.Read</span></span> | <span data-ttu-id="5a568-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5a568-148">Calendars.Read</span></span> |
|[<span data-ttu-id="5a568-149">grupo</span><span class="sxs-lookup"><span data-stu-id="5a568-149">group</span></span>](../resources/group.md) | <span data-ttu-id="5a568-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a568-150">Group.Read.All</span></span> | <span data-ttu-id="5a568-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a568-151">Not supported</span></span> | <span data-ttu-id="5a568-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a568-152">Group.Read.All</span></span> |
|[<span data-ttu-id="5a568-153">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="5a568-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="5a568-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a568-154">Group.Read.All</span></span> | <span data-ttu-id="5a568-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a568-155">Not supported</span></span> | <span data-ttu-id="5a568-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a568-156">Not supported</span></span> |
|[<span data-ttu-id="5a568-157">list</span><span class="sxs-lookup"><span data-stu-id="5a568-157">list</span></span>](../resources/list.md) | <span data-ttu-id="5a568-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a568-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="5a568-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a568-159">Not supported</span></span> | <span data-ttu-id="5a568-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a568-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="5a568-161">message</span><span class="sxs-lookup"><span data-stu-id="5a568-161">message</span></span>](../resources/message.md) | <span data-ttu-id="5a568-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5a568-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="5a568-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5a568-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="5a568-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5a568-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="5a568-165">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="5a568-165">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="5a568-166">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a568-166">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="5a568-167">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a568-167">Not supported</span></span> | <span data-ttu-id="5a568-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a568-168">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="5a568-169">Usuário</span><span class="sxs-lookup"><span data-stu-id="5a568-169">user</span></span>](../resources/user.md) | <span data-ttu-id="5a568-170">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a568-170">User.Read.All</span></span> | <span data-ttu-id="5a568-171">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a568-171">User.Read.All</span></span> | <span data-ttu-id="5a568-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a568-172">User.Read.All</span></span> |

> <span data-ttu-id="5a568-173">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="5a568-173">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="5a568-174">chatMessage</span><span class="sxs-lookup"><span data-stu-id="5a568-174">chatMessage</span></span>

<span data-ttu-id="5a568-175">Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="5a568-175">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="5a568-176">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="5a568-176">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="5a568-177">Antes de criar uma assinatura **chatMessage**, você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="5a568-177">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="5a568-178">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="5a568-178">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="5a568-179">**Observação:** `/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para os usuários que têm as [licenças necessárias](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="5a568-179">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>
<span data-ttu-id="5a568-180">No futuro, a Microsoft poderá exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados acessados pela API.</span><span class="sxs-lookup"><span data-stu-id="5a568-180">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem"></a><span data-ttu-id="5a568-181">driveItem</span><span class="sxs-lookup"><span data-stu-id="5a568-181">driveItem</span></span>

<span data-ttu-id="5a568-182">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5a568-182">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="5a568-183">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="5a568-183">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="5a568-184">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="5a568-184">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="5a568-185">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="5a568-185">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="5a568-186">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="5a568-186">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="5a568-187">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="5a568-187">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="5a568-188">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="5a568-188">contact, event, and message</span></span>

<span data-ttu-id="5a568-189">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="5a568-189">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="5a568-190">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="5a568-190">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="5a568-191">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="5a568-191">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="5a568-192">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="5a568-192">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="5a568-193">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="5a568-193">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="5a568-194">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="5a568-194">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="5a568-195">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="5a568-195">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>
 

## <a name="http-request"></a><span data-ttu-id="5a568-196">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a568-196">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5a568-197">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5a568-197">Optional query parameters</span></span>

<span data-ttu-id="5a568-198">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5a568-198">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a568-199">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a568-199">Request headers</span></span>

| <span data-ttu-id="5a568-200">Nome</span><span class="sxs-lookup"><span data-stu-id="5a568-200">Name</span></span>       | <span data-ttu-id="5a568-201">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a568-201">Type</span></span> | <span data-ttu-id="5a568-202">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a568-202">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5a568-203">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a568-203">Authorization</span></span>  | <span data-ttu-id="5a568-204">string</span><span class="sxs-lookup"><span data-stu-id="5a568-204">string</span></span>  | <span data-ttu-id="5a568-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a568-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a568-207">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a568-207">Request body</span></span>

<span data-ttu-id="5a568-208">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5a568-208">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a568-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a568-209">Response</span></span>

<span data-ttu-id="5a568-210">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a568-210">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a568-211">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a568-211">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5a568-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a568-212">Request</span></span>

<span data-ttu-id="5a568-213">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a568-213">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5a568-214">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a568-214">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="5a568-215">C#</span><span class="sxs-lookup"><span data-stu-id="5a568-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a568-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a568-216">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a568-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a568-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a568-218">Java</span><span class="sxs-lookup"><span data-stu-id="5a568-218">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5a568-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a568-219">Response</span></span>

<span data-ttu-id="5a568-220">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a568-220">Here is an example of the response.</span></span>
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
  "includeResourceData": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

