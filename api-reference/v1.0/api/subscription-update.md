---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: d8a434c6760635fef602b77bbc6631d52c666f40
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108456"
---
# <a name="update-subscription"></a><span data-ttu-id="ba469-103">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="ba469-103">Update subscription</span></span>

<span data-ttu-id="ba469-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba469-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ba469-105">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="ba469-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="ba469-106">As assinaturas expiram após um período de tempo que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="ba469-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="ba469-107">Para evitar notificações ausentes, um aplicativo deve renovar suas assinaturas bem antes da data de expiração.</span><span class="sxs-lookup"><span data-stu-id="ba469-107">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="ba469-108">Consulte [Subscription](../resources/subscription.md) para obter o tamanho máximo de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="ba469-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba469-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba469-109">Permissions</span></span>

<span data-ttu-id="ba469-110">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="ba469-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="ba469-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba469-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba469-112">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="ba469-112">Supported resource</span></span> | <span data-ttu-id="ba469-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba469-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ba469-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba469-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba469-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba469-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="ba469-116">contato</span><span class="sxs-lookup"><span data-stu-id="ba469-116">contact</span></span>](../resources/contact.md) | <span data-ttu-id="ba469-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ba469-117">Contacts.Read</span></span> | <span data-ttu-id="ba469-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ba469-118">Contacts.Read</span></span> | <span data-ttu-id="ba469-119">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ba469-119">Contacts.Read</span></span> |
|<span data-ttu-id="ba469-120">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="ba469-120">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="ba469-121">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ba469-121">Not supported</span></span> | <span data-ttu-id="ba469-122">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba469-122">Files.ReadWrite</span></span> | <span data-ttu-id="ba469-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ba469-123">Not supported</span></span> |
|<span data-ttu-id="ba469-124">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="ba469-124">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="ba469-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba469-125">Files.ReadWrite.All</span></span> | <span data-ttu-id="ba469-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ba469-126">Not supported</span></span> | <span data-ttu-id="ba469-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba469-127">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="ba469-128">evento</span><span class="sxs-lookup"><span data-stu-id="ba469-128">event</span></span>](../resources/event.md) | <span data-ttu-id="ba469-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ba469-129">Calendars.Read</span></span> | <span data-ttu-id="ba469-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ba469-130">Calendars.Read</span></span> | <span data-ttu-id="ba469-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ba469-131">Calendars.Read</span></span> |
|[<span data-ttu-id="ba469-132">grupo</span><span class="sxs-lookup"><span data-stu-id="ba469-132">group</span></span>](../resources/group.md) | <span data-ttu-id="ba469-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba469-133">Group.Read.All</span></span> | <span data-ttu-id="ba469-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ba469-134">Not supported</span></span> | <span data-ttu-id="ba469-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba469-135">Group.Read.All</span></span> |
|[<span data-ttu-id="ba469-136">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="ba469-136">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="ba469-137">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba469-137">Group.Read.All</span></span> | <span data-ttu-id="ba469-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ba469-138">Not supported</span></span> | <span data-ttu-id="ba469-139">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ba469-139">Not supported</span></span> |
|[<span data-ttu-id="ba469-140">lista</span><span class="sxs-lookup"><span data-stu-id="ba469-140">list</span></span>](../resources/list.md) | <span data-ttu-id="ba469-141">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba469-141">Sites.ReadWrite.All</span></span> | <span data-ttu-id="ba469-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ba469-142">Not supported</span></span> | <span data-ttu-id="ba469-143">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba469-143">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="ba469-144">message</span><span class="sxs-lookup"><span data-stu-id="ba469-144">message</span></span>](../resources/message.md) | <span data-ttu-id="ba469-145">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ba469-145">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="ba469-146">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ba469-146">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="ba469-147">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ba469-147">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="ba469-148">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="ba469-148">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="ba469-149">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba469-149">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="ba469-150">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ba469-150">Not supported</span></span> | <span data-ttu-id="ba469-151">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba469-151">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="ba469-152">Usuário</span><span class="sxs-lookup"><span data-stu-id="ba469-152">user</span></span>](../resources/user.md) | <span data-ttu-id="ba469-153">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba469-153">User.Read.All</span></span> | <span data-ttu-id="ba469-154">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba469-154">User.Read.All</span></span> | <span data-ttu-id="ba469-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba469-155">User.Read.All</span></span> |

> <span data-ttu-id="ba469-156">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="ba469-156">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="ba469-157">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="ba469-157">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="ba469-158">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="ba469-158">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="ba469-159">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="ba469-159">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="ba469-160">As notificações são enviadas pelos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outros objetos driveItem na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="ba469-160">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="ba469-161">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="ba469-161">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="ba469-162">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="ba469-162">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="ba469-163">Isso significa que, por exemplo, não é possível usar os calendários de permissão delegada. Leia para inscrever-se em eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="ba469-163">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="ba469-164">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="ba469-164">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="ba469-165">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="ba469-165">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="ba469-166">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="ba469-166">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="ba469-167">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba469-167">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ba469-168">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba469-168">Request headers</span></span>

| <span data-ttu-id="ba469-169">Nome</span><span class="sxs-lookup"><span data-stu-id="ba469-169">Name</span></span>       | <span data-ttu-id="ba469-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba469-170">Type</span></span> | <span data-ttu-id="ba469-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba469-171">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ba469-172">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba469-172">Authorization</span></span>  | <span data-ttu-id="ba469-173">string</span><span class="sxs-lookup"><span data-stu-id="ba469-173">string</span></span>  | <span data-ttu-id="ba469-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba469-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ba469-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba469-176">Response</span></span>

<span data-ttu-id="ba469-177">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba469-177">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba469-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba469-178">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ba469-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba469-179">Request</span></span>

<span data-ttu-id="ba469-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba469-180">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ba469-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba469-181">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ba469-182">C#</span><span class="sxs-lookup"><span data-stu-id="ba469-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba469-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba469-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba469-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba469-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba469-185">Java</span><span class="sxs-lookup"><span data-stu-id="ba469-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ba469-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba469-186">Response</span></span>

<span data-ttu-id="ba469-187">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba469-187">Here is an example of the response.</span></span>
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

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
