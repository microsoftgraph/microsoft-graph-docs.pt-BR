---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: e868489ca5eb95cdc2ee8c33176c8da20271bd12
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537094"
---
# <a name="update-subscription"></a><span data-ttu-id="cdefb-103">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="cdefb-103">Update subscription</span></span>

<span data-ttu-id="cdefb-104">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="cdefb-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="cdefb-105">As assinaturas expiram após um período de tempo que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="cdefb-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="cdefb-106">Para evitar notificações ausentes, um aplicativo deve renovar suas assinaturas bem antes da data de expiração.</span><span class="sxs-lookup"><span data-stu-id="cdefb-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="cdefb-107">Consulte [Subscription](../resources/subscription.md) para obter o tamanho máximo de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="cdefb-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdefb-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="cdefb-108">Permissions</span></span>

<span data-ttu-id="cdefb-109">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="cdefb-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="cdefb-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdefb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cdefb-111">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="cdefb-111">Supported resource</span></span> | <span data-ttu-id="cdefb-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdefb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cdefb-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cdefb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdefb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdefb-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="cdefb-115">contato</span><span class="sxs-lookup"><span data-stu-id="cdefb-115">contact</span></span>](../resources/contact.md) | <span data-ttu-id="cdefb-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="cdefb-116">Contacts.Read</span></span> | <span data-ttu-id="cdefb-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="cdefb-117">Contacts.Read</span></span> | <span data-ttu-id="cdefb-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="cdefb-118">Contacts.Read</span></span> |
|<span data-ttu-id="cdefb-119">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="cdefb-119">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="cdefb-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="cdefb-120">Not supported</span></span> | <span data-ttu-id="cdefb-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdefb-121">Files.ReadWrite</span></span> | <span data-ttu-id="cdefb-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="cdefb-122">Not supported</span></span> |
|<span data-ttu-id="cdefb-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="cdefb-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="cdefb-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdefb-124">Files.ReadWrite.All</span></span> | <span data-ttu-id="cdefb-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="cdefb-125">Not supported</span></span> | <span data-ttu-id="cdefb-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdefb-126">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="cdefb-127">evento</span><span class="sxs-lookup"><span data-stu-id="cdefb-127">event</span></span>](../resources/event.md) | <span data-ttu-id="cdefb-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="cdefb-128">Calendars.Read</span></span> | <span data-ttu-id="cdefb-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="cdefb-129">Calendars.Read</span></span> | <span data-ttu-id="cdefb-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="cdefb-130">Calendars.Read</span></span> |
|[<span data-ttu-id="cdefb-131">grupo</span><span class="sxs-lookup"><span data-stu-id="cdefb-131">group</span></span>](../resources/group.md) | <span data-ttu-id="cdefb-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdefb-132">Group.Read.All</span></span> | <span data-ttu-id="cdefb-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="cdefb-133">Not supported</span></span> | <span data-ttu-id="cdefb-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdefb-134">Group.Read.All</span></span> |
|[<span data-ttu-id="cdefb-135">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="cdefb-135">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="cdefb-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdefb-136">Group.Read.All</span></span> | <span data-ttu-id="cdefb-137">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="cdefb-137">Not supported</span></span> | <span data-ttu-id="cdefb-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="cdefb-138">Not supported</span></span> |
|[<span data-ttu-id="cdefb-139">mensagem</span><span class="sxs-lookup"><span data-stu-id="cdefb-139">message</span></span>](../resources/message.md) | <span data-ttu-id="cdefb-140">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cdefb-140">Mail.Read</span></span> | <span data-ttu-id="cdefb-141">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cdefb-141">Mail.Read</span></span> | <span data-ttu-id="cdefb-142">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cdefb-142">Mail.Read</span></span> |
|[<span data-ttu-id="cdefb-143">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="cdefb-143">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="cdefb-144">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdefb-144">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="cdefb-145">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="cdefb-145">Not supported</span></span> | <span data-ttu-id="cdefb-146">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdefb-146">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="cdefb-147">Usuário</span><span class="sxs-lookup"><span data-stu-id="cdefb-147">user</span></span>](../resources/user.md) | <span data-ttu-id="cdefb-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdefb-148">User.Read.All</span></span> | <span data-ttu-id="cdefb-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdefb-149">User.Read.All</span></span> | <span data-ttu-id="cdefb-150">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdefb-150">User.Read.All</span></span> |

> <span data-ttu-id="cdefb-151">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="cdefb-151">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="cdefb-152">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="cdefb-152">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="cdefb-153">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="cdefb-153">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="cdefb-154">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="cdefb-154">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="cdefb-155">As notificações são enviadas pelos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outros objetos driveItem na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="cdefb-155">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="cdefb-156">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="cdefb-156">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="cdefb-157">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="cdefb-157">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="cdefb-158">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="cdefb-158">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="cdefb-159">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="cdefb-159">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="cdefb-160">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="cdefb-160">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="cdefb-161">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="cdefb-161">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="cdefb-162">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdefb-162">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cdefb-163">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cdefb-163">Request headers</span></span>

| <span data-ttu-id="cdefb-164">Nome</span><span class="sxs-lookup"><span data-stu-id="cdefb-164">Name</span></span>       | <span data-ttu-id="cdefb-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdefb-165">Type</span></span> | <span data-ttu-id="cdefb-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdefb-166">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cdefb-167">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdefb-167">Authorization</span></span>  | <span data-ttu-id="cdefb-168">string</span><span class="sxs-lookup"><span data-stu-id="cdefb-168">string</span></span>  | <span data-ttu-id="cdefb-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdefb-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="cdefb-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdefb-171">Response</span></span>

<span data-ttu-id="cdefb-172">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdefb-172">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdefb-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cdefb-173">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cdefb-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdefb-174">Request</span></span>

<span data-ttu-id="cdefb-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cdefb-175">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="cdefb-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdefb-176">Response</span></span>

<span data-ttu-id="cdefb-177">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdefb-177">Here is an example of the response.</span></span>
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
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
