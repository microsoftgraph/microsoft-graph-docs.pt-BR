---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 1278c6f61ddb62165ef125acc810d5ae6dde0454
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353165"
---
# <a name="update-subscription"></a><span data-ttu-id="e3d42-103">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="e3d42-103">Update subscription</span></span>

<span data-ttu-id="e3d42-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3d42-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3d42-105">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="e3d42-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="e3d42-106">As assinaturas expiram após um período de tempo que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="e3d42-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="e3d42-107">Para evitar notificações de alteração ausentes, um aplicativo deve renovar as assinaturas bem antes da data de expiração.</span><span class="sxs-lookup"><span data-stu-id="e3d42-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="e3d42-108">Consulte [Subscription](../resources/subscription.md) para obter o tamanho máximo de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="e3d42-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3d42-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="e3d42-109">Permissions</span></span>

<span data-ttu-id="e3d42-110">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="e3d42-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="e3d42-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3d42-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3d42-112">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="e3d42-112">Supported resource</span></span> | <span data-ttu-id="e3d42-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3d42-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e3d42-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3d42-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3d42-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3d42-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="e3d42-116">contato</span><span class="sxs-lookup"><span data-stu-id="e3d42-116">contact</span></span>](../resources/contact.md) | <span data-ttu-id="e3d42-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e3d42-117">Contacts.Read</span></span> | <span data-ttu-id="e3d42-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e3d42-118">Contacts.Read</span></span> | <span data-ttu-id="e3d42-119">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e3d42-119">Contacts.Read</span></span> |
|<span data-ttu-id="e3d42-120">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="e3d42-120">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="e3d42-121">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e3d42-121">Not supported</span></span> | <span data-ttu-id="e3d42-122">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3d42-122">Files.ReadWrite</span></span> | <span data-ttu-id="e3d42-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e3d42-123">Not supported</span></span> |
|<span data-ttu-id="e3d42-124">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="e3d42-124">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="e3d42-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3d42-125">Files.ReadWrite.All</span></span> | <span data-ttu-id="e3d42-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e3d42-126">Not supported</span></span> | <span data-ttu-id="e3d42-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3d42-127">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="e3d42-128">evento</span><span class="sxs-lookup"><span data-stu-id="e3d42-128">event</span></span>](../resources/event.md) | <span data-ttu-id="e3d42-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e3d42-129">Calendars.Read</span></span> | <span data-ttu-id="e3d42-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e3d42-130">Calendars.Read</span></span> | <span data-ttu-id="e3d42-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e3d42-131">Calendars.Read</span></span> |
|[<span data-ttu-id="e3d42-132">grupo</span><span class="sxs-lookup"><span data-stu-id="e3d42-132">group</span></span>](../resources/group.md) | <span data-ttu-id="e3d42-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3d42-133">Group.Read.All</span></span> | <span data-ttu-id="e3d42-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e3d42-134">Not supported</span></span> | <span data-ttu-id="e3d42-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3d42-135">Group.Read.All</span></span> |
|[<span data-ttu-id="e3d42-136">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="e3d42-136">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="e3d42-137">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3d42-137">Group.Read.All</span></span> | <span data-ttu-id="e3d42-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e3d42-138">Not supported</span></span> | <span data-ttu-id="e3d42-139">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e3d42-139">Not supported</span></span> |
|[<span data-ttu-id="e3d42-140">list</span><span class="sxs-lookup"><span data-stu-id="e3d42-140">list</span></span>](../resources/list.md) | <span data-ttu-id="e3d42-141">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3d42-141">Sites.ReadWrite.All</span></span> | <span data-ttu-id="e3d42-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e3d42-142">Not supported</span></span> | <span data-ttu-id="e3d42-143">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3d42-143">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="e3d42-144">message</span><span class="sxs-lookup"><span data-stu-id="e3d42-144">message</span></span>](../resources/message.md) | <span data-ttu-id="e3d42-145">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e3d42-145">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="e3d42-146">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e3d42-146">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="e3d42-147">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e3d42-147">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="e3d42-148">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="e3d42-148">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="e3d42-149">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3d42-149">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="e3d42-150">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e3d42-150">Not supported</span></span> | <span data-ttu-id="e3d42-151">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3d42-151">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="e3d42-152">Usuário</span><span class="sxs-lookup"><span data-stu-id="e3d42-152">user</span></span>](../resources/user.md) | <span data-ttu-id="e3d42-153">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3d42-153">User.Read.All</span></span> | <span data-ttu-id="e3d42-154">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3d42-154">User.Read.All</span></span> | <span data-ttu-id="e3d42-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3d42-155">User.Read.All</span></span> |

> <span data-ttu-id="e3d42-156">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="e3d42-156">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="e3d42-157">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="e3d42-157">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="e3d42-158">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="e3d42-158">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="e3d42-159">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="e3d42-159">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="e3d42-160">As notificações de alteração são enviadas para os tipos solicitados de alterações na pasta inscrita ou qualquer arquivo, pasta ou outro objeto driveItem em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="e3d42-160">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="e3d42-161">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="e3d42-161">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="e3d42-162">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="e3d42-162">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="e3d42-163">Isso significa que, por exemplo, você não pode usar os calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="e3d42-163">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="e3d42-164">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="e3d42-164">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="e3d42-165">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="e3d42-165">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="e3d42-166">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="e3d42-166">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="e3d42-167">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3d42-167">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e3d42-168">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3d42-168">Request headers</span></span>

| <span data-ttu-id="e3d42-169">Nome</span><span class="sxs-lookup"><span data-stu-id="e3d42-169">Name</span></span>       | <span data-ttu-id="e3d42-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3d42-170">Type</span></span> | <span data-ttu-id="e3d42-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3d42-171">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e3d42-172">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3d42-172">Authorization</span></span>  | <span data-ttu-id="e3d42-173">string</span><span class="sxs-lookup"><span data-stu-id="e3d42-173">string</span></span>  | <span data-ttu-id="e3d42-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3d42-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e3d42-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3d42-176">Response</span></span>

<span data-ttu-id="e3d42-177">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3d42-177">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="e3d42-178">Para obter detalhes sobre como os erros são retornados, confira [respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="e3d42-178">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="e3d42-179">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3d42-179">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e3d42-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3d42-180">Request</span></span>

<span data-ttu-id="e3d42-181">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3d42-181">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e3d42-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3d42-182">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e3d42-183">C#</span><span class="sxs-lookup"><span data-stu-id="e3d42-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3d42-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3d42-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3d42-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3d42-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3d42-186">Java</span><span class="sxs-lookup"><span data-stu-id="e3d42-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e3d42-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3d42-187">Response</span></span>

<span data-ttu-id="e3d42-188">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3d42-188">Here is an example of the response.</span></span>
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
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
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
