---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 7ff9d85f1befec3e96a76002a10788d7068bf8ab
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331294"
---
# <a name="delete-subscription"></a><span data-ttu-id="2a038-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="2a038-103">Delete subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a038-104">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="2a038-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a038-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2a038-105">Permissions</span></span>

<span data-ttu-id="2a038-106">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="2a038-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="2a038-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a038-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a038-108">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="2a038-108">Supported resource</span></span> | <span data-ttu-id="2a038-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a038-109">Delegated (work or school account)</span></span> | <span data-ttu-id="2a038-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a038-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a038-111">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a038-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="2a038-112">contato</span><span class="sxs-lookup"><span data-stu-id="2a038-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="2a038-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2a038-113">Contacts.Read</span></span> | <span data-ttu-id="2a038-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2a038-114">Contacts.Read</span></span> | <span data-ttu-id="2a038-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2a038-115">Contacts.Read</span></span> |
|<span data-ttu-id="2a038-116">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="2a038-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="2a038-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2a038-117">Not supported</span></span> | <span data-ttu-id="2a038-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a038-118">Files.ReadWrite</span></span> | <span data-ttu-id="2a038-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2a038-119">Not supported</span></span> |
|<span data-ttu-id="2a038-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="2a038-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="2a038-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a038-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="2a038-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2a038-122">Not supported</span></span> | <span data-ttu-id="2a038-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a038-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="2a038-124">evento</span><span class="sxs-lookup"><span data-stu-id="2a038-124">event</span></span>](../resources/event.md) | <span data-ttu-id="2a038-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2a038-125">Calendars.Read</span></span> | <span data-ttu-id="2a038-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2a038-126">Calendars.Read</span></span> | <span data-ttu-id="2a038-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2a038-127">Calendars.Read</span></span> |
|[<span data-ttu-id="2a038-128">grupo</span><span class="sxs-lookup"><span data-stu-id="2a038-128">group</span></span>](../resources/group.md) | <span data-ttu-id="2a038-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a038-129">Group.Read.All</span></span> | <span data-ttu-id="2a038-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2a038-130">Not supported</span></span> | <span data-ttu-id="2a038-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a038-131">Group.Read.All</span></span> |
|[<span data-ttu-id="2a038-132">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="2a038-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="2a038-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a038-133">Group.Read.All</span></span> | <span data-ttu-id="2a038-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2a038-134">Not supported</span></span> | <span data-ttu-id="2a038-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2a038-135">Not supported</span></span> |
|[<span data-ttu-id="2a038-136">list</span><span class="sxs-lookup"><span data-stu-id="2a038-136">list</span></span>](../resources/list.md) | <span data-ttu-id="2a038-137">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a038-137">Sites.ReadWrite.All</span></span> | <span data-ttu-id="2a038-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2a038-138">Not supported</span></span> | <span data-ttu-id="2a038-139">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a038-139">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="2a038-140">message</span><span class="sxs-lookup"><span data-stu-id="2a038-140">message</span></span>](../resources/message.md) | <span data-ttu-id="2a038-141">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2a038-141">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="2a038-142">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2a038-142">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="2a038-143">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2a038-143">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="2a038-144">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="2a038-144">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="2a038-145">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a038-145">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="2a038-146">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2a038-146">Not supported</span></span> | <span data-ttu-id="2a038-147">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a038-147">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="2a038-148">Usuário</span><span class="sxs-lookup"><span data-stu-id="2a038-148">user</span></span>](../resources/user.md) | <span data-ttu-id="2a038-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a038-149">User.Read.All</span></span> | <span data-ttu-id="2a038-150">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a038-150">User.Read.All</span></span> | <span data-ttu-id="2a038-151">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a038-151">User.Read.All</span></span> |

> <span data-ttu-id="2a038-152">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="2a038-152">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="2a038-153">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="2a038-153">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="2a038-154">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="2a038-154">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="2a038-155">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="2a038-155">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="2a038-156">As notificações são enviadas pelos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outros objetos driveItem na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="2a038-156">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="2a038-157">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="2a038-157">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="2a038-158">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="2a038-158">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="2a038-159">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="2a038-159">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="2a038-160">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="2a038-160">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="2a038-161">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="2a038-161">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="2a038-162">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="2a038-162">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="2a038-163">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a038-163">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2a038-164">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a038-164">Request headers</span></span>

| <span data-ttu-id="2a038-165">Nome</span><span class="sxs-lookup"><span data-stu-id="2a038-165">Name</span></span>       | <span data-ttu-id="2a038-166">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a038-166">Type</span></span> | <span data-ttu-id="2a038-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a038-167">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2a038-168">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a038-168">Authorization</span></span>  | <span data-ttu-id="2a038-169">string</span><span class="sxs-lookup"><span data-stu-id="2a038-169">string</span></span>  | <span data-ttu-id="2a038-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a038-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a038-172">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a038-172">Request body</span></span>

<span data-ttu-id="2a038-173">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2a038-173">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a038-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a038-174">Response</span></span>

<span data-ttu-id="2a038-175">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2a038-175">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2a038-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a038-176">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2a038-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a038-177">Request</span></span>

<span data-ttu-id="2a038-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a038-178">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2a038-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a038-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="2a038-180">C#</span><span class="sxs-lookup"><span data-stu-id="2a038-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a038-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a038-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a038-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a038-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2a038-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a038-183">Response</span></span>

<span data-ttu-id="2a038-184">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a038-184">Here is an example of the response.</span></span>
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
