---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: e868489ca5eb95cdc2ee8c33176c8da20271bd12
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159532"
---
# <a name="update-subscription"></a><span data-ttu-id="6cfad-103">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="6cfad-103">Update subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cfad-104">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="6cfad-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="6cfad-105">As assinaturas expiram após um período de tempo que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="6cfad-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="6cfad-106">Para evitar notificações ausentes, um aplicativo deve renovar suas assinaturas bem antes da data de expiração.</span><span class="sxs-lookup"><span data-stu-id="6cfad-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="6cfad-107">Consulte [Subscription](../resources/subscription.md) para obter o tamanho máximo de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="6cfad-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cfad-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="6cfad-108">Permissions</span></span>

<span data-ttu-id="6cfad-109">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o menos privilegiado necessário para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6cfad-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="6cfad-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cfad-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6cfad-111">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="6cfad-111">Supported resource</span></span> | <span data-ttu-id="6cfad-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cfad-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6cfad-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cfad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cfad-114">Application</span><span class="sxs-lookup"><span data-stu-id="6cfad-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="6cfad-115">contato</span><span class="sxs-lookup"><span data-stu-id="6cfad-115">contact</span></span>](../resources/contact.md) | <span data-ttu-id="6cfad-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6cfad-116">Contacts.Read</span></span> | <span data-ttu-id="6cfad-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6cfad-117">Contacts.Read</span></span> | <span data-ttu-id="6cfad-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6cfad-118">Contacts.Read</span></span> |
|<span data-ttu-id="6cfad-119">[driveItem](../resources/driveitem.md) (OneDrive pessoal do usuário)</span><span class="sxs-lookup"><span data-stu-id="6cfad-119">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="6cfad-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6cfad-120">Not supported</span></span> | <span data-ttu-id="6cfad-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6cfad-121">Files.ReadWrite</span></span> | <span data-ttu-id="6cfad-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6cfad-122">Not supported</span></span> |
|<span data-ttu-id="6cfad-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="6cfad-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="6cfad-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cfad-124">Files.ReadWrite.All</span></span> | <span data-ttu-id="6cfad-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6cfad-125">Not supported</span></span> | <span data-ttu-id="6cfad-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cfad-126">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="6cfad-127">event</span><span class="sxs-lookup"><span data-stu-id="6cfad-127">event</span></span>](../resources/event.md) | <span data-ttu-id="6cfad-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6cfad-128">Calendars.Read</span></span> | <span data-ttu-id="6cfad-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6cfad-129">Calendars.Read</span></span> | <span data-ttu-id="6cfad-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6cfad-130">Calendars.Read</span></span> |
|[<span data-ttu-id="6cfad-131">group</span><span class="sxs-lookup"><span data-stu-id="6cfad-131">group</span></span>](../resources/group.md) | <span data-ttu-id="6cfad-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cfad-132">Group.Read.All</span></span> | <span data-ttu-id="6cfad-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6cfad-133">Not supported</span></span> | <span data-ttu-id="6cfad-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cfad-134">Group.Read.All</span></span> |
|[<span data-ttu-id="6cfad-135">conversa de grupo</span><span class="sxs-lookup"><span data-stu-id="6cfad-135">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="6cfad-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cfad-136">Group.Read.All</span></span> | <span data-ttu-id="6cfad-137">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6cfad-137">Not supported</span></span> | <span data-ttu-id="6cfad-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6cfad-138">Not supported</span></span> |
|[<span data-ttu-id="6cfad-139">message</span><span class="sxs-lookup"><span data-stu-id="6cfad-139">message</span></span>](../resources/message.md) | <span data-ttu-id="6cfad-140">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6cfad-140">Mail.Read</span></span> | <span data-ttu-id="6cfad-141">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6cfad-141">Mail.Read</span></span> | <span data-ttu-id="6cfad-142">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6cfad-142">Mail.Read</span></span> |
|[<span data-ttu-id="6cfad-143">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="6cfad-143">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="6cfad-144">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cfad-144">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="6cfad-145">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6cfad-145">Not supported</span></span> | <span data-ttu-id="6cfad-146">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cfad-146">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="6cfad-147">user</span><span class="sxs-lookup"><span data-stu-id="6cfad-147">user</span></span>](../resources/user.md) | <span data-ttu-id="6cfad-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cfad-148">User.Read.All</span></span> | <span data-ttu-id="6cfad-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cfad-149">User.Read.All</span></span> | <span data-ttu-id="6cfad-150">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cfad-150">User.Read.All</span></span> |

> <span data-ttu-id="6cfad-151">**Observação:** Há limitações adicionais para assinaturas em itens do OneDrive e do Outlook.</span><span class="sxs-lookup"><span data-stu-id="6cfad-151">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="6cfad-152">As limitações se aplicam à criação e ao gerenciamento de assinaturas (obtendo, atualizando e excluindo assinaturas).</span><span class="sxs-lookup"><span data-stu-id="6cfad-152">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="6cfad-153">No OneDrive pessoal, você pode inscrever-se na pasta raiz ou em qualquer subpasta nessa unidade.</span><span class="sxs-lookup"><span data-stu-id="6cfad-153">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="6cfad-154">No OneDrive for Business, você pode inscrever-se apenas na pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="6cfad-154">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="6cfad-155">As notificações são enviadas para os tipos solicitados de alterações na pasta inscrita ou qualquer arquivo, pasta ou outro objeto driveItem em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="6cfad-155">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="6cfad-156">Você não pode se inscrever em instâncias de **unidade** ou **driveItem** que não são pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="6cfad-156">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="6cfad-157">No Outlook, a permissão delegada oferece suporte à assinatura de itens em pastas somente na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="6cfad-157">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="6cfad-158">Isso significa que, por exemplo, não é possível usar os calendários de permissão delegada. Leia para inscrever-se em eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="6cfad-158">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="6cfad-159">Para inscrever-se para alterar as notificações de contatos, eventos ou mensagens do Outlook em pastas compartilhadas _ou delegadas_ :</span><span class="sxs-lookup"><span data-stu-id="6cfad-159">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="6cfad-160">Use a permissão de aplicativo correspondente para inscrever-se nas alterações de itens em uma pasta ou em uma caixa de correio de _qualquer_ usuário no locatário.</span><span class="sxs-lookup"><span data-stu-id="6cfad-160">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="6cfad-161">Não use as permissões de compartilhamento do Outlook (Contacts. Read. Shared, caLendars. Read. Shared, mail. Read. Shared e suas contrapartes de leitura/gravação), já que eles **não** oferecem suporte à inscrição para alterar notificações em itens em pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="6cfad-161">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="6cfad-162">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6cfad-162">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6cfad-163">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6cfad-163">Request headers</span></span>

| <span data-ttu-id="6cfad-164">Nome</span><span class="sxs-lookup"><span data-stu-id="6cfad-164">Name</span></span>       | <span data-ttu-id="6cfad-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cfad-165">Type</span></span> | <span data-ttu-id="6cfad-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cfad-166">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6cfad-167">Autorização</span><span class="sxs-lookup"><span data-stu-id="6cfad-167">Authorization</span></span>  | <span data-ttu-id="6cfad-168">string</span><span class="sxs-lookup"><span data-stu-id="6cfad-168">string</span></span>  | <span data-ttu-id="6cfad-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6cfad-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6cfad-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cfad-171">Response</span></span>

<span data-ttu-id="6cfad-172">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6cfad-172">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cfad-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6cfad-173">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6cfad-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6cfad-174">Request</span></span>

<span data-ttu-id="6cfad-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6cfad-175">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="6cfad-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cfad-176">Response</span></span>

<span data-ttu-id="6cfad-177">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6cfad-177">Here is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/subscription-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
