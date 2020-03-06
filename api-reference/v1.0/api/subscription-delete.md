---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: b74046ae383f6744f13b4309884557a4d38db2be
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509749"
---
# <a name="delete-subscription"></a><span data-ttu-id="ff65e-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="ff65e-103">Delete subscription</span></span>

<span data-ttu-id="ff65e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff65e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ff65e-105">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="ff65e-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff65e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff65e-106">Permissions</span></span>

<span data-ttu-id="ff65e-107">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="ff65e-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="ff65e-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff65e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ff65e-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="ff65e-109">Supported resource</span></span> | <span data-ttu-id="ff65e-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff65e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ff65e-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff65e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff65e-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff65e-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="ff65e-113">contato</span><span class="sxs-lookup"><span data-stu-id="ff65e-113">contact</span></span>](../resources/contact.md) | <span data-ttu-id="ff65e-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ff65e-114">Contacts.Read</span></span> | <span data-ttu-id="ff65e-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ff65e-115">Contacts.Read</span></span> | <span data-ttu-id="ff65e-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ff65e-116">Contacts.Read</span></span> |
|<span data-ttu-id="ff65e-117">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="ff65e-117">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="ff65e-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ff65e-118">Not supported</span></span> | <span data-ttu-id="ff65e-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff65e-119">Files.ReadWrite</span></span> | <span data-ttu-id="ff65e-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ff65e-120">Not supported</span></span> |
|<span data-ttu-id="ff65e-121">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="ff65e-121">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="ff65e-122">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff65e-122">Files.ReadWrite.All</span></span> | <span data-ttu-id="ff65e-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ff65e-123">Not supported</span></span> | <span data-ttu-id="ff65e-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff65e-124">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="ff65e-125">evento</span><span class="sxs-lookup"><span data-stu-id="ff65e-125">event</span></span>](../resources/event.md) | <span data-ttu-id="ff65e-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ff65e-126">Calendars.Read</span></span> | <span data-ttu-id="ff65e-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ff65e-127">Calendars.Read</span></span> | <span data-ttu-id="ff65e-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ff65e-128">Calendars.Read</span></span> |
|[<span data-ttu-id="ff65e-129">grupo</span><span class="sxs-lookup"><span data-stu-id="ff65e-129">group</span></span>](../resources/group.md) | <span data-ttu-id="ff65e-130">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff65e-130">Group.Read.All</span></span> | <span data-ttu-id="ff65e-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ff65e-131">Not supported</span></span> | <span data-ttu-id="ff65e-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff65e-132">Group.Read.All</span></span> |
|[<span data-ttu-id="ff65e-133">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="ff65e-133">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="ff65e-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff65e-134">Group.Read.All</span></span> | <span data-ttu-id="ff65e-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ff65e-135">Not supported</span></span> | <span data-ttu-id="ff65e-136">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ff65e-136">Not supported</span></span> |
|[<span data-ttu-id="ff65e-137">message</span><span class="sxs-lookup"><span data-stu-id="ff65e-137">message</span></span>](../resources/message.md) | <span data-ttu-id="ff65e-138">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ff65e-138">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="ff65e-139">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ff65e-139">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="ff65e-140">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ff65e-140">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="ff65e-141">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="ff65e-141">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="ff65e-142">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff65e-142">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="ff65e-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ff65e-143">Not supported</span></span> | <span data-ttu-id="ff65e-144">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff65e-144">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="ff65e-145">Usuário</span><span class="sxs-lookup"><span data-stu-id="ff65e-145">user</span></span>](../resources/user.md) | <span data-ttu-id="ff65e-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff65e-146">User.Read.All</span></span> | <span data-ttu-id="ff65e-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff65e-147">User.Read.All</span></span> | <span data-ttu-id="ff65e-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff65e-148">User.Read.All</span></span> |

> <span data-ttu-id="ff65e-149">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="ff65e-149">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="ff65e-150">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="ff65e-150">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="ff65e-151">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="ff65e-151">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="ff65e-152">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="ff65e-152">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="ff65e-153">As notificações são enviadas pelos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outros objetos driveItem na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="ff65e-153">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="ff65e-154">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="ff65e-154">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="ff65e-155">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="ff65e-155">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="ff65e-156">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="ff65e-156">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="ff65e-157">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="ff65e-157">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="ff65e-158">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="ff65e-158">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="ff65e-159">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="ff65e-159">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="ff65e-160">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff65e-160">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ff65e-161">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff65e-161">Request headers</span></span>

| <span data-ttu-id="ff65e-162">Nome</span><span class="sxs-lookup"><span data-stu-id="ff65e-162">Name</span></span>       | <span data-ttu-id="ff65e-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff65e-163">Type</span></span> | <span data-ttu-id="ff65e-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff65e-164">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ff65e-165">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff65e-165">Authorization</span></span>  | <span data-ttu-id="ff65e-166">string</span><span class="sxs-lookup"><span data-stu-id="ff65e-166">string</span></span>  | <span data-ttu-id="ff65e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff65e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff65e-169">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff65e-169">Request body</span></span>

<span data-ttu-id="ff65e-170">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ff65e-170">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff65e-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff65e-171">Response</span></span>

<span data-ttu-id="ff65e-172">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ff65e-172">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ff65e-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff65e-173">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ff65e-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff65e-174">Request</span></span>

<span data-ttu-id="ff65e-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff65e-175">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ff65e-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff65e-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="ff65e-177">C#</span><span class="sxs-lookup"><span data-stu-id="ff65e-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff65e-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff65e-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff65e-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff65e-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff65e-180">Java</span><span class="sxs-lookup"><span data-stu-id="ff65e-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ff65e-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff65e-181">Response</span></span>

<span data-ttu-id="ff65e-182">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff65e-182">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
