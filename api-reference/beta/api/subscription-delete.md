---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 94553470bb19bfaccd1824631d183bb931ab0ea8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453111"
---
# <a name="delete-subscription"></a><span data-ttu-id="db5f7-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="db5f7-103">Delete subscription</span></span>

<span data-ttu-id="db5f7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="db5f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db5f7-105">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="db5f7-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="db5f7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="db5f7-106">Permissions</span></span>

<span data-ttu-id="db5f7-107">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="db5f7-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="db5f7-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db5f7-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db5f7-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="db5f7-109">Supported resource</span></span> | <span data-ttu-id="db5f7-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db5f7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="db5f7-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db5f7-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db5f7-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db5f7-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="db5f7-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="db5f7-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="db5f7-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="db5f7-114">Not supported</span></span> | <span data-ttu-id="db5f7-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="db5f7-115">Not supported</span></span> | <span data-ttu-id="db5f7-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="db5f7-116">CallRecords.Read.All</span></span>  |
|[<span data-ttu-id="db5f7-117">contato</span><span class="sxs-lookup"><span data-stu-id="db5f7-117">contact</span></span>](../resources/contact.md) | <span data-ttu-id="db5f7-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="db5f7-118">Contacts.Read</span></span> | <span data-ttu-id="db5f7-119">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="db5f7-119">Contacts.Read</span></span> | <span data-ttu-id="db5f7-120">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="db5f7-120">Contacts.Read</span></span> |
|<span data-ttu-id="db5f7-121">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="db5f7-121">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="db5f7-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="db5f7-122">Not supported</span></span> | <span data-ttu-id="db5f7-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db5f7-123">Files.ReadWrite</span></span> | <span data-ttu-id="db5f7-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="db5f7-124">Not supported</span></span> |
|<span data-ttu-id="db5f7-125">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="db5f7-125">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="db5f7-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db5f7-126">Files.ReadWrite.All</span></span> | <span data-ttu-id="db5f7-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="db5f7-127">Not supported</span></span> | <span data-ttu-id="db5f7-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db5f7-128">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="db5f7-129">evento</span><span class="sxs-lookup"><span data-stu-id="db5f7-129">event</span></span>](../resources/event.md) | <span data-ttu-id="db5f7-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="db5f7-130">Calendars.Read</span></span> | <span data-ttu-id="db5f7-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="db5f7-131">Calendars.Read</span></span> | <span data-ttu-id="db5f7-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="db5f7-132">Calendars.Read</span></span> |
|[<span data-ttu-id="db5f7-133">grupo</span><span class="sxs-lookup"><span data-stu-id="db5f7-133">group</span></span>](../resources/group.md) | <span data-ttu-id="db5f7-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="db5f7-134">Group.Read.All</span></span> | <span data-ttu-id="db5f7-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="db5f7-135">Not supported</span></span> | <span data-ttu-id="db5f7-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="db5f7-136">Group.Read.All</span></span> |
|[<span data-ttu-id="db5f7-137">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="db5f7-137">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="db5f7-138">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="db5f7-138">Group.Read.All</span></span> | <span data-ttu-id="db5f7-139">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="db5f7-139">Not supported</span></span> | <span data-ttu-id="db5f7-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="db5f7-140">Not supported</span></span> |
|[<span data-ttu-id="db5f7-141">list</span><span class="sxs-lookup"><span data-stu-id="db5f7-141">list</span></span>](../resources/list.md) | <span data-ttu-id="db5f7-142">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db5f7-142">Sites.ReadWrite.All</span></span> | <span data-ttu-id="db5f7-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="db5f7-143">Not supported</span></span> | <span data-ttu-id="db5f7-144">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db5f7-144">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="db5f7-145">message</span><span class="sxs-lookup"><span data-stu-id="db5f7-145">message</span></span>](../resources/message.md) | <span data-ttu-id="db5f7-146">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="db5f7-146">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="db5f7-147">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="db5f7-147">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="db5f7-148">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="db5f7-148">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="db5f7-149">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="db5f7-149">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="db5f7-150">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db5f7-150">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="db5f7-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="db5f7-151">Not supported</span></span> | <span data-ttu-id="db5f7-152">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db5f7-152">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="db5f7-153">Usuário</span><span class="sxs-lookup"><span data-stu-id="db5f7-153">user</span></span>](../resources/user.md) | <span data-ttu-id="db5f7-154">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="db5f7-154">User.Read.All</span></span> | <span data-ttu-id="db5f7-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="db5f7-155">User.Read.All</span></span> | <span data-ttu-id="db5f7-156">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="db5f7-156">User.Read.All</span></span> |

> <span data-ttu-id="db5f7-157">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="db5f7-157">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="db5f7-158">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="db5f7-158">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="db5f7-159">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="db5f7-159">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="db5f7-160">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="db5f7-160">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="db5f7-161">As notificações são enviadas pelos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outros objetos driveItem na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="db5f7-161">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="db5f7-162">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="db5f7-162">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="db5f7-163">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="db5f7-163">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="db5f7-164">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="db5f7-164">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="db5f7-165">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="db5f7-165">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="db5f7-166">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="db5f7-166">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="db5f7-167">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="db5f7-167">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="db5f7-168">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db5f7-168">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="db5f7-169">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db5f7-169">Request headers</span></span>

| <span data-ttu-id="db5f7-170">Nome</span><span class="sxs-lookup"><span data-stu-id="db5f7-170">Name</span></span>       | <span data-ttu-id="db5f7-171">Tipo</span><span class="sxs-lookup"><span data-stu-id="db5f7-171">Type</span></span> | <span data-ttu-id="db5f7-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="db5f7-172">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="db5f7-173">Autorização</span><span class="sxs-lookup"><span data-stu-id="db5f7-173">Authorization</span></span>  | <span data-ttu-id="db5f7-174">string</span><span class="sxs-lookup"><span data-stu-id="db5f7-174">string</span></span>  | <span data-ttu-id="db5f7-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db5f7-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db5f7-177">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db5f7-177">Request body</span></span>

<span data-ttu-id="db5f7-178">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="db5f7-178">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db5f7-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="db5f7-179">Response</span></span>

<span data-ttu-id="db5f7-180">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="db5f7-180">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="db5f7-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db5f7-181">Example</span></span>

##### <a name="request"></a><span data-ttu-id="db5f7-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db5f7-182">Request</span></span>

<span data-ttu-id="db5f7-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db5f7-183">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db5f7-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="db5f7-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="db5f7-185">C#</span><span class="sxs-lookup"><span data-stu-id="db5f7-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db5f7-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db5f7-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db5f7-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db5f7-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="db5f7-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="db5f7-188">Response</span></span>

<span data-ttu-id="db5f7-189">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db5f7-189">Here is an example of the response.</span></span>
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
