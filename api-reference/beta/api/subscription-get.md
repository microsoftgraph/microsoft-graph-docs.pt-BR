---
title: Obter assinatura
description: Recupere as propriedades e os relacionamentos da uma assinatura.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: c73f01a65a2b81bfa34818f9a7a96f754501bd65
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163466"
---
# <a name="get-subscription"></a><span data-ttu-id="86c89-103">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="86c89-103">Get subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86c89-104">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="86c89-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="86c89-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="86c89-105">Permissions</span></span>

<span data-ttu-id="86c89-106">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o menos privilegiado necessário para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="86c89-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="86c89-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86c89-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="86c89-108">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="86c89-108">Supported resource</span></span> | <span data-ttu-id="86c89-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86c89-109">Delegated (work or school account)</span></span> | <span data-ttu-id="86c89-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86c89-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86c89-111">Application</span><span class="sxs-lookup"><span data-stu-id="86c89-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="86c89-112">contato</span><span class="sxs-lookup"><span data-stu-id="86c89-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="86c89-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="86c89-113">Contacts.Read</span></span> | <span data-ttu-id="86c89-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="86c89-114">Contacts.Read</span></span> | <span data-ttu-id="86c89-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="86c89-115">Contacts.Read</span></span> |
|<span data-ttu-id="86c89-116">[driveItem](../resources/driveitem.md) (OneDrive pessoal do usuário)</span><span class="sxs-lookup"><span data-stu-id="86c89-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="86c89-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="86c89-117">Not supported</span></span> | <span data-ttu-id="86c89-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86c89-118">Files.ReadWrite</span></span> | <span data-ttu-id="86c89-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="86c89-119">Not supported</span></span> |
|<span data-ttu-id="86c89-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="86c89-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="86c89-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86c89-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="86c89-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="86c89-122">Not supported</span></span> | <span data-ttu-id="86c89-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86c89-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="86c89-124">event</span><span class="sxs-lookup"><span data-stu-id="86c89-124">event</span></span>](../resources/event.md) | <span data-ttu-id="86c89-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="86c89-125">Calendars.Read</span></span> | <span data-ttu-id="86c89-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="86c89-126">Calendars.Read</span></span> | <span data-ttu-id="86c89-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="86c89-127">Calendars.Read</span></span> |
|[<span data-ttu-id="86c89-128">group</span><span class="sxs-lookup"><span data-stu-id="86c89-128">group</span></span>](../resources/group.md) | <span data-ttu-id="86c89-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="86c89-129">Group.Read.All</span></span> | <span data-ttu-id="86c89-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="86c89-130">Not supported</span></span> | <span data-ttu-id="86c89-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="86c89-131">Group.Read.All</span></span> |
|[<span data-ttu-id="86c89-132">conversa de grupo</span><span class="sxs-lookup"><span data-stu-id="86c89-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="86c89-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="86c89-133">Group.Read.All</span></span> | <span data-ttu-id="86c89-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="86c89-134">Not supported</span></span> | <span data-ttu-id="86c89-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="86c89-135">Not supported</span></span> |
|[<span data-ttu-id="86c89-136">message</span><span class="sxs-lookup"><span data-stu-id="86c89-136">message</span></span>](../resources/message.md) | <span data-ttu-id="86c89-137">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="86c89-137">Mail.Read</span></span> | <span data-ttu-id="86c89-138">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="86c89-138">Mail.Read</span></span> | <span data-ttu-id="86c89-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="86c89-139">Mail.Read</span></span> |
|[<span data-ttu-id="86c89-140">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="86c89-140">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="86c89-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86c89-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="86c89-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="86c89-142">Not supported</span></span> | <span data-ttu-id="86c89-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86c89-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="86c89-144">user</span><span class="sxs-lookup"><span data-stu-id="86c89-144">user</span></span>](../resources/user.md) | <span data-ttu-id="86c89-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="86c89-145">User.Read.All</span></span> | <span data-ttu-id="86c89-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="86c89-146">User.Read.All</span></span> | <span data-ttu-id="86c89-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="86c89-147">User.Read.All</span></span> |

> <span data-ttu-id="86c89-148">**Observação:** Há limitações adicionais para assinaturas em itens do OneDrive e do Outlook.</span><span class="sxs-lookup"><span data-stu-id="86c89-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="86c89-149">As limitações se aplicam à criação e ao gerenciamento de assinaturas (obtendo, atualizando e excluindo assinaturas).</span><span class="sxs-lookup"><span data-stu-id="86c89-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="86c89-150">No OneDrive pessoal, você pode inscrever-se na pasta raiz ou em qualquer subpasta nessa unidade.</span><span class="sxs-lookup"><span data-stu-id="86c89-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="86c89-151">No OneDrive for Business, você pode inscrever-se apenas na pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="86c89-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="86c89-152">As notificações são enviadas para os tipos solicitados de alterações na pasta inscrita ou qualquer arquivo, pasta ou outro objeto driveItem em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="86c89-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="86c89-153">Você não pode se inscrever em instâncias de **unidade** ou **driveItem** que não são pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="86c89-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="86c89-154">No Outlook, a permissão delegada oferece suporte à assinatura de itens em pastas somente na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="86c89-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="86c89-155">Isso significa que, por exemplo, não é possível usar os calendários de permissão delegada. Leia para inscrever-se em eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="86c89-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="86c89-156">Para inscrever-se para alterar as notificações de contatos, eventos ou mensagens do Outlook em pastas compartilhadas _ou delegadas_ :</span><span class="sxs-lookup"><span data-stu-id="86c89-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="86c89-157">Use a permissão de aplicativo correspondente para inscrever-se nas alterações de itens em uma pasta ou em uma caixa de correio de _qualquer_ usuário no locatário.</span><span class="sxs-lookup"><span data-stu-id="86c89-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="86c89-158">Não use as permissões de compartilhamento do Outlook (Contacts. Read. Shared, caLendars. Read. Shared, mail. Read. Shared e suas contrapartes de leitura/gravação), já que eles **não** oferecem suporte à inscrição para alterar notificações em itens em pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="86c89-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="86c89-159">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86c89-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="86c89-160">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="86c89-160">Optional query parameters</span></span>

<span data-ttu-id="86c89-161">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="86c89-161">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86c89-162">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86c89-162">Request headers</span></span>

| <span data-ttu-id="86c89-163">Nome</span><span class="sxs-lookup"><span data-stu-id="86c89-163">Name</span></span>       | <span data-ttu-id="86c89-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="86c89-164">Type</span></span> | <span data-ttu-id="86c89-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="86c89-165">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="86c89-166">Autorização</span><span class="sxs-lookup"><span data-stu-id="86c89-166">Authorization</span></span>  | <span data-ttu-id="86c89-167">string</span><span class="sxs-lookup"><span data-stu-id="86c89-167">string</span></span>  | <span data-ttu-id="86c89-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86c89-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86c89-170">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86c89-170">Request body</span></span>

<span data-ttu-id="86c89-171">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86c89-171">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86c89-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="86c89-172">Response</span></span>

<span data-ttu-id="86c89-173">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86c89-173">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86c89-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86c89-174">Example</span></span>

##### <a name="request"></a><span data-ttu-id="86c89-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86c89-175">Request</span></span>

<span data-ttu-id="86c89-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86c89-176">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="86c89-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="86c89-177">Response</span></span>

<span data-ttu-id="86c89-178">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86c89-178">Here is an example of the response.</span></span>
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
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
