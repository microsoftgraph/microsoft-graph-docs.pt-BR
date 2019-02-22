---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 9fa5a60bbb00bb7d15ae14a0b76235a5629f2c42
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140450"
---
# <a name="delete-subscription"></a><span data-ttu-id="3ae8d-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="3ae8d-103">Delete subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ae8d-104">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="3ae8d-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ae8d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3ae8d-105">Permissions</span></span>

<span data-ttu-id="3ae8d-106">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o menos privilegiado necessário para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3ae8d-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="3ae8d-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ae8d-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ae8d-108">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="3ae8d-108">Supported resource</span></span> | <span data-ttu-id="3ae8d-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ae8d-109">Delegated (work or school account)</span></span> | <span data-ttu-id="3ae8d-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ae8d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ae8d-111">Application</span><span class="sxs-lookup"><span data-stu-id="3ae8d-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="3ae8d-112">contato</span><span class="sxs-lookup"><span data-stu-id="3ae8d-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="3ae8d-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3ae8d-113">Contacts.Read</span></span> | <span data-ttu-id="3ae8d-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3ae8d-114">Contacts.Read</span></span> | <span data-ttu-id="3ae8d-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3ae8d-115">Contacts.Read</span></span> |
|<span data-ttu-id="3ae8d-116">[driveItem](../resources/driveitem.md) (OneDrive pessoal do usuário)</span><span class="sxs-lookup"><span data-stu-id="3ae8d-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="3ae8d-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3ae8d-117">Not supported</span></span> | <span data-ttu-id="3ae8d-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ae8d-118">Files.ReadWrite</span></span> | <span data-ttu-id="3ae8d-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3ae8d-119">Not supported</span></span> |
|<span data-ttu-id="3ae8d-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="3ae8d-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="3ae8d-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ae8d-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="3ae8d-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3ae8d-122">Not supported</span></span> | <span data-ttu-id="3ae8d-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ae8d-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="3ae8d-124">event</span><span class="sxs-lookup"><span data-stu-id="3ae8d-124">event</span></span>](../resources/event.md) | <span data-ttu-id="3ae8d-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3ae8d-125">Calendars.Read</span></span> | <span data-ttu-id="3ae8d-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3ae8d-126">Calendars.Read</span></span> | <span data-ttu-id="3ae8d-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3ae8d-127">Calendars.Read</span></span> |
|[<span data-ttu-id="3ae8d-128">grupo</span><span class="sxs-lookup"><span data-stu-id="3ae8d-128">group</span></span>](../resources/group.md) | <span data-ttu-id="3ae8d-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ae8d-129">Group.Read.All</span></span> | <span data-ttu-id="3ae8d-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3ae8d-130">Not supported</span></span> | <span data-ttu-id="3ae8d-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ae8d-131">Group.Read.All</span></span> |
|[<span data-ttu-id="3ae8d-132">conversa de grupo</span><span class="sxs-lookup"><span data-stu-id="3ae8d-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="3ae8d-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ae8d-133">Group.Read.All</span></span> | <span data-ttu-id="3ae8d-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3ae8d-134">Not supported</span></span> | <span data-ttu-id="3ae8d-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3ae8d-135">Not supported</span></span> |
|[<span data-ttu-id="3ae8d-136">message</span><span class="sxs-lookup"><span data-stu-id="3ae8d-136">message</span></span>](../resources/message.md) | <span data-ttu-id="3ae8d-137">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3ae8d-137">Mail.Read</span></span> | <span data-ttu-id="3ae8d-138">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3ae8d-138">Mail.Read</span></span> | <span data-ttu-id="3ae8d-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3ae8d-139">Mail.Read</span></span> |
|[<span data-ttu-id="3ae8d-140">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="3ae8d-140">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="3ae8d-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ae8d-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="3ae8d-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3ae8d-142">Not supported</span></span> | <span data-ttu-id="3ae8d-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ae8d-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="3ae8d-144">user</span><span class="sxs-lookup"><span data-stu-id="3ae8d-144">user</span></span>](../resources/user.md) | <span data-ttu-id="3ae8d-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ae8d-145">User.Read.All</span></span> | <span data-ttu-id="3ae8d-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ae8d-146">User.Read.All</span></span> | <span data-ttu-id="3ae8d-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ae8d-147">User.Read.All</span></span> |

> <span data-ttu-id="3ae8d-148">**Observação:** Há limitações adicionais para assinaturas em itens do OneDrive e do Outlook.</span><span class="sxs-lookup"><span data-stu-id="3ae8d-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="3ae8d-149">As limitações se aplicam à criação e ao gerenciamento de assinaturas (obtendo, atualizando e excluindo assinaturas).</span><span class="sxs-lookup"><span data-stu-id="3ae8d-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="3ae8d-150">No OneDrive pessoal, você pode inscrever-se na pasta raiz ou em qualquer subpasta nessa unidade.</span><span class="sxs-lookup"><span data-stu-id="3ae8d-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="3ae8d-151">No OneDrive for Business, você pode inscrever-se apenas na pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="3ae8d-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="3ae8d-152">As notificações são enviadas para os tipos solicitados de alterações na pasta inscrita ou qualquer arquivo, pasta ou outro objeto driveItem em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="3ae8d-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="3ae8d-153">Você não pode se inscrever em instâncias de **unidade** ou **driveItem** que não são pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="3ae8d-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="3ae8d-154">No Outlook, a permissão delegada oferece suporte à assinatura de itens em pastas somente na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="3ae8d-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="3ae8d-155">Isso significa que, por exemplo, não é possível usar os calendários de permissão delegada. Leia para inscrever-se em eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="3ae8d-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="3ae8d-156">Para inscrever-se para alterar as notificações de contatos, eventos ou mensagens do Outlook em pastas compartilhadas _ou delegadas_ :</span><span class="sxs-lookup"><span data-stu-id="3ae8d-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="3ae8d-157">Use a permissão de aplicativo correspondente para inscrever-se nas alterações de itens em uma pasta ou em uma caixa de correio de _qualquer_ usuário no locatário.</span><span class="sxs-lookup"><span data-stu-id="3ae8d-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="3ae8d-158">Não use as permissões de compartilhamento do Outlook (Contacts. Read. Shared, caLendars. Read. Shared, mail. Read. Shared e suas contrapartes de leitura/gravação), já que eles **não** oferecem suporte à inscrição para alterar notificações em itens em pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="3ae8d-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="3ae8d-159">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ae8d-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3ae8d-160">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ae8d-160">Request headers</span></span>

| <span data-ttu-id="3ae8d-161">Nome</span><span class="sxs-lookup"><span data-stu-id="3ae8d-161">Name</span></span>       | <span data-ttu-id="3ae8d-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ae8d-162">Type</span></span> | <span data-ttu-id="3ae8d-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ae8d-163">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3ae8d-164">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ae8d-164">Authorization</span></span>  | <span data-ttu-id="3ae8d-165">string</span><span class="sxs-lookup"><span data-stu-id="3ae8d-165">string</span></span>  | <span data-ttu-id="3ae8d-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ae8d-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ae8d-168">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ae8d-168">Request body</span></span>

<span data-ttu-id="3ae8d-169">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3ae8d-169">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ae8d-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ae8d-170">Response</span></span>

<span data-ttu-id="3ae8d-171">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3ae8d-171">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3ae8d-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ae8d-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3ae8d-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ae8d-173">Request</span></span>

<span data-ttu-id="3ae8d-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ae8d-174">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="3ae8d-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ae8d-175">Response</span></span>

<span data-ttu-id="3ae8d-176">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ae8d-176">Here is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/subscription-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
