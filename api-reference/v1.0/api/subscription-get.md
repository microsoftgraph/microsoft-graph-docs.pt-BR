---
title: Obter assinatura
description: Recupere as propriedades e os relacionamentos da uma assinatura.
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 52a0676db0e14a985b518799766f13a9f007c58a
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848188"
---
# <a name="get-subscription"></a><span data-ttu-id="dfc5a-103">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="dfc5a-103">Get subscription</span></span>

<span data-ttu-id="dfc5a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfc5a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dfc5a-105">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="dfc5a-105">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfc5a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dfc5a-106">Permissions</span></span>

<span data-ttu-id="dfc5a-107">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="dfc5a-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="dfc5a-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfc5a-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dfc5a-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="dfc5a-109">Supported resource</span></span> | <span data-ttu-id="dfc5a-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfc5a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dfc5a-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfc5a-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfc5a-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfc5a-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="dfc5a-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="dfc5a-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="dfc5a-114">Incompatível</span><span class="sxs-lookup"><span data-stu-id="dfc5a-114">Not supported</span></span> | <span data-ttu-id="dfc5a-115">Incompatível</span><span class="sxs-lookup"><span data-stu-id="dfc5a-115">Not supported</span></span> | <span data-ttu-id="dfc5a-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc5a-116">CallRecords.Read.All</span></span> |
|<span data-ttu-id="dfc5a-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="dfc5a-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="dfc5a-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dfc5a-118">Not supported</span></span> | <span data-ttu-id="dfc5a-119">Incompatível</span><span class="sxs-lookup"><span data-stu-id="dfc5a-119">Not supported</span></span> |  <span data-ttu-id="dfc5a-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc5a-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="dfc5a-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="dfc5a-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="dfc5a-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dfc5a-122">Not supported</span></span> | <span data-ttu-id="dfc5a-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dfc5a-123">Not supported</span></span> | <span data-ttu-id="dfc5a-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc5a-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="dfc5a-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="dfc5a-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="dfc5a-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dfc5a-126">Not supported</span></span> | <span data-ttu-id="dfc5a-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dfc5a-127">Not supported</span></span> | <span data-ttu-id="dfc5a-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc5a-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="dfc5a-129">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="dfc5a-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="dfc5a-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dfc5a-130">Not supported</span></span> | <span data-ttu-id="dfc5a-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dfc5a-131">Not supported</span></span> | <span data-ttu-id="dfc5a-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc5a-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="dfc5a-133">contato</span><span class="sxs-lookup"><span data-stu-id="dfc5a-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="dfc5a-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dfc5a-134">Contacts.Read</span></span> | <span data-ttu-id="dfc5a-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dfc5a-135">Contacts.Read</span></span> | <span data-ttu-id="dfc5a-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dfc5a-136">Contacts.Read</span></span> |
|<span data-ttu-id="dfc5a-137">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="dfc5a-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="dfc5a-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dfc5a-138">Not supported</span></span> | <span data-ttu-id="dfc5a-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfc5a-139">Files.ReadWrite</span></span> | <span data-ttu-id="dfc5a-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dfc5a-140">Not supported</span></span> |
|<span data-ttu-id="dfc5a-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="dfc5a-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="dfc5a-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfc5a-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="dfc5a-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dfc5a-143">Not supported</span></span> | <span data-ttu-id="dfc5a-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfc5a-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="dfc5a-145">evento</span><span class="sxs-lookup"><span data-stu-id="dfc5a-145">event</span></span>](../resources/event.md) | <span data-ttu-id="dfc5a-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dfc5a-146">Calendars.Read</span></span> | <span data-ttu-id="dfc5a-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dfc5a-147">Calendars.Read</span></span> | <span data-ttu-id="dfc5a-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dfc5a-148">Calendars.Read</span></span> |
|[<span data-ttu-id="dfc5a-149">grupo</span><span class="sxs-lookup"><span data-stu-id="dfc5a-149">group</span></span>](../resources/group.md) | <span data-ttu-id="dfc5a-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc5a-150">Group.Read.All</span></span> | <span data-ttu-id="dfc5a-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dfc5a-151">Not supported</span></span> | <span data-ttu-id="dfc5a-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc5a-152">Group.Read.All</span></span> |
|[<span data-ttu-id="dfc5a-153">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="dfc5a-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="dfc5a-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc5a-154">Group.Read.All</span></span> | <span data-ttu-id="dfc5a-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dfc5a-155">Not supported</span></span> | <span data-ttu-id="dfc5a-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dfc5a-156">Not supported</span></span> |
|[<span data-ttu-id="dfc5a-157">list</span><span class="sxs-lookup"><span data-stu-id="dfc5a-157">list</span></span>](../resources/list.md) | <span data-ttu-id="dfc5a-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfc5a-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="dfc5a-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dfc5a-159">Not supported</span></span> | <span data-ttu-id="dfc5a-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfc5a-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="dfc5a-161">message</span><span class="sxs-lookup"><span data-stu-id="dfc5a-161">message</span></span>](../resources/message.md) | <span data-ttu-id="dfc5a-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dfc5a-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="dfc5a-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dfc5a-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="dfc5a-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dfc5a-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="dfc5a-165">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="dfc5a-165">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="dfc5a-166">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfc5a-166">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="dfc5a-167">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dfc5a-167">Not supported</span></span> | <span data-ttu-id="dfc5a-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfc5a-168">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="dfc5a-169">Usuário</span><span class="sxs-lookup"><span data-stu-id="dfc5a-169">user</span></span>](../resources/user.md) | <span data-ttu-id="dfc5a-170">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc5a-170">User.Read.All</span></span> | <span data-ttu-id="dfc5a-171">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc5a-171">User.Read.All</span></span> | <span data-ttu-id="dfc5a-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc5a-172">User.Read.All</span></span> |

