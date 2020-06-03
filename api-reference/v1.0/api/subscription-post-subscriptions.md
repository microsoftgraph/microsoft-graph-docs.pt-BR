---
title: Criar assinatura
description: Assina um aplicativo de escuta para receber notificações de alteração quando os dados do Microsoft Graph são alterados.
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 28053ccd79b8cbab521f3cbd702dd46835d14ecb
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491824"
---
# <a name="create-subscription"></a><span data-ttu-id="b07f8-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="b07f8-103">Create subscription</span></span>

<span data-ttu-id="b07f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b07f8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b07f8-105">Assina um aplicativo de escuta para receber notificações de alteração quando o tipo solicitado de alterações ocorrerem no recurso especificado no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b07f8-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="b07f8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b07f8-106">Permissions</span></span>

 <span data-ttu-id="b07f8-107">Criar uma assinatura exige o escopo de leitura do recurso.</span><span class="sxs-lookup"><span data-stu-id="b07f8-107">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="b07f8-108">Por exemplo, para obter notificações de alteração em mensagens, seu aplicativo precisa da `Mail.Read` permissão.</span><span class="sxs-lookup"><span data-stu-id="b07f8-108">For example, to get change notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="b07f8-109">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="b07f8-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="b07f8-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b07f8-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b07f8-111">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="b07f8-111">Supported resource</span></span> | <span data-ttu-id="b07f8-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b07f8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b07f8-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b07f8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b07f8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b07f8-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="b07f8-115">[callRecord](../resources/callrecords-callrecord.md) (/Communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="b07f8-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="b07f8-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b07f8-116">Not supported</span></span> | <span data-ttu-id="b07f8-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b07f8-117">Not supported</span></span> | <span data-ttu-id="b07f8-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="b07f8-118">CallRecords.Read.All</span></span>  |
|[<span data-ttu-id="b07f8-119">contato</span><span class="sxs-lookup"><span data-stu-id="b07f8-119">contact</span></span>](../resources/contact.md) | <span data-ttu-id="b07f8-120">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b07f8-120">Contacts.Read</span></span> | <span data-ttu-id="b07f8-121">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b07f8-121">Contacts.Read</span></span> | <span data-ttu-id="b07f8-122">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b07f8-122">Contacts.Read</span></span> |
|<span data-ttu-id="b07f8-123">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="b07f8-123">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="b07f8-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b07f8-124">Not supported</span></span> | <span data-ttu-id="b07f8-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b07f8-125">Files.ReadWrite</span></span> | <span data-ttu-id="b07f8-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b07f8-126">Not supported</span></span> |
|<span data-ttu-id="b07f8-127">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="b07f8-127">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="b07f8-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b07f8-128">Files.ReadWrite.All</span></span> | <span data-ttu-id="b07f8-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b07f8-129">Not supported</span></span> | <span data-ttu-id="b07f8-130">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b07f8-130">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="b07f8-131">evento</span><span class="sxs-lookup"><span data-stu-id="b07f8-131">event</span></span>](../resources/event.md) | <span data-ttu-id="b07f8-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b07f8-132">Calendars.Read</span></span> | <span data-ttu-id="b07f8-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b07f8-133">Calendars.Read</span></span> | <span data-ttu-id="b07f8-134">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b07f8-134">Calendars.Read</span></span> |
|[<span data-ttu-id="b07f8-135">grupo</span><span class="sxs-lookup"><span data-stu-id="b07f8-135">group</span></span>](../resources/group.md) | <span data-ttu-id="b07f8-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b07f8-136">Group.Read.All</span></span> | <span data-ttu-id="b07f8-137">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b07f8-137">Not supported</span></span> | <span data-ttu-id="b07f8-138">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b07f8-138">Group.Read.All</span></span> |
|[<span data-ttu-id="b07f8-139">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="b07f8-139">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="b07f8-140">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b07f8-140">Group.Read.All</span></span> | <span data-ttu-id="b07f8-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b07f8-141">Not supported</span></span> | <span data-ttu-id="b07f8-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b07f8-142">Not supported</span></span> |
|[<span data-ttu-id="b07f8-143">list</span><span class="sxs-lookup"><span data-stu-id="b07f8-143">list</span></span>](../resources/list.md) | <span data-ttu-id="b07f8-144">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b07f8-144">Sites.ReadWrite.All</span></span> | <span data-ttu-id="b07f8-145">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b07f8-145">Not supported</span></span> | <span data-ttu-id="b07f8-146">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b07f8-146">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="b07f8-147">message</span><span class="sxs-lookup"><span data-stu-id="b07f8-147">message</span></span>](../resources/message.md) | <span data-ttu-id="b07f8-148">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b07f8-148">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="b07f8-149">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b07f8-149">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="b07f8-150">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b07f8-150">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="b07f8-151">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="b07f8-151">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="b07f8-152">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b07f8-152">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="b07f8-153">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b07f8-153">Not supported</span></span> | <span data-ttu-id="b07f8-154">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b07f8-154">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="b07f8-155">Usuário</span><span class="sxs-lookup"><span data-stu-id="b07f8-155">user</span></span>](../resources/user.md) | <span data-ttu-id="b07f8-156">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b07f8-156">User.Read.All</span></span> | <span data-ttu-id="b07f8-157">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b07f8-157">User.Read.All</span></span> | <span data-ttu-id="b07f8-158">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b07f8-158">User.Read.All</span></span> |

> <span data-ttu-id="b07f8-159">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="b07f8-159">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="b07f8-160">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="b07f8-160">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="b07f8-161">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="b07f8-161">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="b07f8-162">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="b07f8-162">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="b07f8-163">As notificações de alteração são enviadas para os tipos solicitados de alterações na pasta inscrita ou qualquer arquivo, pasta ou outra instância do **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="b07f8-163">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="b07f8-164">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="b07f8-164">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="b07f8-165">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="b07f8-165">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="b07f8-166">Isso significa que, por exemplo, você não pode usar os calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="b07f8-166">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="b07f8-167">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="b07f8-167">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="b07f8-168">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="b07f8-168">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="b07f8-169">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="b07f8-169">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span> 


## <a name="http-request"></a><span data-ttu-id="b07f8-170">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b07f8-170">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="b07f8-171">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b07f8-171">Request headers</span></span>

| <span data-ttu-id="b07f8-172">Nome</span><span class="sxs-lookup"><span data-stu-id="b07f8-172">Name</span></span>       | <span data-ttu-id="b07f8-173">Tipo</span><span class="sxs-lookup"><span data-stu-id="b07f8-173">Type</span></span> | <span data-ttu-id="b07f8-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="b07f8-174">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b07f8-175">Autorização</span><span class="sxs-lookup"><span data-stu-id="b07f8-175">Authorization</span></span>  | <span data-ttu-id="b07f8-176">string</span><span class="sxs-lookup"><span data-stu-id="b07f8-176">string</span></span>  | <span data-ttu-id="b07f8-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b07f8-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b07f8-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="b07f8-179">Response</span></span>

<span data-ttu-id="b07f8-180">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b07f8-180">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>
<span data-ttu-id="b07f8-181">Para obter detalhes sobre como os erros são retornados, confira [respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="b07f8-181">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="b07f8-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b07f8-182">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b07f8-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b07f8-183">Request</span></span>

<span data-ttu-id="b07f8-184">Aqui está um exemplo da solicitação para enviar uma notificação de alteração quando o usuário recebe um novo email.</span><span class="sxs-lookup"><span data-stu-id="b07f8-184">Here is an example of the request to send a change notification when the user receives a new mail.</span></span>

# <a name="http"></a>[<span data-ttu-id="b07f8-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="b07f8-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue",
   "latestSupportedTlsVersion": "v1_2"
}
```
# <a name="c"></a>[<span data-ttu-id="b07f8-186">C#</span><span class="sxs-lookup"><span data-stu-id="b07f8-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b07f8-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b07f8-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b07f8-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b07f8-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b07f8-189">Java</span><span class="sxs-lookup"><span data-stu-id="b07f8-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="b07f8-190">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="b07f8-190">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="b07f8-191">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="b07f8-191">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="b07f8-192">Exemplos de recursos</span><span class="sxs-lookup"><span data-stu-id="b07f8-192">Resources examples</span></span>

<span data-ttu-id="b07f8-193">Estes são os valores válidos da propriedade de recurso da assinatura:</span><span class="sxs-lookup"><span data-stu-id="b07f8-193">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="b07f8-194">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="b07f8-194">Resource type</span></span> | <span data-ttu-id="b07f8-195">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b07f8-195">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="b07f8-196">Email</span><span class="sxs-lookup"><span data-stu-id="b07f8-196">Mail</span></span>|<span data-ttu-id="b07f8-197">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="b07f8-197">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="b07f8-198">me/messages</span><span class="sxs-lookup"><span data-stu-id="b07f8-198">me/messages</span></span>|
|<span data-ttu-id="b07f8-199">Contatos</span><span class="sxs-lookup"><span data-stu-id="b07f8-199">Contacts</span></span>|<span data-ttu-id="b07f8-200">me/contacts</span><span class="sxs-lookup"><span data-stu-id="b07f8-200">me/contacts</span></span>|
|<span data-ttu-id="b07f8-201">Calendários</span><span class="sxs-lookup"><span data-stu-id="b07f8-201">Calendars</span></span>|<span data-ttu-id="b07f8-202">me/events</span><span class="sxs-lookup"><span data-stu-id="b07f8-202">me/events</span></span>|
|<span data-ttu-id="b07f8-203">Usuários</span><span class="sxs-lookup"><span data-stu-id="b07f8-203">Users</span></span>|<span data-ttu-id="b07f8-204">usuários</span><span class="sxs-lookup"><span data-stu-id="b07f8-204">users</span></span>|
|<span data-ttu-id="b07f8-205">Grupos</span><span class="sxs-lookup"><span data-stu-id="b07f8-205">Groups</span></span>|<span data-ttu-id="b07f8-206">grupos</span><span class="sxs-lookup"><span data-stu-id="b07f8-206">groups</span></span>|
|<span data-ttu-id="b07f8-207">Conversas</span><span class="sxs-lookup"><span data-stu-id="b07f8-207">Conversations</span></span>|<span data-ttu-id="b07f8-208">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="b07f8-208">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="b07f8-209">Unidades</span><span class="sxs-lookup"><span data-stu-id="b07f8-209">Drives</span></span>|<span data-ttu-id="b07f8-210">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="b07f8-210">me/drive/root</span></span>|
|<span data-ttu-id="b07f8-211">Listar</span><span class="sxs-lookup"><span data-stu-id="b07f8-211">List</span></span>|<span data-ttu-id="b07f8-212">sites/{site-id}/lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="b07f8-212">sites/{site-id}/lists/{list-id}</span></span>|
|<span data-ttu-id="b07f8-213">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="b07f8-213">Security alert</span></span>|<span data-ttu-id="b07f8-214">security/alerts?$filter=status eq 'New'</span><span class="sxs-lookup"><span data-stu-id="b07f8-214">security/alerts?$filter=status eq 'New'</span></span>|
|<span data-ttu-id="b07f8-215">Registros de chamadas</span><span class="sxs-lookup"><span data-stu-id="b07f8-215">Call records</span></span>|<span data-ttu-id="b07f8-216">comunicações/callRecords</span><span class="sxs-lookup"><span data-stu-id="b07f8-216">communications/callRecords</span></span>|

##### <a name="response"></a><span data-ttu-id="b07f8-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="b07f8-217">Response</span></span>

<span data-ttu-id="b07f8-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b07f8-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "changeType": "updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="b07f8-221">Validação de ponto de extremidade da notificação</span><span class="sxs-lookup"><span data-stu-id="b07f8-221">Notification endpoint validation</span></span>

<span data-ttu-id="b07f8-222">O ponto de extremidade da notificação da assinatura (especificado na `notificationUrl` propriedade) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [Configurar notificações para alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="b07f8-222">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="b07f8-223">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="b07f8-223">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
