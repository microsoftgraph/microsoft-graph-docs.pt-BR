---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 2900fd09839bdd570a41a5bad40578dec1c7ace8
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742213"
---
# <a name="update-subscription"></a><span data-ttu-id="8d20b-103">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="8d20b-103">Update subscription</span></span>

<span data-ttu-id="8d20b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d20b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8d20b-105">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="8d20b-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="8d20b-106">As assinaturas expiram após um período de tempo que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="8d20b-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="8d20b-107">Para evitar notificações de alteração ausentes, um aplicativo deve renovar as assinaturas bem antes da data de expiração.</span><span class="sxs-lookup"><span data-stu-id="8d20b-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="8d20b-108">Consulte [Subscription](../resources/subscription.md) para obter o tamanho máximo de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="8d20b-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d20b-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d20b-109">Permissions</span></span>

<span data-ttu-id="8d20b-110">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="8d20b-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="8d20b-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d20b-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8d20b-112">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="8d20b-112">Supported resource</span></span> | <span data-ttu-id="8d20b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d20b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8d20b-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d20b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d20b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d20b-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="8d20b-116">callRecord</span><span class="sxs-lookup"><span data-stu-id="8d20b-116">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="8d20b-117">Incompatível</span><span class="sxs-lookup"><span data-stu-id="8d20b-117">Not supported</span></span> | <span data-ttu-id="8d20b-118">Incompatível</span><span class="sxs-lookup"><span data-stu-id="8d20b-118">Not supported</span></span> | <span data-ttu-id="8d20b-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d20b-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="8d20b-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="8d20b-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="8d20b-121">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8d20b-121">Not supported</span></span> | <span data-ttu-id="8d20b-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8d20b-122">Not supported</span></span> | <span data-ttu-id="8d20b-123">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d20b-123">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="8d20b-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="8d20b-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="8d20b-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8d20b-125">Not supported</span></span> | <span data-ttu-id="8d20b-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8d20b-126">Not supported</span></span> | <span data-ttu-id="8d20b-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d20b-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="8d20b-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="8d20b-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="8d20b-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8d20b-129">Not supported</span></span> | <span data-ttu-id="8d20b-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8d20b-130">Not supported</span></span> | <span data-ttu-id="8d20b-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d20b-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="8d20b-132">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="8d20b-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="8d20b-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8d20b-133">Not supported</span></span> | <span data-ttu-id="8d20b-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8d20b-134">Not supported</span></span> | <span data-ttu-id="8d20b-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d20b-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="8d20b-136">contato</span><span class="sxs-lookup"><span data-stu-id="8d20b-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="8d20b-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8d20b-137">Contacts.Read</span></span> | <span data-ttu-id="8d20b-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8d20b-138">Contacts.Read</span></span> | <span data-ttu-id="8d20b-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8d20b-139">Contacts.Read</span></span> |
|<span data-ttu-id="8d20b-140">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="8d20b-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="8d20b-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8d20b-141">Not supported</span></span> | <span data-ttu-id="8d20b-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d20b-142">Files.ReadWrite</span></span> | <span data-ttu-id="8d20b-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8d20b-143">Not supported</span></span> |
|<span data-ttu-id="8d20b-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="8d20b-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="8d20b-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d20b-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="8d20b-146">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8d20b-146">Not supported</span></span> | <span data-ttu-id="8d20b-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d20b-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="8d20b-148">evento</span><span class="sxs-lookup"><span data-stu-id="8d20b-148">event</span></span>](../resources/event.md) | <span data-ttu-id="8d20b-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8d20b-149">Calendars.Read</span></span> | <span data-ttu-id="8d20b-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8d20b-150">Calendars.Read</span></span> | <span data-ttu-id="8d20b-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8d20b-151">Calendars.Read</span></span> |
|[<span data-ttu-id="8d20b-152">grupo</span><span class="sxs-lookup"><span data-stu-id="8d20b-152">group</span></span>](../resources/group.md) | <span data-ttu-id="8d20b-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d20b-153">Group.Read.All</span></span> | <span data-ttu-id="8d20b-154">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8d20b-154">Not supported</span></span> | <span data-ttu-id="8d20b-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d20b-155">Group.Read.All</span></span> |
|[<span data-ttu-id="8d20b-156">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="8d20b-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="8d20b-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d20b-157">Group.Read.All</span></span> | <span data-ttu-id="8d20b-158">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8d20b-158">Not supported</span></span> | <span data-ttu-id="8d20b-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8d20b-159">Not supported</span></span> |
|[<span data-ttu-id="8d20b-160">list</span><span class="sxs-lookup"><span data-stu-id="8d20b-160">list</span></span>](../resources/list.md) | <span data-ttu-id="8d20b-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d20b-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="8d20b-162">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8d20b-162">Not supported</span></span> | <span data-ttu-id="8d20b-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d20b-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="8d20b-164">message</span><span class="sxs-lookup"><span data-stu-id="8d20b-164">message</span></span>](../resources/message.md) | <span data-ttu-id="8d20b-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8d20b-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="8d20b-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8d20b-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="8d20b-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8d20b-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="8d20b-168">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="8d20b-168">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="8d20b-169">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d20b-169">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="8d20b-170">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8d20b-170">Not supported</span></span> | <span data-ttu-id="8d20b-171">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d20b-171">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="8d20b-172">Usuário</span><span class="sxs-lookup"><span data-stu-id="8d20b-172">user</span></span>](../resources/user.md) | <span data-ttu-id="8d20b-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d20b-173">User.Read.All</span></span> | <span data-ttu-id="8d20b-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d20b-174">User.Read.All</span></span> | <span data-ttu-id="8d20b-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d20b-175">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="8d20b-176">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8d20b-176">chatMessage</span></span>

<span data-ttu-id="8d20b-177">Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="8d20b-177">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="8d20b-178">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="8d20b-178">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="8d20b-179">Antes de criar uma assinatura **chatMessage**, você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="8d20b-179">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="8d20b-180">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="8d20b-180">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="8d20b-181">**Observação:** `/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para os usuários que têm as[licenças necessárias](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="8d20b-181">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="8d20b-182">driveItem</span><span class="sxs-lookup"><span data-stu-id="8d20b-182">driveItem</span></span>

<span data-ttu-id="8d20b-183">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8d20b-183">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="8d20b-184">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="8d20b-184">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="8d20b-185">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="8d20b-185">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="8d20b-186">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="8d20b-186">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="8d20b-187">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="8d20b-187">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="8d20b-188">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="8d20b-188">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="8d20b-189">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="8d20b-189">contact, event, and message</span></span>

<span data-ttu-id="8d20b-190">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="8d20b-190">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="8d20b-191">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="8d20b-191">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="8d20b-192">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="8d20b-192">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="8d20b-193">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="8d20b-193">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="8d20b-194">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="8d20b-194">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="8d20b-195">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="8d20b-195">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="8d20b-196">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="8d20b-196">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="8d20b-197">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d20b-197">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8d20b-198">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d20b-198">Request headers</span></span>

| <span data-ttu-id="8d20b-199">Nome</span><span class="sxs-lookup"><span data-stu-id="8d20b-199">Name</span></span>       | <span data-ttu-id="8d20b-200">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d20b-200">Type</span></span> | <span data-ttu-id="8d20b-201">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d20b-201">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8d20b-202">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d20b-202">Authorization</span></span>  | <span data-ttu-id="8d20b-203">string</span><span class="sxs-lookup"><span data-stu-id="8d20b-203">string</span></span>  | <span data-ttu-id="8d20b-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d20b-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8d20b-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d20b-206">Response</span></span>

<span data-ttu-id="8d20b-207">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d20b-207">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="8d20b-208">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="8d20b-208">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="8d20b-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d20b-209">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8d20b-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d20b-210">Request</span></span>

<span data-ttu-id="8d20b-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d20b-211">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8d20b-212">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d20b-212">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8d20b-213">C#</span><span class="sxs-lookup"><span data-stu-id="8d20b-213">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d20b-214">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d20b-214">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d20b-215">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d20b-215">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d20b-216">Java</span><span class="sxs-lookup"><span data-stu-id="8d20b-216">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8d20b-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d20b-217">Response</span></span>

<span data-ttu-id="8d20b-218">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d20b-218">Here is an example of the response.</span></span>
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

