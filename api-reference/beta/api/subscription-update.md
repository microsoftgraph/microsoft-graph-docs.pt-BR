---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
author: piotrci
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 8df27c24839467543323fcab583b36f825d8193e
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38702549"
---
# <a name="update-subscription"></a><span data-ttu-id="bbf2f-103">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="bbf2f-103">Update subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbf2f-104">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="bbf2f-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="bbf2f-105">As assinaturas expiram após um período de tempo que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="bbf2f-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="bbf2f-106">Para evitar notificações ausentes, um aplicativo deve renovar suas assinaturas bem antes da data de expiração.</span><span class="sxs-lookup"><span data-stu-id="bbf2f-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="bbf2f-107">Consulte [Subscription](../resources/subscription.md) para obter o tamanho máximo de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="bbf2f-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbf2f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="bbf2f-108">Permissions</span></span>

<span data-ttu-id="bbf2f-109">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="bbf2f-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="bbf2f-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbf2f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bbf2f-111">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="bbf2f-111">Supported resource</span></span> | <span data-ttu-id="bbf2f-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbf2f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bbf2f-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbf2f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbf2f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbf2f-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="bbf2f-115">contato</span><span class="sxs-lookup"><span data-stu-id="bbf2f-115">contact</span></span>](../resources/contact.md) | <span data-ttu-id="bbf2f-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="bbf2f-116">Contacts.Read</span></span> | <span data-ttu-id="bbf2f-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="bbf2f-117">Contacts.Read</span></span> | <span data-ttu-id="bbf2f-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="bbf2f-118">Contacts.Read</span></span> |
|<span data-ttu-id="bbf2f-119">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="bbf2f-119">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="bbf2f-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bbf2f-120">Not supported</span></span> | <span data-ttu-id="bbf2f-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bbf2f-121">Files.ReadWrite</span></span> | <span data-ttu-id="bbf2f-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bbf2f-122">Not supported</span></span> |
|<span data-ttu-id="bbf2f-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="bbf2f-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="bbf2f-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbf2f-124">Files.ReadWrite.All</span></span> | <span data-ttu-id="bbf2f-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bbf2f-125">Not supported</span></span> | <span data-ttu-id="bbf2f-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbf2f-126">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="bbf2f-127">evento</span><span class="sxs-lookup"><span data-stu-id="bbf2f-127">event</span></span>](../resources/event.md) | <span data-ttu-id="bbf2f-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bbf2f-128">Calendars.Read</span></span> | <span data-ttu-id="bbf2f-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bbf2f-129">Calendars.Read</span></span> | <span data-ttu-id="bbf2f-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bbf2f-130">Calendars.Read</span></span> |
|[<span data-ttu-id="bbf2f-131">grupo</span><span class="sxs-lookup"><span data-stu-id="bbf2f-131">group</span></span>](../resources/group.md) | <span data-ttu-id="bbf2f-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbf2f-132">Group.Read.All</span></span> | <span data-ttu-id="bbf2f-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bbf2f-133">Not supported</span></span> | <span data-ttu-id="bbf2f-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbf2f-134">Group.Read.All</span></span> |
|[<span data-ttu-id="bbf2f-135">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="bbf2f-135">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="bbf2f-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbf2f-136">Group.Read.All</span></span> | <span data-ttu-id="bbf2f-137">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bbf2f-137">Not supported</span></span> | <span data-ttu-id="bbf2f-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bbf2f-138">Not supported</span></span> |
|[<span data-ttu-id="bbf2f-139">Mensagem</span><span class="sxs-lookup"><span data-stu-id="bbf2f-139">message</span></span>](../resources/message.md) | <span data-ttu-id="bbf2f-140">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="bbf2f-140">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="bbf2f-141">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="bbf2f-141">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="bbf2f-142">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="bbf2f-142">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="bbf2f-143">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="bbf2f-143">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="bbf2f-144">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbf2f-144">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="bbf2f-145">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bbf2f-145">Not supported</span></span> | <span data-ttu-id="bbf2f-146">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbf2f-146">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="bbf2f-147">Usuário</span><span class="sxs-lookup"><span data-stu-id="bbf2f-147">user</span></span>](../resources/user.md) | <span data-ttu-id="bbf2f-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbf2f-148">User.Read.All</span></span> | <span data-ttu-id="bbf2f-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbf2f-149">User.Read.All</span></span> | <span data-ttu-id="bbf2f-150">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbf2f-150">User.Read.All</span></span> |

> <span data-ttu-id="bbf2f-151">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="bbf2f-151">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="bbf2f-152">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="bbf2f-152">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="bbf2f-153">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="bbf2f-153">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="bbf2f-154">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="bbf2f-154">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="bbf2f-155">As notificações são enviadas pelos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outros objetos driveItem na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="bbf2f-155">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="bbf2f-156">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="bbf2f-156">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="bbf2f-157">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="bbf2f-157">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="bbf2f-158">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="bbf2f-158">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="bbf2f-159">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="bbf2f-159">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="bbf2f-160">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="bbf2f-160">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="bbf2f-161">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="bbf2f-161">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="bbf2f-162">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbf2f-162">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bbf2f-163">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbf2f-163">Request headers</span></span>

| <span data-ttu-id="bbf2f-164">Nome</span><span class="sxs-lookup"><span data-stu-id="bbf2f-164">Name</span></span>       | <span data-ttu-id="bbf2f-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbf2f-165">Type</span></span> | <span data-ttu-id="bbf2f-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbf2f-166">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bbf2f-167">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbf2f-167">Authorization</span></span>  | <span data-ttu-id="bbf2f-168">string</span><span class="sxs-lookup"><span data-stu-id="bbf2f-168">string</span></span>  | <span data-ttu-id="bbf2f-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbf2f-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bbf2f-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbf2f-171">Response</span></span>

<span data-ttu-id="bbf2f-172">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbf2f-172">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbf2f-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbf2f-173">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bbf2f-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbf2f-174">Request</span></span>

<span data-ttu-id="bbf2f-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbf2f-175">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bbf2f-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbf2f-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/beta/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bbf2f-177">C#</span><span class="sxs-lookup"><span data-stu-id="bbf2f-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bbf2f-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bbf2f-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bbf2f-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbf2f-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bbf2f-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbf2f-180">Response</span></span>

<span data-ttu-id="bbf2f-181">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbf2f-181">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
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
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
