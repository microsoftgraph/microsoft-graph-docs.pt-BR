---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: f1f0dc151748d1f61f002f94243c13ce0f81c94b
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353174"
---
# <a name="delete-subscription"></a><span data-ttu-id="dd19b-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="dd19b-103">Delete subscription</span></span>

<span data-ttu-id="dd19b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd19b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd19b-105">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="dd19b-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd19b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd19b-106">Permissions</span></span>

<span data-ttu-id="dd19b-107">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="dd19b-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="dd19b-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd19b-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd19b-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="dd19b-109">Supported resource</span></span> | <span data-ttu-id="dd19b-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd19b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dd19b-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd19b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd19b-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd19b-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="dd19b-113">contato</span><span class="sxs-lookup"><span data-stu-id="dd19b-113">contact</span></span>](../resources/contact.md) | <span data-ttu-id="dd19b-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dd19b-114">Contacts.Read</span></span> | <span data-ttu-id="dd19b-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dd19b-115">Contacts.Read</span></span> | <span data-ttu-id="dd19b-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dd19b-116">Contacts.Read</span></span> |
|<span data-ttu-id="dd19b-117">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="dd19b-117">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="dd19b-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dd19b-118">Not supported</span></span> | <span data-ttu-id="dd19b-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd19b-119">Files.ReadWrite</span></span> | <span data-ttu-id="dd19b-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dd19b-120">Not supported</span></span> |
|<span data-ttu-id="dd19b-121">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="dd19b-121">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="dd19b-122">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd19b-122">Files.ReadWrite.All</span></span> | <span data-ttu-id="dd19b-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dd19b-123">Not supported</span></span> | <span data-ttu-id="dd19b-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd19b-124">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="dd19b-125">evento</span><span class="sxs-lookup"><span data-stu-id="dd19b-125">event</span></span>](../resources/event.md) | <span data-ttu-id="dd19b-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dd19b-126">Calendars.Read</span></span> | <span data-ttu-id="dd19b-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dd19b-127">Calendars.Read</span></span> | <span data-ttu-id="dd19b-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dd19b-128">Calendars.Read</span></span> |
|[<span data-ttu-id="dd19b-129">grupo</span><span class="sxs-lookup"><span data-stu-id="dd19b-129">group</span></span>](../resources/group.md) | <span data-ttu-id="dd19b-130">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd19b-130">Group.Read.All</span></span> | <span data-ttu-id="dd19b-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dd19b-131">Not supported</span></span> | <span data-ttu-id="dd19b-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd19b-132">Group.Read.All</span></span> |
|[<span data-ttu-id="dd19b-133">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="dd19b-133">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="dd19b-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd19b-134">Group.Read.All</span></span> | <span data-ttu-id="dd19b-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dd19b-135">Not supported</span></span> | <span data-ttu-id="dd19b-136">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dd19b-136">Not supported</span></span> |
|[<span data-ttu-id="dd19b-137">list</span><span class="sxs-lookup"><span data-stu-id="dd19b-137">list</span></span>](../resources/list.md) | <span data-ttu-id="dd19b-138">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd19b-138">Sites.ReadWrite.All</span></span> | <span data-ttu-id="dd19b-139">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dd19b-139">Not supported</span></span> | <span data-ttu-id="dd19b-140">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd19b-140">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="dd19b-141">message</span><span class="sxs-lookup"><span data-stu-id="dd19b-141">message</span></span>](../resources/message.md) | <span data-ttu-id="dd19b-142">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dd19b-142">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="dd19b-143">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dd19b-143">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="dd19b-144">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dd19b-144">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="dd19b-145">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="dd19b-145">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="dd19b-146">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd19b-146">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="dd19b-147">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dd19b-147">Not supported</span></span> | <span data-ttu-id="dd19b-148">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd19b-148">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="dd19b-149">Usuário</span><span class="sxs-lookup"><span data-stu-id="dd19b-149">user</span></span>](../resources/user.md) | <span data-ttu-id="dd19b-150">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd19b-150">User.Read.All</span></span> | <span data-ttu-id="dd19b-151">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd19b-151">User.Read.All</span></span> | <span data-ttu-id="dd19b-152">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd19b-152">User.Read.All</span></span> |

> <span data-ttu-id="dd19b-153">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="dd19b-153">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="dd19b-154">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="dd19b-154">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="dd19b-155">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="dd19b-155">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="dd19b-156">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="dd19b-156">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="dd19b-157">As notificações de alteração são enviadas para os tipos solicitados de alterações na pasta inscrita ou qualquer arquivo, pasta ou outro objeto driveItem em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="dd19b-157">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="dd19b-158">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="dd19b-158">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="dd19b-159">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="dd19b-159">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="dd19b-160">Isso significa que, por exemplo, você não pode usar os calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="dd19b-160">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="dd19b-161">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="dd19b-161">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="dd19b-162">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="dd19b-162">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="dd19b-163">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="dd19b-163">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="dd19b-164">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd19b-164">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dd19b-165">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd19b-165">Request headers</span></span>

| <span data-ttu-id="dd19b-166">Nome</span><span class="sxs-lookup"><span data-stu-id="dd19b-166">Name</span></span>       | <span data-ttu-id="dd19b-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd19b-167">Type</span></span> | <span data-ttu-id="dd19b-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd19b-168">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dd19b-169">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd19b-169">Authorization</span></span>  | <span data-ttu-id="dd19b-170">string</span><span class="sxs-lookup"><span data-stu-id="dd19b-170">string</span></span>  | <span data-ttu-id="dd19b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd19b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd19b-173">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd19b-173">Request body</span></span>

<span data-ttu-id="dd19b-174">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dd19b-174">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd19b-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd19b-175">Response</span></span>

<span data-ttu-id="dd19b-176">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dd19b-176">If successful, this method returns a `204 No Content` response code.</span></span>
<span data-ttu-id="dd19b-177">Para obter detalhes sobre como os erros são retornados, confira [respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="dd19b-177">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="dd19b-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd19b-178">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dd19b-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd19b-179">Request</span></span>

<span data-ttu-id="dd19b-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd19b-180">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd19b-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd19b-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="dd19b-182">C#</span><span class="sxs-lookup"><span data-stu-id="dd19b-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd19b-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd19b-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd19b-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd19b-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd19b-185">Java</span><span class="sxs-lookup"><span data-stu-id="dd19b-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dd19b-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd19b-186">Response</span></span>

<span data-ttu-id="dd19b-187">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd19b-187">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
