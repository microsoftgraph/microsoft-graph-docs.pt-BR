---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
ms.openlocfilehash: 63bcf8f4084053356819601cd6306ad3ff5238c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836117"
---
# <a name="update-subscription"></a><span data-ttu-id="5ca62-103">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="5ca62-103">Update subscription</span></span>

> <span data-ttu-id="5ca62-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5ca62-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ca62-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5ca62-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5ca62-106">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="5ca62-106">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="5ca62-107">Assinaturas expiram após um período de tempo que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="5ca62-107">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="5ca62-108">Para evitar notificações de ausentes, um aplicativo deve renovar suas assinaturas bem antes de começar sua data de expiração.</span><span class="sxs-lookup"><span data-stu-id="5ca62-108">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="5ca62-109">Consulte [assinatura](../resources/subscription.md) para o comprimento máximo de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="5ca62-109">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ca62-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ca62-110">Permissions</span></span>

<span data-ttu-id="5ca62-p103">A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ca62-p103">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5ca62-113">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="5ca62-113">Resource type / Item</span></span>        | <span data-ttu-id="5ca62-114">Permissão</span><span class="sxs-lookup"><span data-stu-id="5ca62-114">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="5ca62-115">Contatos</span><span class="sxs-lookup"><span data-stu-id="5ca62-115">Contacts</span></span>                    | <span data-ttu-id="5ca62-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5ca62-116">Contacts.Read</span></span>       |
| <span data-ttu-id="5ca62-117">Conversas</span><span class="sxs-lookup"><span data-stu-id="5ca62-117">Conversations</span></span>               | <span data-ttu-id="5ca62-118">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ca62-118">Group.Read.All</span></span>      |
| <span data-ttu-id="5ca62-119">Eventos</span><span class="sxs-lookup"><span data-stu-id="5ca62-119">Events</span></span>                      | <span data-ttu-id="5ca62-120">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5ca62-120">Calendars.Read</span></span>      |
| <span data-ttu-id="5ca62-121">Mensagens</span><span class="sxs-lookup"><span data-stu-id="5ca62-121">Messages</span></span>                    | <span data-ttu-id="5ca62-122">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5ca62-122">Mail.Read</span></span>           |
| <span data-ttu-id="5ca62-123">Grupos</span><span class="sxs-lookup"><span data-stu-id="5ca62-123">Groups</span></span>                      | <span data-ttu-id="5ca62-124">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ca62-124">Group.Read.All</span></span>      |
| <span data-ttu-id="5ca62-125">Usuários</span><span class="sxs-lookup"><span data-stu-id="5ca62-125">Users</span></span>                       | <span data-ttu-id="5ca62-126">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ca62-126">User.Read.All</span></span>       |
| <span data-ttu-id="5ca62-127">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="5ca62-127">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="5ca62-128">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ca62-128">Files.ReadWrite</span></span>     |
| <span data-ttu-id="5ca62-129">Drives (conteúdo do SharePoint shared e unidades)</span><span class="sxs-lookup"><span data-stu-id="5ca62-129">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="5ca62-130">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ca62-130">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="5ca62-131">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="5ca62-131">Security alert</span></span>               | <span data-ttu-id="5ca62-132">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ca62-132">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="5ca62-133">***Observação:*** O ponto de extremidade /beta permite que as permissões de aplicativo para a maioria dos recursos.</span><span class="sxs-lookup"><span data-stu-id="5ca62-133">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="5ca62-134">Não há suporte para conversas em itens de raiz uma unidade OneDrive e de grupo com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ca62-134">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="5ca62-135">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ca62-135">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5ca62-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca62-136">Request headers</span></span>

| <span data-ttu-id="5ca62-137">Nome</span><span class="sxs-lookup"><span data-stu-id="5ca62-137">Name</span></span>       | <span data-ttu-id="5ca62-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ca62-138">Type</span></span> | <span data-ttu-id="5ca62-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ca62-139">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5ca62-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ca62-140">Authorization</span></span>  | <span data-ttu-id="5ca62-141">string</span><span class="sxs-lookup"><span data-stu-id="5ca62-141">string</span></span>  | <span data-ttu-id="5ca62-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ca62-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5ca62-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ca62-144">Response</span></span>

<span data-ttu-id="5ca62-145">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ca62-145">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ca62-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ca62-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5ca62-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca62-147">Request</span></span>

<span data-ttu-id="5ca62-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ca62-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/beta/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="5ca62-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ca62-149">Response</span></span>

<span data-ttu-id="5ca62-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ca62-150">Here is an example of the response.</span></span>
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
  "clientState":"secretClientValue",
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
