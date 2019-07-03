---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 50cd70ed1284b9ea165118db6af3141a6dadec6a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459885"
---
# <a name="delete-subscription"></a><span data-ttu-id="91b69-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="91b69-103">Delete subscription</span></span>

<span data-ttu-id="91b69-104">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="91b69-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="91b69-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="91b69-105">Permissions</span></span>

<span data-ttu-id="91b69-106">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="91b69-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="91b69-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91b69-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91b69-108">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="91b69-108">Supported resource</span></span> | <span data-ttu-id="91b69-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91b69-109">Delegated (work or school account)</span></span> | <span data-ttu-id="91b69-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91b69-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91b69-111">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91b69-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="91b69-112">contato</span><span class="sxs-lookup"><span data-stu-id="91b69-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="91b69-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="91b69-113">Contacts.Read</span></span> | <span data-ttu-id="91b69-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="91b69-114">Contacts.Read</span></span> | <span data-ttu-id="91b69-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="91b69-115">Contacts.Read</span></span> |
|<span data-ttu-id="91b69-116">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="91b69-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="91b69-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="91b69-117">Not supported</span></span> | <span data-ttu-id="91b69-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91b69-118">Files.ReadWrite</span></span> | <span data-ttu-id="91b69-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="91b69-119">Not supported</span></span> |
|<span data-ttu-id="91b69-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="91b69-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="91b69-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91b69-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="91b69-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="91b69-122">Not supported</span></span> | <span data-ttu-id="91b69-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91b69-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="91b69-124">evento</span><span class="sxs-lookup"><span data-stu-id="91b69-124">event</span></span>](../resources/event.md) | <span data-ttu-id="91b69-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="91b69-125">Calendars.Read</span></span> | <span data-ttu-id="91b69-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="91b69-126">Calendars.Read</span></span> | <span data-ttu-id="91b69-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="91b69-127">Calendars.Read</span></span> |
|[<span data-ttu-id="91b69-128">grupo</span><span class="sxs-lookup"><span data-stu-id="91b69-128">group</span></span>](../resources/group.md) | <span data-ttu-id="91b69-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="91b69-129">Group.Read.All</span></span> | <span data-ttu-id="91b69-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="91b69-130">Not supported</span></span> | <span data-ttu-id="91b69-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="91b69-131">Group.Read.All</span></span> |
|[<span data-ttu-id="91b69-132">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="91b69-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="91b69-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="91b69-133">Group.Read.All</span></span> | <span data-ttu-id="91b69-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="91b69-134">Not supported</span></span> | <span data-ttu-id="91b69-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="91b69-135">Not supported</span></span> |
|[<span data-ttu-id="91b69-136">mensagem</span><span class="sxs-lookup"><span data-stu-id="91b69-136">message</span></span>](../resources/message.md) | <span data-ttu-id="91b69-137">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="91b69-137">Mail.Read</span></span> | <span data-ttu-id="91b69-138">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="91b69-138">Mail.Read</span></span> | <span data-ttu-id="91b69-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="91b69-139">Mail.Read</span></span> |
|[<span data-ttu-id="91b69-140">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="91b69-140">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="91b69-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91b69-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="91b69-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="91b69-142">Not supported</span></span> | <span data-ttu-id="91b69-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91b69-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="91b69-144">Usuário</span><span class="sxs-lookup"><span data-stu-id="91b69-144">user</span></span>](../resources/user.md) | <span data-ttu-id="91b69-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="91b69-145">User.Read.All</span></span> | <span data-ttu-id="91b69-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="91b69-146">User.Read.All</span></span> | <span data-ttu-id="91b69-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="91b69-147">User.Read.All</span></span> |

> <span data-ttu-id="91b69-148">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="91b69-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="91b69-149">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="91b69-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="91b69-150">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="91b69-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="91b69-151">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="91b69-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="91b69-152">As notificações são enviadas pelos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outros objetos driveItem na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="91b69-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="91b69-153">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="91b69-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="91b69-154">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="91b69-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="91b69-155">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="91b69-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="91b69-156">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="91b69-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="91b69-157">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="91b69-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="91b69-158">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="91b69-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="91b69-159">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91b69-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="91b69-160">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91b69-160">Request headers</span></span>

| <span data-ttu-id="91b69-161">Nome</span><span class="sxs-lookup"><span data-stu-id="91b69-161">Name</span></span>       | <span data-ttu-id="91b69-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="91b69-162">Type</span></span> | <span data-ttu-id="91b69-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="91b69-163">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="91b69-164">Autorização</span><span class="sxs-lookup"><span data-stu-id="91b69-164">Authorization</span></span>  | <span data-ttu-id="91b69-165">string</span><span class="sxs-lookup"><span data-stu-id="91b69-165">string</span></span>  | <span data-ttu-id="91b69-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91b69-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91b69-168">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91b69-168">Request body</span></span>

<span data-ttu-id="91b69-169">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="91b69-169">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91b69-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="91b69-170">Response</span></span>

<span data-ttu-id="91b69-171">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="91b69-171">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="91b69-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91b69-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="91b69-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91b69-173">Request</span></span>

<span data-ttu-id="91b69-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91b69-174">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="91b69-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="91b69-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="91b69-176">C#</span><span class="sxs-lookup"><span data-stu-id="91b69-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="91b69-177">Javascript</span><span class="sxs-lookup"><span data-stu-id="91b69-177">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="91b69-178">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="91b69-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="91b69-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="91b69-179">Response</span></span>

<span data-ttu-id="91b69-180">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91b69-180">Here is an example of the response.</span></span>
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
