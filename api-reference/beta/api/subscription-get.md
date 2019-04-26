---
title: Obter assinatura
description: Recupere as propriedades e os relacionamentos da uma assinatura.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 2ed0d30da74859650ef159f264618b0145644d76
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330552"
---
# <a name="get-subscription"></a><span data-ttu-id="95f2e-103">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="95f2e-103">Get subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95f2e-104">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="95f2e-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="95f2e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="95f2e-105">Permissions</span></span>

<span data-ttu-id="95f2e-106">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="95f2e-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="95f2e-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95f2e-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="95f2e-108">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="95f2e-108">Supported resource</span></span> | <span data-ttu-id="95f2e-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95f2e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="95f2e-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95f2e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95f2e-111">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95f2e-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="95f2e-112">contato</span><span class="sxs-lookup"><span data-stu-id="95f2e-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="95f2e-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="95f2e-113">Contacts.Read</span></span> | <span data-ttu-id="95f2e-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="95f2e-114">Contacts.Read</span></span> | <span data-ttu-id="95f2e-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="95f2e-115">Contacts.Read</span></span> |
|<span data-ttu-id="95f2e-116">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="95f2e-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="95f2e-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95f2e-117">Not supported</span></span> | <span data-ttu-id="95f2e-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95f2e-118">Files.ReadWrite</span></span> | <span data-ttu-id="95f2e-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95f2e-119">Not supported</span></span> |
|<span data-ttu-id="95f2e-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="95f2e-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="95f2e-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95f2e-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="95f2e-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95f2e-122">Not supported</span></span> | <span data-ttu-id="95f2e-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95f2e-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="95f2e-124">evento</span><span class="sxs-lookup"><span data-stu-id="95f2e-124">event</span></span>](../resources/event.md) | <span data-ttu-id="95f2e-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="95f2e-125">Calendars.Read</span></span> | <span data-ttu-id="95f2e-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="95f2e-126">Calendars.Read</span></span> | <span data-ttu-id="95f2e-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="95f2e-127">Calendars.Read</span></span> |
|[<span data-ttu-id="95f2e-128">grupo</span><span class="sxs-lookup"><span data-stu-id="95f2e-128">group</span></span>](../resources/group.md) | <span data-ttu-id="95f2e-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="95f2e-129">Group.Read.All</span></span> | <span data-ttu-id="95f2e-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95f2e-130">Not supported</span></span> | <span data-ttu-id="95f2e-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="95f2e-131">Group.Read.All</span></span> |
|[<span data-ttu-id="95f2e-132">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="95f2e-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="95f2e-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="95f2e-133">Group.Read.All</span></span> | <span data-ttu-id="95f2e-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95f2e-134">Not supported</span></span> | <span data-ttu-id="95f2e-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95f2e-135">Not supported</span></span> |
|[<span data-ttu-id="95f2e-136">mensagem</span><span class="sxs-lookup"><span data-stu-id="95f2e-136">message</span></span>](../resources/message.md) | <span data-ttu-id="95f2e-137">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="95f2e-137">Mail.Read</span></span> | <span data-ttu-id="95f2e-138">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="95f2e-138">Mail.Read</span></span> | <span data-ttu-id="95f2e-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="95f2e-139">Mail.Read</span></span> |
|[<span data-ttu-id="95f2e-140">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="95f2e-140">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="95f2e-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95f2e-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="95f2e-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95f2e-142">Not supported</span></span> | <span data-ttu-id="95f2e-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95f2e-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="95f2e-144">Usuário</span><span class="sxs-lookup"><span data-stu-id="95f2e-144">user</span></span>](../resources/user.md) | <span data-ttu-id="95f2e-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="95f2e-145">User.Read.All</span></span> | <span data-ttu-id="95f2e-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="95f2e-146">User.Read.All</span></span> | <span data-ttu-id="95f2e-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="95f2e-147">User.Read.All</span></span> |

> <span data-ttu-id="95f2e-148">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="95f2e-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="95f2e-149">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="95f2e-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="95f2e-150">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="95f2e-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="95f2e-151">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="95f2e-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="95f2e-152">As notificações são enviadas pelos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outros objetos driveItem na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="95f2e-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="95f2e-153">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="95f2e-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="95f2e-154">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="95f2e-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="95f2e-155">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="95f2e-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="95f2e-156">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="95f2e-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="95f2e-157">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="95f2e-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="95f2e-158">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="95f2e-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="95f2e-159">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95f2e-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="95f2e-160">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="95f2e-160">Optional query parameters</span></span>

<span data-ttu-id="95f2e-161">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="95f2e-161">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="95f2e-162">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95f2e-162">Request headers</span></span>

| <span data-ttu-id="95f2e-163">Nome</span><span class="sxs-lookup"><span data-stu-id="95f2e-163">Name</span></span>       | <span data-ttu-id="95f2e-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="95f2e-164">Type</span></span> | <span data-ttu-id="95f2e-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="95f2e-165">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="95f2e-166">Autorização</span><span class="sxs-lookup"><span data-stu-id="95f2e-166">Authorization</span></span>  | <span data-ttu-id="95f2e-167">string</span><span class="sxs-lookup"><span data-stu-id="95f2e-167">string</span></span>  | <span data-ttu-id="95f2e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95f2e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95f2e-170">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95f2e-170">Request body</span></span>

<span data-ttu-id="95f2e-171">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="95f2e-171">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95f2e-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="95f2e-172">Response</span></span>

<span data-ttu-id="95f2e-173">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95f2e-173">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95f2e-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95f2e-174">Example</span></span>

##### <a name="request"></a><span data-ttu-id="95f2e-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95f2e-175">Request</span></span>

<span data-ttu-id="95f2e-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95f2e-176">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="95f2e-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="95f2e-177">Response</span></span>

<span data-ttu-id="95f2e-178">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95f2e-178">Here is an example of the response.</span></span>
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
  "suppressions": []
}
-->