> <span data-ttu-id="dfc5a-173">**Observação** : Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="dfc5a-173">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="dfc5a-174">chatMessage</span><span class="sxs-lookup"><span data-stu-id="dfc5a-174">chatMessage</span></span>

<span data-ttu-id="dfc5a-175">Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="dfc5a-175">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="dfc5a-176">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="dfc5a-176">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="dfc5a-177">Antes de criar uma assinatura **chatMessage** , você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="dfc5a-177">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="dfc5a-178">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="dfc5a-178">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="dfc5a-179">**Observação:** `/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para os usuários que têm as [licenças necessárias](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="dfc5a-179">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="dfc5a-180">driveItem</span><span class="sxs-lookup"><span data-stu-id="dfc5a-180">driveItem</span></span>

<span data-ttu-id="dfc5a-181">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="dfc5a-181">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="dfc5a-182">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="dfc5a-182">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="dfc5a-183">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="dfc5a-183">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="dfc5a-184">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="dfc5a-184">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="dfc5a-185">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="dfc5a-185">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="dfc5a-186">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="dfc5a-186">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="dfc5a-187">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="dfc5a-187">contact, event, and message</span></span>

<span data-ttu-id="dfc5a-188">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="dfc5a-188">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="dfc5a-189">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="dfc5a-189">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="dfc5a-190">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="dfc5a-190">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="dfc5a-191">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="dfc5a-191">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="dfc5a-192">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_ :</span><span class="sxs-lookup"><span data-stu-id="dfc5a-192">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="dfc5a-193">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="dfc5a-193">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="dfc5a-194">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="dfc5a-194">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>
 

## <a name="http-request"></a><span data-ttu-id="dfc5a-195">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfc5a-195">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dfc5a-196">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dfc5a-196">Optional query parameters</span></span>

<span data-ttu-id="dfc5a-197">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dfc5a-197">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfc5a-198">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfc5a-198">Request headers</span></span>

| <span data-ttu-id="dfc5a-199">Nome</span><span class="sxs-lookup"><span data-stu-id="dfc5a-199">Name</span></span>       | <span data-ttu-id="dfc5a-200">Tipo</span><span class="sxs-lookup"><span data-stu-id="dfc5a-200">Type</span></span> | <span data-ttu-id="dfc5a-201">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfc5a-201">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dfc5a-202">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfc5a-202">Authorization</span></span>  | <span data-ttu-id="dfc5a-203">string</span><span class="sxs-lookup"><span data-stu-id="dfc5a-203">string</span></span>  | <span data-ttu-id="dfc5a-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfc5a-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfc5a-206">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfc5a-206">Request body</span></span>

<span data-ttu-id="dfc5a-207">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dfc5a-207">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfc5a-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfc5a-208">Response</span></span>

<span data-ttu-id="dfc5a-209">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfc5a-209">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfc5a-210">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dfc5a-210">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dfc5a-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfc5a-211">Request</span></span>

<span data-ttu-id="dfc5a-212">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfc5a-212">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dfc5a-213">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfc5a-213">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="dfc5a-214">C#</span><span class="sxs-lookup"><span data-stu-id="dfc5a-214">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dfc5a-215">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfc5a-215">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dfc5a-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dfc5a-216">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dfc5a-217">Java</span><span class="sxs-lookup"><span data-stu-id="dfc5a-217">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dfc5a-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfc5a-218">Response</span></span>

<span data-ttu-id="dfc5a-219">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfc5a-219">Here is an example of the response.</span></span>
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

