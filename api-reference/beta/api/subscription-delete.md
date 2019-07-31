---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: piotrci
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: d5085f616d386d6fc9438b163b13173d19cfcfe1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977791"
---
# <a name="delete-subscription"></a><span data-ttu-id="a8185-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="a8185-103">Delete subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8185-104">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="a8185-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8185-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8185-105">Permissions</span></span>

<span data-ttu-id="a8185-106">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="a8185-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="a8185-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8185-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a8185-108">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="a8185-108">Supported resource</span></span> | <span data-ttu-id="a8185-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8185-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a8185-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8185-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8185-111">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8185-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="a8185-112">contato</span><span class="sxs-lookup"><span data-stu-id="a8185-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="a8185-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a8185-113">Contacts.Read</span></span> | <span data-ttu-id="a8185-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a8185-114">Contacts.Read</span></span> | <span data-ttu-id="a8185-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a8185-115">Contacts.Read</span></span> |
|<span data-ttu-id="a8185-116">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="a8185-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="a8185-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a8185-117">Not supported</span></span> | <span data-ttu-id="a8185-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8185-118">Files.ReadWrite</span></span> | <span data-ttu-id="a8185-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a8185-119">Not supported</span></span> |
|<span data-ttu-id="a8185-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="a8185-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="a8185-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8185-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="a8185-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a8185-122">Not supported</span></span> | <span data-ttu-id="a8185-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8185-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="a8185-124">evento</span><span class="sxs-lookup"><span data-stu-id="a8185-124">event</span></span>](../resources/event.md) | <span data-ttu-id="a8185-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a8185-125">Calendars.Read</span></span> | <span data-ttu-id="a8185-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a8185-126">Calendars.Read</span></span> | <span data-ttu-id="a8185-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a8185-127">Calendars.Read</span></span> |
|[<span data-ttu-id="a8185-128">grupo</span><span class="sxs-lookup"><span data-stu-id="a8185-128">group</span></span>](../resources/group.md) | <span data-ttu-id="a8185-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8185-129">Group.Read.All</span></span> | <span data-ttu-id="a8185-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a8185-130">Not supported</span></span> | <span data-ttu-id="a8185-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8185-131">Group.Read.All</span></span> |
|[<span data-ttu-id="a8185-132">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="a8185-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="a8185-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8185-133">Group.Read.All</span></span> | <span data-ttu-id="a8185-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a8185-134">Not supported</span></span> | <span data-ttu-id="a8185-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a8185-135">Not supported</span></span> |
|[<span data-ttu-id="a8185-136">mensagem</span><span class="sxs-lookup"><span data-stu-id="a8185-136">message</span></span>](../resources/message.md) | <span data-ttu-id="a8185-137">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a8185-137">Mail.Read</span></span> | <span data-ttu-id="a8185-138">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a8185-138">Mail.Read</span></span> | <span data-ttu-id="a8185-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a8185-139">Mail.Read</span></span> |
|[<span data-ttu-id="a8185-140">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="a8185-140">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="a8185-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8185-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="a8185-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a8185-142">Not supported</span></span> | <span data-ttu-id="a8185-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8185-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="a8185-144">Usuário</span><span class="sxs-lookup"><span data-stu-id="a8185-144">user</span></span>](../resources/user.md) | <span data-ttu-id="a8185-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8185-145">User.Read.All</span></span> | <span data-ttu-id="a8185-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8185-146">User.Read.All</span></span> | <span data-ttu-id="a8185-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8185-147">User.Read.All</span></span> |

> <span data-ttu-id="a8185-148">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="a8185-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="a8185-149">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="a8185-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="a8185-150">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="a8185-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="a8185-151">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="a8185-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="a8185-152">As notificações são enviadas pelos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outros objetos driveItem na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="a8185-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="a8185-153">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="a8185-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="a8185-154">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="a8185-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="a8185-155">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="a8185-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="a8185-156">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="a8185-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="a8185-157">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="a8185-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="a8185-158">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="a8185-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="a8185-159">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8185-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a8185-160">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8185-160">Request headers</span></span>

| <span data-ttu-id="a8185-161">Nome</span><span class="sxs-lookup"><span data-stu-id="a8185-161">Name</span></span>       | <span data-ttu-id="a8185-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8185-162">Type</span></span> | <span data-ttu-id="a8185-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8185-163">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a8185-164">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8185-164">Authorization</span></span>  | <span data-ttu-id="a8185-165">string</span><span class="sxs-lookup"><span data-stu-id="a8185-165">string</span></span>  | <span data-ttu-id="a8185-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8185-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8185-168">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8185-168">Request body</span></span>

<span data-ttu-id="a8185-169">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a8185-169">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8185-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8185-170">Response</span></span>

<span data-ttu-id="a8185-171">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a8185-171">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a8185-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8185-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a8185-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8185-173">Request</span></span>

<span data-ttu-id="a8185-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8185-174">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a8185-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8185-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a8185-176">C#</span><span class="sxs-lookup"><span data-stu-id="a8185-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8185-177">Javascript</span><span class="sxs-lookup"><span data-stu-id="a8185-177">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a8185-178">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a8185-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a8185-179">Java</span><span class="sxs-lookup"><span data-stu-id="a8185-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a8185-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8185-180">Response</span></span>

<span data-ttu-id="a8185-181">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8185-181">Here is an example of the response.</span></span>
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
