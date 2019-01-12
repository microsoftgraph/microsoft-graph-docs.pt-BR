---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: a980d1fdc50a3295a309ccb1d58c0ebf5b5b6133
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976629"
---
# <a name="update-subscription"></a><span data-ttu-id="a2b8a-103">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="a2b8a-103">Update subscription</span></span>

<span data-ttu-id="a2b8a-104">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="a2b8a-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="a2b8a-105">Assinaturas expiram após um período de tempo que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="a2b8a-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="a2b8a-106">Para evitar notificações de ausentes, um aplicativo deve renovar suas assinaturas bem antes de começar sua data de expiração.</span><span class="sxs-lookup"><span data-stu-id="a2b8a-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="a2b8a-107">Consulte [assinatura](../resources/subscription.md) para o comprimento máximo de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="a2b8a-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2b8a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2b8a-108">Permissions</span></span>

<span data-ttu-id="a2b8a-p102">A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2b8a-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a2b8a-111">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="a2b8a-111">Resource type / Item</span></span>        | <span data-ttu-id="a2b8a-112">Permissão</span><span class="sxs-lookup"><span data-stu-id="a2b8a-112">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="a2b8a-113">Contatos</span><span class="sxs-lookup"><span data-stu-id="a2b8a-113">Contacts</span></span>                    | <span data-ttu-id="a2b8a-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a2b8a-114">Contacts.Read</span></span>       |
| <span data-ttu-id="a2b8a-115">Conversas</span><span class="sxs-lookup"><span data-stu-id="a2b8a-115">Conversations</span></span>               | <span data-ttu-id="a2b8a-116">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2b8a-116">Group.Read.All</span></span>      |
| <span data-ttu-id="a2b8a-117">Eventos</span><span class="sxs-lookup"><span data-stu-id="a2b8a-117">Events</span></span>                      | <span data-ttu-id="a2b8a-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a2b8a-118">Calendars.Read</span></span>      |
| <span data-ttu-id="a2b8a-119">Mensagens</span><span class="sxs-lookup"><span data-stu-id="a2b8a-119">Messages</span></span>                    | <span data-ttu-id="a2b8a-120">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a2b8a-120">Mail.Read</span></span>           |
| <span data-ttu-id="a2b8a-121">Grupos</span><span class="sxs-lookup"><span data-stu-id="a2b8a-121">Groups</span></span>                      | <span data-ttu-id="a2b8a-122">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2b8a-122">Group.Read.All</span></span>      |
| <span data-ttu-id="a2b8a-123">Usuários</span><span class="sxs-lookup"><span data-stu-id="a2b8a-123">Users</span></span>                       | <span data-ttu-id="a2b8a-124">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2b8a-124">User.Read.All</span></span>       |
| <span data-ttu-id="a2b8a-125">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="a2b8a-125">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="a2b8a-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2b8a-126">Files.ReadWrite</span></span>     |
| <span data-ttu-id="a2b8a-127">Drives (conteúdo do SharePoint shared e unidades)</span><span class="sxs-lookup"><span data-stu-id="a2b8a-127">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="a2b8a-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2b8a-128">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="a2b8a-129">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="a2b8a-129">Security alert</span></span>| <span data-ttu-id="a2b8a-130">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2b8a-130">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2b8a-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2b8a-131">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a2b8a-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2b8a-132">Request headers</span></span>

| <span data-ttu-id="a2b8a-133">Nome</span><span class="sxs-lookup"><span data-stu-id="a2b8a-133">Name</span></span>       | <span data-ttu-id="a2b8a-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2b8a-134">Type</span></span> | <span data-ttu-id="a2b8a-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2b8a-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a2b8a-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2b8a-136">Authorization</span></span>  | <span data-ttu-id="a2b8a-137">string</span><span class="sxs-lookup"><span data-stu-id="a2b8a-137">string</span></span>  | <span data-ttu-id="a2b8a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2b8a-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a2b8a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2b8a-140">Response</span></span>

<span data-ttu-id="a2b8a-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2b8a-141">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2b8a-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2b8a-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a2b8a-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2b8a-143">Request</span></span>

<span data-ttu-id="a2b8a-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2b8a-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="a2b8a-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2b8a-145">Response</span></span>

<span data-ttu-id="a2b8a-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2b8a-146">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
