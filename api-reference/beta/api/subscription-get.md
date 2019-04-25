---
title: Obter assinatura
description: Recupere as propriedades e os relacionamentos da uma assinatura.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: c73f01a65a2b81bfa34818f9a7a96f754501bd65
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545169"
---
# <a name="get-subscription"></a><span data-ttu-id="603ab-103">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="603ab-103">Get subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="603ab-104">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="603ab-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="603ab-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="603ab-105">Permissions</span></span>

<span data-ttu-id="603ab-106">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="603ab-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="603ab-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="603ab-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="603ab-108">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="603ab-108">Supported resource</span></span> | <span data-ttu-id="603ab-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="603ab-109">Delegated (work or school account)</span></span> | <span data-ttu-id="603ab-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="603ab-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="603ab-111">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="603ab-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="603ab-112">contato</span><span class="sxs-lookup"><span data-stu-id="603ab-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="603ab-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="603ab-113">Contacts.Read</span></span> | <span data-ttu-id="603ab-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="603ab-114">Contacts.Read</span></span> | <span data-ttu-id="603ab-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="603ab-115">Contacts.Read</span></span> |
|<span data-ttu-id="603ab-116">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="603ab-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="603ab-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="603ab-117">Not supported</span></span> | <span data-ttu-id="603ab-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="603ab-118">Files.ReadWrite</span></span> | <span data-ttu-id="603ab-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="603ab-119">Not supported</span></span> |
|<span data-ttu-id="603ab-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="603ab-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="603ab-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="603ab-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="603ab-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="603ab-122">Not supported</span></span> | <span data-ttu-id="603ab-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="603ab-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="603ab-124">evento</span><span class="sxs-lookup"><span data-stu-id="603ab-124">event</span></span>](../resources/event.md) | <span data-ttu-id="603ab-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="603ab-125">Calendars.Read</span></span> | <span data-ttu-id="603ab-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="603ab-126">Calendars.Read</span></span> | <span data-ttu-id="603ab-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="603ab-127">Calendars.Read</span></span> |
|[<span data-ttu-id="603ab-128">grupo</span><span class="sxs-lookup"><span data-stu-id="603ab-128">group</span></span>](../resources/group.md) | <span data-ttu-id="603ab-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="603ab-129">Group.Read.All</span></span> | <span data-ttu-id="603ab-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="603ab-130">Not supported</span></span> | <span data-ttu-id="603ab-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="603ab-131">Group.Read.All</span></span> |
|[<span data-ttu-id="603ab-132">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="603ab-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="603ab-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="603ab-133">Group.Read.All</span></span> | <span data-ttu-id="603ab-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="603ab-134">Not supported</span></span> | <span data-ttu-id="603ab-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="603ab-135">Not supported</span></span> |
|[<span data-ttu-id="603ab-136">mensagem</span><span class="sxs-lookup"><span data-stu-id="603ab-136">message</span></span>](../resources/message.md) | <span data-ttu-id="603ab-137">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="603ab-137">Mail.Read</span></span> | <span data-ttu-id="603ab-138">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="603ab-138">Mail.Read</span></span> | <span data-ttu-id="603ab-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="603ab-139">Mail.Read</span></span> |
|[<span data-ttu-id="603ab-140">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="603ab-140">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="603ab-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="603ab-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="603ab-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="603ab-142">Not supported</span></span> | <span data-ttu-id="603ab-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="603ab-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="603ab-144">Usuário</span><span class="sxs-lookup"><span data-stu-id="603ab-144">user</span></span>](../resources/user.md) | <span data-ttu-id="603ab-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="603ab-145">User.Read.All</span></span> | <span data-ttu-id="603ab-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="603ab-146">User.Read.All</span></span> | <span data-ttu-id="603ab-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="603ab-147">User.Read.All</span></span> |

> <span data-ttu-id="603ab-148">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="603ab-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="603ab-149">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="603ab-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="603ab-150">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="603ab-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="603ab-151">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="603ab-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="603ab-152">As notificações são enviadas pelos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outros objetos driveItem na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="603ab-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="603ab-153">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="603ab-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="603ab-154">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="603ab-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="603ab-155">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="603ab-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="603ab-156">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="603ab-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="603ab-157">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="603ab-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="603ab-158">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="603ab-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="603ab-159">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="603ab-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="603ab-160">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="603ab-160">Optional query parameters</span></span>

<span data-ttu-id="603ab-161">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="603ab-161">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="603ab-162">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="603ab-162">Request headers</span></span>

| <span data-ttu-id="603ab-163">Nome</span><span class="sxs-lookup"><span data-stu-id="603ab-163">Name</span></span>       | <span data-ttu-id="603ab-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="603ab-164">Type</span></span> | <span data-ttu-id="603ab-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="603ab-165">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="603ab-166">Autorização</span><span class="sxs-lookup"><span data-stu-id="603ab-166">Authorization</span></span>  | <span data-ttu-id="603ab-167">string</span><span class="sxs-lookup"><span data-stu-id="603ab-167">string</span></span>  | <span data-ttu-id="603ab-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="603ab-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="603ab-170">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="603ab-170">Request body</span></span>

<span data-ttu-id="603ab-171">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="603ab-171">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="603ab-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="603ab-172">Response</span></span>

<span data-ttu-id="603ab-173">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="603ab-173">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="603ab-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="603ab-174">Example</span></span>

##### <a name="request"></a><span data-ttu-id="603ab-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="603ab-175">Request</span></span>

<span data-ttu-id="603ab-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="603ab-176">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="603ab-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="603ab-177">Response</span></span>

<span data-ttu-id="603ab-178">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="603ab-178">Here is an example of the response.</span></span>
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
