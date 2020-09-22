---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: aee0ca84cccd371c307b405357516d8fda61deab
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038029"
---
# <a name="update-subscription"></a><span data-ttu-id="e62c8-103">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="e62c8-103">Update subscription</span></span>

<span data-ttu-id="e62c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e62c8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e62c8-105">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="e62c8-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="e62c8-106">As assinaturas expiram após um período de tempo que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="e62c8-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="e62c8-107">Para evitar notificações de alteração ausentes, um aplicativo deve renovar as assinaturas bem antes da data de expiração.</span><span class="sxs-lookup"><span data-stu-id="e62c8-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="e62c8-108">Consulte [Subscription](../resources/subscription.md) para obter o tamanho máximo de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="e62c8-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="e62c8-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="e62c8-109">Permissions</span></span>

<span data-ttu-id="e62c8-110">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="e62c8-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="e62c8-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e62c8-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e62c8-112">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="e62c8-112">Supported resource</span></span> | <span data-ttu-id="e62c8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e62c8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e62c8-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e62c8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e62c8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e62c8-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="e62c8-116">callRecord</span><span class="sxs-lookup"><span data-stu-id="e62c8-116">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="e62c8-117">Incompatível</span><span class="sxs-lookup"><span data-stu-id="e62c8-117">Not supported</span></span> | <span data-ttu-id="e62c8-118">Incompatível</span><span class="sxs-lookup"><span data-stu-id="e62c8-118">Not supported</span></span> | <span data-ttu-id="e62c8-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="e62c8-119">CallRecords.Read.All</span></span>  |
|[<span data-ttu-id="e62c8-120">contato</span><span class="sxs-lookup"><span data-stu-id="e62c8-120">contact</span></span>](../resources/contact.md) | <span data-ttu-id="e62c8-121">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e62c8-121">Contacts.Read</span></span> | <span data-ttu-id="e62c8-122">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e62c8-122">Contacts.Read</span></span> | <span data-ttu-id="e62c8-123">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e62c8-123">Contacts.Read</span></span> |
|<span data-ttu-id="e62c8-124">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="e62c8-124">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="e62c8-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e62c8-125">Not supported</span></span> | <span data-ttu-id="e62c8-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e62c8-126">Files.ReadWrite</span></span> | <span data-ttu-id="e62c8-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e62c8-127">Not supported</span></span> |
|<span data-ttu-id="e62c8-128">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="e62c8-128">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="e62c8-129">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e62c8-129">Files.ReadWrite.All</span></span> | <span data-ttu-id="e62c8-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e62c8-130">Not supported</span></span> | <span data-ttu-id="e62c8-131">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e62c8-131">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="e62c8-132">evento</span><span class="sxs-lookup"><span data-stu-id="e62c8-132">event</span></span>](../resources/event.md) | <span data-ttu-id="e62c8-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e62c8-133">Calendars.Read</span></span> | <span data-ttu-id="e62c8-134">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e62c8-134">Calendars.Read</span></span> | <span data-ttu-id="e62c8-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e62c8-135">Calendars.Read</span></span> |
|[<span data-ttu-id="e62c8-136">grupo</span><span class="sxs-lookup"><span data-stu-id="e62c8-136">group</span></span>](../resources/group.md) | <span data-ttu-id="e62c8-137">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e62c8-137">Group.Read.All</span></span> | <span data-ttu-id="e62c8-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e62c8-138">Not supported</span></span> | <span data-ttu-id="e62c8-139">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e62c8-139">Group.Read.All</span></span> |
|[<span data-ttu-id="e62c8-140">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="e62c8-140">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="e62c8-141">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e62c8-141">Group.Read.All</span></span> | <span data-ttu-id="e62c8-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e62c8-142">Not supported</span></span> | <span data-ttu-id="e62c8-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e62c8-143">Not supported</span></span> |
|[<span data-ttu-id="e62c8-144">list</span><span class="sxs-lookup"><span data-stu-id="e62c8-144">list</span></span>](../resources/list.md) | <span data-ttu-id="e62c8-145">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e62c8-145">Sites.ReadWrite.All</span></span> | <span data-ttu-id="e62c8-146">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e62c8-146">Not supported</span></span> | <span data-ttu-id="e62c8-147">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e62c8-147">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="e62c8-148">message</span><span class="sxs-lookup"><span data-stu-id="e62c8-148">message</span></span>](../resources/message.md) | <span data-ttu-id="e62c8-149">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e62c8-149">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="e62c8-150">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e62c8-150">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="e62c8-151">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e62c8-151">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="e62c8-152">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="e62c8-152">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="e62c8-153">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e62c8-153">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="e62c8-154">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e62c8-154">Not supported</span></span> | <span data-ttu-id="e62c8-155">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e62c8-155">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="e62c8-156">Usuário</span><span class="sxs-lookup"><span data-stu-id="e62c8-156">user</span></span>](../resources/user.md) | <span data-ttu-id="e62c8-157">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e62c8-157">User.Read.All</span></span> | <span data-ttu-id="e62c8-158">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e62c8-158">User.Read.All</span></span> | <span data-ttu-id="e62c8-159">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e62c8-159">User.Read.All</span></span> |

> <span data-ttu-id="e62c8-160">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="e62c8-160">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="e62c8-161">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="e62c8-161">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="e62c8-162">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="e62c8-162">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="e62c8-163">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="e62c8-163">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="e62c8-164">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta, ou outros objetos driveItem em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="e62c8-164">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="e62c8-165">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="e62c8-165">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="e62c8-166">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="e62c8-166">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="e62c8-167">Isso significa que, por exemplo, você não pode usar os calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="e62c8-167">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="e62c8-168">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="e62c8-168">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="e62c8-169">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="e62c8-169">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="e62c8-170">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="e62c8-170">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="e62c8-171">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e62c8-171">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e62c8-172">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e62c8-172">Request headers</span></span>

| <span data-ttu-id="e62c8-173">Nome</span><span class="sxs-lookup"><span data-stu-id="e62c8-173">Name</span></span>       | <span data-ttu-id="e62c8-174">Tipo</span><span class="sxs-lookup"><span data-stu-id="e62c8-174">Type</span></span> | <span data-ttu-id="e62c8-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="e62c8-175">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e62c8-176">Autorização</span><span class="sxs-lookup"><span data-stu-id="e62c8-176">Authorization</span></span>  | <span data-ttu-id="e62c8-177">string</span><span class="sxs-lookup"><span data-stu-id="e62c8-177">string</span></span>  | <span data-ttu-id="e62c8-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e62c8-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e62c8-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="e62c8-180">Response</span></span>

<span data-ttu-id="e62c8-181">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e62c8-181">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="e62c8-182">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="e62c8-182">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="e62c8-183">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e62c8-183">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e62c8-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e62c8-184">Request</span></span>

<span data-ttu-id="e62c8-185">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e62c8-185">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e62c8-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="e62c8-186">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e62c8-187">C#</span><span class="sxs-lookup"><span data-stu-id="e62c8-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e62c8-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e62c8-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e62c8-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e62c8-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e62c8-190">Java</span><span class="sxs-lookup"><span data-stu-id="e62c8-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e62c8-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="e62c8-191">Response</span></span>

<span data-ttu-id="e62c8-192">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e62c8-192">Here is an example of the response.</span></span>
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

