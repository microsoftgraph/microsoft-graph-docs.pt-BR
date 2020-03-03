---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 3328291435e3d6ce067b21a604d76ce46ee5ea2e
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394461"
---
# <a name="delete-subscription"></a><span data-ttu-id="da911-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="da911-103">Delete subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da911-104">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="da911-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="da911-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="da911-105">Permissions</span></span>

<span data-ttu-id="da911-106">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="da911-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="da911-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da911-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="da911-108">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="da911-108">Supported resource</span></span> | <span data-ttu-id="da911-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da911-109">Delegated (work or school account)</span></span> | <span data-ttu-id="da911-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da911-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da911-111">Application</span><span class="sxs-lookup"><span data-stu-id="da911-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="da911-112">callRecord</span><span class="sxs-lookup"><span data-stu-id="da911-112">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="da911-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="da911-113">Not supported</span></span> | <span data-ttu-id="da911-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="da911-114">Not supported</span></span> | <span data-ttu-id="da911-115">CallRecords. Read. All</span><span class="sxs-lookup"><span data-stu-id="da911-115">CallRecords.Read.All</span></span>  |
|[<span data-ttu-id="da911-116">contato</span><span class="sxs-lookup"><span data-stu-id="da911-116">contact</span></span>](../resources/contact.md) | <span data-ttu-id="da911-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="da911-117">Contacts.Read</span></span> | <span data-ttu-id="da911-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="da911-118">Contacts.Read</span></span> | <span data-ttu-id="da911-119">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="da911-119">Contacts.Read</span></span> |
|<span data-ttu-id="da911-120">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="da911-120">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="da911-121">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="da911-121">Not supported</span></span> | <span data-ttu-id="da911-122">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da911-122">Files.ReadWrite</span></span> | <span data-ttu-id="da911-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="da911-123">Not supported</span></span> |
|<span data-ttu-id="da911-124">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="da911-124">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="da911-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da911-125">Files.ReadWrite.All</span></span> | <span data-ttu-id="da911-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="da911-126">Not supported</span></span> | <span data-ttu-id="da911-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da911-127">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="da911-128">evento</span><span class="sxs-lookup"><span data-stu-id="da911-128">event</span></span>](../resources/event.md) | <span data-ttu-id="da911-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="da911-129">Calendars.Read</span></span> | <span data-ttu-id="da911-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="da911-130">Calendars.Read</span></span> | <span data-ttu-id="da911-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="da911-131">Calendars.Read</span></span> |
|[<span data-ttu-id="da911-132">grupo</span><span class="sxs-lookup"><span data-stu-id="da911-132">group</span></span>](../resources/group.md) | <span data-ttu-id="da911-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="da911-133">Group.Read.All</span></span> | <span data-ttu-id="da911-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="da911-134">Not supported</span></span> | <span data-ttu-id="da911-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="da911-135">Group.Read.All</span></span> |
|[<span data-ttu-id="da911-136">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="da911-136">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="da911-137">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="da911-137">Group.Read.All</span></span> | <span data-ttu-id="da911-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="da911-138">Not supported</span></span> | <span data-ttu-id="da911-139">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="da911-139">Not supported</span></span> |
|[<span data-ttu-id="da911-140">list</span><span class="sxs-lookup"><span data-stu-id="da911-140">list</span></span>](../resources/list.md) | <span data-ttu-id="da911-141">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da911-141">Sites.ReadWrite.All</span></span> | <span data-ttu-id="da911-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="da911-142">Not supported</span></span> | <span data-ttu-id="da911-143">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da911-143">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="da911-144">message</span><span class="sxs-lookup"><span data-stu-id="da911-144">message</span></span>](../resources/message.md) | <span data-ttu-id="da911-145">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="da911-145">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="da911-146">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="da911-146">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="da911-147">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="da911-147">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="da911-148">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="da911-148">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="da911-149">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da911-149">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="da911-150">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="da911-150">Not supported</span></span> | <span data-ttu-id="da911-151">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da911-151">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="da911-152">Usuário</span><span class="sxs-lookup"><span data-stu-id="da911-152">user</span></span>](../resources/user.md) | <span data-ttu-id="da911-153">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="da911-153">User.Read.All</span></span> | <span data-ttu-id="da911-154">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="da911-154">User.Read.All</span></span> | <span data-ttu-id="da911-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="da911-155">User.Read.All</span></span> |

> <span data-ttu-id="da911-156">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="da911-156">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="da911-157">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="da911-157">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="da911-158">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="da911-158">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="da911-159">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="da911-159">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="da911-160">As notificações são enviadas pelos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outros objetos driveItem na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="da911-160">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="da911-161">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="da911-161">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="da911-162">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="da911-162">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="da911-163">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="da911-163">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="da911-164">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="da911-164">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="da911-165">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="da911-165">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="da911-166">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="da911-166">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="da911-167">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da911-167">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="da911-168">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da911-168">Request headers</span></span>

| <span data-ttu-id="da911-169">Nome</span><span class="sxs-lookup"><span data-stu-id="da911-169">Name</span></span>       | <span data-ttu-id="da911-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="da911-170">Type</span></span> | <span data-ttu-id="da911-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="da911-171">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="da911-172">Autorização</span><span class="sxs-lookup"><span data-stu-id="da911-172">Authorization</span></span>  | <span data-ttu-id="da911-173">string</span><span class="sxs-lookup"><span data-stu-id="da911-173">string</span></span>  | <span data-ttu-id="da911-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da911-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da911-176">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da911-176">Request body</span></span>

<span data-ttu-id="da911-177">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da911-177">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da911-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="da911-178">Response</span></span>

<span data-ttu-id="da911-179">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="da911-179">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="da911-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da911-180">Example</span></span>

##### <a name="request"></a><span data-ttu-id="da911-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da911-181">Request</span></span>

<span data-ttu-id="da911-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da911-182">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="da911-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="da911-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="da911-184">C#</span><span class="sxs-lookup"><span data-stu-id="da911-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da911-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da911-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da911-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da911-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="da911-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="da911-187">Response</span></span>

<span data-ttu-id="da911-188">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da911-188">Here is an example of the response.</span></span>
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
