---
title: Criar assinatura
description: Assina um aplicativo de escuta para receber notificações quando os dados no Microsoft Graph são alterados.
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 4a1a2f899ec8e52e342ffe86f163ca4514a1d85e
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108470"
---
# <a name="create-subscription"></a><span data-ttu-id="89b03-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="89b03-103">Create subscription</span></span>

<span data-ttu-id="89b03-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89b03-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89b03-105">Assinar um aplicativo de escuta para receber notificações quando o tipo de alterações solicitadas ocorrer em recursos específicos no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="89b03-105">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="89b03-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="89b03-106">Permissions</span></span>

 <span data-ttu-id="89b03-107">Criar uma assinatura exige o escopo de leitura do recurso.</span><span class="sxs-lookup"><span data-stu-id="89b03-107">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="89b03-108">Por exemplo, para obter notificações por mensagens, seu aplicativo precisa da `Mail.Read` permissão.</span><span class="sxs-lookup"><span data-stu-id="89b03-108">For example, to get notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="89b03-109">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="89b03-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="89b03-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89b03-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89b03-111">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="89b03-111">Supported resource</span></span> | <span data-ttu-id="89b03-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89b03-112">Delegated (work or school account)</span></span> | <span data-ttu-id="89b03-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89b03-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89b03-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89b03-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="89b03-115">contato</span><span class="sxs-lookup"><span data-stu-id="89b03-115">contact</span></span>](../resources/contact.md) | <span data-ttu-id="89b03-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="89b03-116">Contacts.Read</span></span> | <span data-ttu-id="89b03-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="89b03-117">Contacts.Read</span></span> | <span data-ttu-id="89b03-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="89b03-118">Contacts.Read</span></span> |
