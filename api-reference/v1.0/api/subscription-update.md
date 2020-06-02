---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: eb9100490ace0fdfd95b0a061d9735c2d3c72dae
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491683"
---
# <a name="update-subscription"></a><span data-ttu-id="bf561-103">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="bf561-103">Update subscription</span></span>

<span data-ttu-id="bf561-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf561-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bf561-105">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="bf561-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="bf561-106">As assinaturas expiram após um período de tempo que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="bf561-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="bf561-107">Para evitar notificações de alteração ausentes, um aplicativo deve renovar as assinaturas bem antes da data de expiração.</span><span class="sxs-lookup"><span data-stu-id="bf561-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="bf561-108">Consulte [Subscription](../resources/subscription.md) para obter o tamanho máximo de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="bf561-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf561-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf561-109">Permissions</span></span>

<span data-ttu-id="bf561-110">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="bf561-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="bf561-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf561-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bf561-112">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="bf561-112">Supported resource</span></span> | <span data-ttu-id="bf561-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf561-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bf561-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf561-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf561-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf561-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="bf561-116">callRecord</span><span class="sxs-lookup"><span data-stu-id="bf561-116">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="bf561-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf561-117">Not supported</span></span> | <span data-ttu-id="bf561-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf561-118">Not supported</span></span> | <span data-ttu-id="bf561-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf561-119">CallRecords.Read.All</span></span>  |
|[<span data-ttu-id="bf561-120">contato</span><span class="sxs-lookup"><span data-stu-id="bf561-120">contact</span></span>](../resources/contact.md) | <span data-ttu-id="bf561-121">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="bf561-121">Contacts.Read</span></span> | <span data-ttu-id="bf561-122">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="bf561-122">Contacts.Read</span></span> | <span data-ttu-id="bf561-123">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="bf561-123">Contacts.Read</span></span> |
|<span data-ttu-id="bf561-124">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="bf561-124">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="bf561-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf561-125">Not supported</span></span> | <span data-ttu-id="bf561-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf561-126">Files.ReadWrite</span></span> | <span data-ttu-id="bf561-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf561-127">Not supported</span></span> |
|<span data-ttu-id="bf561-128">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="bf561-128">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="bf561-129">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf561-129">Files.ReadWrite.All</span></span> | <span data-ttu-id="bf561-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf561-130">Not supported</span></span> | <span data-ttu-id="bf561-131">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf561-131">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="bf561-132">evento</span><span class="sxs-lookup"><span data-stu-id="bf561-132">event</span></span>](../resources/event.md) | <span data-ttu-id="bf561-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bf561-133">Calendars.Read</span></span> | <span data-ttu-id="bf561-134">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bf561-134">Calendars.Read</span></span> | <span data-ttu-id="bf561-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bf561-135">Calendars.Read</span></span> |
|[<span data-ttu-id="bf561-136">grupo</span><span class="sxs-lookup"><span data-stu-id="bf561-136">group</span></span>](../resources/group.md) | <span data-ttu-id="bf561-137">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf561-137">Group.Read.All</span></span> | <span data-ttu-id="bf561-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf561-138">Not supported</span></span> | <span data-ttu-id="bf561-139">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf561-139">Group.Read.All</span></span> |
|[<span data-ttu-id="bf561-140">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="bf561-140">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="bf561-141">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf561-141">Group.Read.All</span></span> | <span data-ttu-id="bf561-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf561-142">Not supported</span></span> | <span data-ttu-id="bf561-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf561-143">Not supported</span></span> |
|[<span data-ttu-id="bf561-144">list</span><span class="sxs-lookup"><span data-stu-id="bf561-144">list</span></span>](../resources/list.md) | <span data-ttu-id="bf561-145">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf561-145">Sites.ReadWrite.All</span></span> | <span data-ttu-id="bf561-146">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf561-146">Not supported</span></span> | <span data-ttu-id="bf561-147">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf561-147">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="bf561-148">message</span><span class="sxs-lookup"><span data-stu-id="bf561-148">message</span></span>](../resources/message.md) | <span data-ttu-id="bf561-149">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bf561-149">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="bf561-150">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bf561-150">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="bf561-151">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bf561-151">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="bf561-152">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="bf561-152">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="bf561-153">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf561-153">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="bf561-154">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf561-154">Not supported</span></span> | <span data-ttu-id="bf561-155">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf561-155">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="bf561-156">Usuário</span><span class="sxs-lookup"><span data-stu-id="bf561-156">user</span></span>](../resources/user.md) | <span data-ttu-id="bf561-157">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf561-157">User.Read.All</span></span> | <span data-ttu-id="bf561-158">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf561-158">User.Read.All</span></span> | <span data-ttu-id="bf561-159">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf561-159">User.Read.All</span></span> |

> <span data-ttu-id="bf561-160">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="bf561-160">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="bf561-161">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="bf561-161">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="bf561-162">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="bf561-162">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="bf561-163">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="bf561-163">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="bf561-164">As notificações de alteração são enviadas para os tipos solicitados de alterações na pasta inscrita ou qualquer arquivo, pasta ou outro objeto driveItem em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="bf561-164">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="bf561-165">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="bf561-165">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="bf561-166">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="bf561-166">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="bf561-167">Isso significa que, por exemplo, você não pode usar os calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="bf561-167">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="bf561-168">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="bf561-168">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="bf561-169">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="bf561-169">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="bf561-170">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="bf561-170">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="bf561-171">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf561-171">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bf561-172">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf561-172">Request headers</span></span>

| <span data-ttu-id="bf561-173">Nome</span><span class="sxs-lookup"><span data-stu-id="bf561-173">Name</span></span>       | <span data-ttu-id="bf561-174">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf561-174">Type</span></span> | <span data-ttu-id="bf561-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf561-175">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bf561-176">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf561-176">Authorization</span></span>  | <span data-ttu-id="bf561-177">string</span><span class="sxs-lookup"><span data-stu-id="bf561-177">string</span></span>  | <span data-ttu-id="bf561-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf561-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bf561-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf561-180">Response</span></span>

<span data-ttu-id="bf561-181">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf561-181">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="bf561-182">Para obter detalhes sobre como os erros são retornados, confira [respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="bf561-182">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="bf561-183">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf561-183">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bf561-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf561-184">Request</span></span>

<span data-ttu-id="bf561-185">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf561-185">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bf561-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf561-186">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bf561-187">C#</span><span class="sxs-lookup"><span data-stu-id="bf561-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf561-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf561-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf561-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf561-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bf561-190">Java</span><span class="sxs-lookup"><span data-stu-id="bf561-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bf561-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf561-191">Response</span></span>

<span data-ttu-id="bf561-192">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf561-192">Here is an example of the response.</span></span>
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
