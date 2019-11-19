---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: piotrci
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 381c816685129a7cfe7dda88050a96a9a78dca8b
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703697"
---
# <a name="delete-subscription"></a><span data-ttu-id="2cc00-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="2cc00-103">Delete subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cc00-104">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="2cc00-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="2cc00-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2cc00-105">Permissions</span></span>

<span data-ttu-id="2cc00-106">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="2cc00-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="2cc00-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cc00-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2cc00-108">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="2cc00-108">Supported resource</span></span> | <span data-ttu-id="2cc00-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2cc00-109">Delegated (work or school account)</span></span> | <span data-ttu-id="2cc00-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2cc00-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2cc00-111">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2cc00-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="2cc00-112">contato</span><span class="sxs-lookup"><span data-stu-id="2cc00-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="2cc00-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2cc00-113">Contacts.Read</span></span> | <span data-ttu-id="2cc00-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2cc00-114">Contacts.Read</span></span> | <span data-ttu-id="2cc00-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2cc00-115">Contacts.Read</span></span> |
|<span data-ttu-id="2cc00-116">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="2cc00-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="2cc00-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2cc00-117">Not supported</span></span> | <span data-ttu-id="2cc00-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2cc00-118">Files.ReadWrite</span></span> | <span data-ttu-id="2cc00-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2cc00-119">Not supported</span></span> |
|<span data-ttu-id="2cc00-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="2cc00-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="2cc00-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cc00-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="2cc00-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2cc00-122">Not supported</span></span> | <span data-ttu-id="2cc00-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cc00-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="2cc00-124">evento</span><span class="sxs-lookup"><span data-stu-id="2cc00-124">event</span></span>](../resources/event.md) | <span data-ttu-id="2cc00-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2cc00-125">Calendars.Read</span></span> | <span data-ttu-id="2cc00-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2cc00-126">Calendars.Read</span></span> | <span data-ttu-id="2cc00-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2cc00-127">Calendars.Read</span></span> |
|[<span data-ttu-id="2cc00-128">grupo</span><span class="sxs-lookup"><span data-stu-id="2cc00-128">group</span></span>](../resources/group.md) | <span data-ttu-id="2cc00-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2cc00-129">Group.Read.All</span></span> | <span data-ttu-id="2cc00-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2cc00-130">Not supported</span></span> | <span data-ttu-id="2cc00-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2cc00-131">Group.Read.All</span></span> |
|[<span data-ttu-id="2cc00-132">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="2cc00-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="2cc00-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2cc00-133">Group.Read.All</span></span> | <span data-ttu-id="2cc00-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2cc00-134">Not supported</span></span> | <span data-ttu-id="2cc00-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2cc00-135">Not supported</span></span> |
|[<span data-ttu-id="2cc00-136">Mensagem</span><span class="sxs-lookup"><span data-stu-id="2cc00-136">message</span></span>](../resources/message.md) | <span data-ttu-id="2cc00-137">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="2cc00-137">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="2cc00-138">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="2cc00-138">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="2cc00-139">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="2cc00-139">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="2cc00-140">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="2cc00-140">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="2cc00-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cc00-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="2cc00-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2cc00-142">Not supported</span></span> | <span data-ttu-id="2cc00-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cc00-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="2cc00-144">Usuário</span><span class="sxs-lookup"><span data-stu-id="2cc00-144">user</span></span>](../resources/user.md) | <span data-ttu-id="2cc00-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2cc00-145">User.Read.All</span></span> | <span data-ttu-id="2cc00-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2cc00-146">User.Read.All</span></span> | <span data-ttu-id="2cc00-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2cc00-147">User.Read.All</span></span> |

> <span data-ttu-id="2cc00-148">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="2cc00-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="2cc00-149">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="2cc00-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="2cc00-150">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="2cc00-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="2cc00-151">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="2cc00-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="2cc00-152">As notificações são enviadas pelos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outros objetos driveItem na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="2cc00-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="2cc00-153">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="2cc00-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="2cc00-154">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="2cc00-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="2cc00-155">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="2cc00-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="2cc00-156">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="2cc00-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="2cc00-157">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="2cc00-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="2cc00-158">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="2cc00-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="2cc00-159">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2cc00-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2cc00-160">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2cc00-160">Request headers</span></span>

| <span data-ttu-id="2cc00-161">Nome</span><span class="sxs-lookup"><span data-stu-id="2cc00-161">Name</span></span>       | <span data-ttu-id="2cc00-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="2cc00-162">Type</span></span> | <span data-ttu-id="2cc00-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cc00-163">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2cc00-164">Autorização</span><span class="sxs-lookup"><span data-stu-id="2cc00-164">Authorization</span></span>  | <span data-ttu-id="2cc00-165">string</span><span class="sxs-lookup"><span data-stu-id="2cc00-165">string</span></span>  | <span data-ttu-id="2cc00-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2cc00-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2cc00-168">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2cc00-168">Request body</span></span>

<span data-ttu-id="2cc00-169">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2cc00-169">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2cc00-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cc00-170">Response</span></span>

<span data-ttu-id="2cc00-171">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2cc00-171">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2cc00-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2cc00-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2cc00-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2cc00-173">Request</span></span>

<span data-ttu-id="2cc00-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2cc00-174">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2cc00-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="2cc00-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2cc00-176">C#</span><span class="sxs-lookup"><span data-stu-id="2cc00-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2cc00-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2cc00-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2cc00-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2cc00-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2cc00-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cc00-179">Response</span></span>

<span data-ttu-id="2cc00-180">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2cc00-180">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
