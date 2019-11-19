---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: piotrci
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: ad49621da8bac1092678940e0255c395e7e8ea88
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704161"
---
# <a name="delete-subscription"></a><span data-ttu-id="2af38-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="2af38-103">Delete subscription</span></span>

<span data-ttu-id="2af38-104">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="2af38-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="2af38-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2af38-105">Permissions</span></span>

<span data-ttu-id="2af38-106">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="2af38-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="2af38-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2af38-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2af38-108">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="2af38-108">Supported resource</span></span> | <span data-ttu-id="2af38-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2af38-109">Delegated (work or school account)</span></span> | <span data-ttu-id="2af38-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2af38-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2af38-111">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2af38-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="2af38-112">contato</span><span class="sxs-lookup"><span data-stu-id="2af38-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="2af38-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2af38-113">Contacts.Read</span></span> | <span data-ttu-id="2af38-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2af38-114">Contacts.Read</span></span> | <span data-ttu-id="2af38-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2af38-115">Contacts.Read</span></span> |
|<span data-ttu-id="2af38-116">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="2af38-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="2af38-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2af38-117">Not supported</span></span> | <span data-ttu-id="2af38-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2af38-118">Files.ReadWrite</span></span> | <span data-ttu-id="2af38-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2af38-119">Not supported</span></span> |
|<span data-ttu-id="2af38-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="2af38-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="2af38-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af38-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="2af38-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2af38-122">Not supported</span></span> | <span data-ttu-id="2af38-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af38-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="2af38-124">evento</span><span class="sxs-lookup"><span data-stu-id="2af38-124">event</span></span>](../resources/event.md) | <span data-ttu-id="2af38-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2af38-125">Calendars.Read</span></span> | <span data-ttu-id="2af38-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2af38-126">Calendars.Read</span></span> | <span data-ttu-id="2af38-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2af38-127">Calendars.Read</span></span> |
|[<span data-ttu-id="2af38-128">grupo</span><span class="sxs-lookup"><span data-stu-id="2af38-128">group</span></span>](../resources/group.md) | <span data-ttu-id="2af38-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2af38-129">Group.Read.All</span></span> | <span data-ttu-id="2af38-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2af38-130">Not supported</span></span> | <span data-ttu-id="2af38-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2af38-131">Group.Read.All</span></span> |
|[<span data-ttu-id="2af38-132">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="2af38-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="2af38-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2af38-133">Group.Read.All</span></span> | <span data-ttu-id="2af38-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2af38-134">Not supported</span></span> | <span data-ttu-id="2af38-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2af38-135">Not supported</span></span> |
|[<span data-ttu-id="2af38-136">Mensagem</span><span class="sxs-lookup"><span data-stu-id="2af38-136">message</span></span>](../resources/message.md) | <span data-ttu-id="2af38-137">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="2af38-137">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="2af38-138">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="2af38-138">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="2af38-139">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="2af38-139">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="2af38-140">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="2af38-140">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="2af38-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af38-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="2af38-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2af38-142">Not supported</span></span> | <span data-ttu-id="2af38-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af38-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="2af38-144">Usuário</span><span class="sxs-lookup"><span data-stu-id="2af38-144">user</span></span>](../resources/user.md) | <span data-ttu-id="2af38-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2af38-145">User.Read.All</span></span> | <span data-ttu-id="2af38-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2af38-146">User.Read.All</span></span> | <span data-ttu-id="2af38-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2af38-147">User.Read.All</span></span> |

> <span data-ttu-id="2af38-148">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="2af38-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="2af38-149">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="2af38-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="2af38-150">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="2af38-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="2af38-151">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="2af38-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="2af38-152">As notificações são enviadas pelos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outros objetos driveItem na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="2af38-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="2af38-153">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="2af38-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="2af38-154">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="2af38-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="2af38-155">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="2af38-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="2af38-156">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="2af38-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="2af38-157">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="2af38-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="2af38-158">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="2af38-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="2af38-159">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2af38-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2af38-160">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2af38-160">Request headers</span></span>

| <span data-ttu-id="2af38-161">Nome</span><span class="sxs-lookup"><span data-stu-id="2af38-161">Name</span></span>       | <span data-ttu-id="2af38-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="2af38-162">Type</span></span> | <span data-ttu-id="2af38-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="2af38-163">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2af38-164">Autorização</span><span class="sxs-lookup"><span data-stu-id="2af38-164">Authorization</span></span>  | <span data-ttu-id="2af38-165">string</span><span class="sxs-lookup"><span data-stu-id="2af38-165">string</span></span>  | <span data-ttu-id="2af38-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2af38-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2af38-168">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2af38-168">Request body</span></span>

<span data-ttu-id="2af38-169">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2af38-169">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2af38-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="2af38-170">Response</span></span>

<span data-ttu-id="2af38-171">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2af38-171">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2af38-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2af38-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2af38-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2af38-173">Request</span></span>

<span data-ttu-id="2af38-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2af38-174">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2af38-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="2af38-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2af38-176">C#</span><span class="sxs-lookup"><span data-stu-id="2af38-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2af38-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2af38-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2af38-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2af38-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2af38-179">Java</span><span class="sxs-lookup"><span data-stu-id="2af38-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2af38-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="2af38-180">Response</span></span>

<span data-ttu-id="2af38-181">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2af38-181">Here is an example of the response.</span></span>
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