|<span data-ttu-id="89b03-119">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="89b03-119">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="89b03-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="89b03-120">Not supported</span></span> | <span data-ttu-id="89b03-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89b03-121">Files.ReadWrite</span></span> | <span data-ttu-id="89b03-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="89b03-122">Not supported</span></span> |
|<span data-ttu-id="89b03-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="89b03-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="89b03-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89b03-124">Files.ReadWrite.All</span></span> | <span data-ttu-id="89b03-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="89b03-125">Not supported</span></span> | <span data-ttu-id="89b03-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89b03-126">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="89b03-127">evento</span><span class="sxs-lookup"><span data-stu-id="89b03-127">event</span></span>](../resources/event.md) | <span data-ttu-id="89b03-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="89b03-128">Calendars.Read</span></span> | <span data-ttu-id="89b03-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="89b03-129">Calendars.Read</span></span> | <span data-ttu-id="89b03-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="89b03-130">Calendars.Read</span></span> |
|[<span data-ttu-id="89b03-131">grupo</span><span class="sxs-lookup"><span data-stu-id="89b03-131">group</span></span>](../resources/group.md) | <span data-ttu-id="89b03-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="89b03-132">Group.Read.All</span></span> | <span data-ttu-id="89b03-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="89b03-133">Not supported</span></span> | <span data-ttu-id="89b03-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="89b03-134">Group.Read.All</span></span> |
|[<span data-ttu-id="89b03-135">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="89b03-135">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="89b03-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="89b03-136">Group.Read.All</span></span> | <span data-ttu-id="89b03-137">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="89b03-137">Not supported</span></span> | <span data-ttu-id="89b03-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="89b03-138">Not supported</span></span> |
|[<span data-ttu-id="89b03-139">list</span><span class="sxs-lookup"><span data-stu-id="89b03-139">list</span></span>](../resources/list.md) | <span data-ttu-id="89b03-140">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89b03-140">Sites.ReadWrite.All</span></span> | <span data-ttu-id="89b03-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="89b03-141">Not supported</span></span> | <span data-ttu-id="89b03-142">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89b03-142">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="89b03-143">message</span><span class="sxs-lookup"><span data-stu-id="89b03-143">message</span></span>](../resources/message.md) | <span data-ttu-id="89b03-144">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="89b03-144">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="89b03-145">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="89b03-145">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="89b03-146">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="89b03-146">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="89b03-147">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="89b03-147">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="89b03-148">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89b03-148">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="89b03-149">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="89b03-149">Not supported</span></span> | <span data-ttu-id="89b03-150">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89b03-150">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="89b03-151">Usuário</span><span class="sxs-lookup"><span data-stu-id="89b03-151">user</span></span>](../resources/user.md) | <span data-ttu-id="89b03-152">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="89b03-152">User.Read.All</span></span> | <span data-ttu-id="89b03-153">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="89b03-153">User.Read.All</span></span> | <span data-ttu-id="89b03-154">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="89b03-154">User.Read.All</span></span> |

> <span data-ttu-id="89b03-155">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="89b03-155">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="89b03-156">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="89b03-156">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="89b03-157">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="89b03-157">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="89b03-158">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="89b03-158">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="89b03-159">As notificações são enviadas pelos tipos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outras instâncias **driveItem** na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="89b03-159">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="89b03-160">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="89b03-160">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="89b03-161">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="89b03-161">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="89b03-162">Isso significa que, por exemplo, você não pode usar os calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="89b03-162">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="89b03-163">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="89b03-163">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="89b03-164">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="89b03-164">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="89b03-165">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="89b03-165">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span> 


## <a name="http-request"></a><span data-ttu-id="89b03-166">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89b03-166">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="89b03-167">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89b03-167">Request headers</span></span>

| <span data-ttu-id="89b03-168">Nome</span><span class="sxs-lookup"><span data-stu-id="89b03-168">Name</span></span>       | <span data-ttu-id="89b03-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="89b03-169">Type</span></span> | <span data-ttu-id="89b03-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="89b03-170">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="89b03-171">Autorização</span><span class="sxs-lookup"><span data-stu-id="89b03-171">Authorization</span></span>  | <span data-ttu-id="89b03-172">string</span><span class="sxs-lookup"><span data-stu-id="89b03-172">string</span></span>  | <span data-ttu-id="89b03-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89b03-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="89b03-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="89b03-175">Response</span></span>

<span data-ttu-id="89b03-176">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89b03-176">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89b03-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89b03-177">Example</span></span>

##### <a name="request"></a><span data-ttu-id="89b03-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89b03-178">Request</span></span>

<span data-ttu-id="89b03-179">Veja a seguir um exemplo da solicitação para enviar uma notificação quando o usuário receber um novo email.</span><span class="sxs-lookup"><span data-stu-id="89b03-179">Here is an example of the request to send a notification when the user receives a new mail.</span></span>

# <a name="http"></a>[<span data-ttu-id="89b03-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="89b03-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="89b03-181">C#</span><span class="sxs-lookup"><span data-stu-id="89b03-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89b03-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89b03-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89b03-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89b03-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89b03-184">Java</span><span class="sxs-lookup"><span data-stu-id="89b03-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="89b03-185">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="89b03-185">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="89b03-186">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="89b03-186">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="89b03-187">Exemplos de recursos</span><span class="sxs-lookup"><span data-stu-id="89b03-187">Resources examples</span></span>

<span data-ttu-id="89b03-188">Estes são os valores válidos da propriedade de recurso da assinatura:</span><span class="sxs-lookup"><span data-stu-id="89b03-188">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="89b03-189">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="89b03-189">Resource type</span></span> | <span data-ttu-id="89b03-190">Exemplos</span><span class="sxs-lookup"><span data-stu-id="89b03-190">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="89b03-191">Email</span><span class="sxs-lookup"><span data-stu-id="89b03-191">Mail</span></span>|<span data-ttu-id="89b03-192">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="89b03-192">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="89b03-193">me/messages</span><span class="sxs-lookup"><span data-stu-id="89b03-193">me/messages</span></span>|
|<span data-ttu-id="89b03-194">Contatos</span><span class="sxs-lookup"><span data-stu-id="89b03-194">Contacts</span></span>|<span data-ttu-id="89b03-195">me/contacts</span><span class="sxs-lookup"><span data-stu-id="89b03-195">me/contacts</span></span>|
|<span data-ttu-id="89b03-196">Calendários</span><span class="sxs-lookup"><span data-stu-id="89b03-196">Calendars</span></span>|<span data-ttu-id="89b03-197">me/events</span><span class="sxs-lookup"><span data-stu-id="89b03-197">me/events</span></span>|
|<span data-ttu-id="89b03-198">Usuários</span><span class="sxs-lookup"><span data-stu-id="89b03-198">Users</span></span>|<span data-ttu-id="89b03-199">usuários</span><span class="sxs-lookup"><span data-stu-id="89b03-199">users</span></span>|
|<span data-ttu-id="89b03-200">Grupos</span><span class="sxs-lookup"><span data-stu-id="89b03-200">Groups</span></span>|<span data-ttu-id="89b03-201">grupos</span><span class="sxs-lookup"><span data-stu-id="89b03-201">groups</span></span>|
|<span data-ttu-id="89b03-202">Conversas</span><span class="sxs-lookup"><span data-stu-id="89b03-202">Conversations</span></span>|<span data-ttu-id="89b03-203">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="89b03-203">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="89b03-204">Unidades</span><span class="sxs-lookup"><span data-stu-id="89b03-204">Drives</span></span>|<span data-ttu-id="89b03-205">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="89b03-205">me/drive/root</span></span>|
|<span data-ttu-id="89b03-206">Listar</span><span class="sxs-lookup"><span data-stu-id="89b03-206">List</span></span>|<span data-ttu-id="89b03-207">site/{site-id}/lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="89b03-207">site/{site-id}/lists/{list-id}</span></span>|
|<span data-ttu-id="89b03-208">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="89b03-208">Security alert</span></span>|<span data-ttu-id="89b03-209">security/alerts?$filter=status eq 'New'</span><span class="sxs-lookup"><span data-stu-id="89b03-209">security/alerts?$filter=status eq 'New'</span></span>|

##### <a name="response"></a><span data-ttu-id="89b03-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="89b03-210">Response</span></span>

<span data-ttu-id="89b03-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89b03-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "changeType": "updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="89b03-214">Validação de ponto de extremidade da notificação</span><span class="sxs-lookup"><span data-stu-id="89b03-214">Notification endpoint validation</span></span>

<span data-ttu-id="89b03-215">O ponto de extremidade da notificação da assinatura (especificado na `notificationUrl` propriedade) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [Configurar notificações para alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="89b03-215">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="89b03-216">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="89b03-216">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
