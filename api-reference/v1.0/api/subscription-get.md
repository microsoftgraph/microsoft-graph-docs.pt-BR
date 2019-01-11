---
title: Obter assinatura
description: Recupere as propriedades e os relacionamentos da uma assinatura.
localization_priority: Priority
ms.openlocfilehash: a9cdc93d958895deaeb8778b69651a898d5a94c2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840296"
---
# <a name="get-subscription"></a><span data-ttu-id="9c1b9-103">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="9c1b9-103">Get subscription</span></span>

<span data-ttu-id="9c1b9-104">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="9c1b9-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c1b9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c1b9-105">Permissions</span></span>

<span data-ttu-id="9c1b9-p101">A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c1b9-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9c1b9-108">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="9c1b9-108">Resource type / Item</span></span>        | <span data-ttu-id="9c1b9-109">Permissão</span><span class="sxs-lookup"><span data-stu-id="9c1b9-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="9c1b9-110">Contatos</span><span class="sxs-lookup"><span data-stu-id="9c1b9-110">Contacts</span></span>                    | <span data-ttu-id="9c1b9-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9c1b9-111">Contacts.Read</span></span>       |
| <span data-ttu-id="9c1b9-112">Conversas</span><span class="sxs-lookup"><span data-stu-id="9c1b9-112">Conversations</span></span>               | <span data-ttu-id="9c1b9-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c1b9-113">Group.Read.All</span></span>      |
| <span data-ttu-id="9c1b9-114">Eventos</span><span class="sxs-lookup"><span data-stu-id="9c1b9-114">Events</span></span>                      | <span data-ttu-id="9c1b9-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9c1b9-115">Calendars.Read</span></span>      |
| <span data-ttu-id="9c1b9-116">Mensagens</span><span class="sxs-lookup"><span data-stu-id="9c1b9-116">Messages</span></span>                    | <span data-ttu-id="9c1b9-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9c1b9-117">Mail.Read</span></span>           |
| <span data-ttu-id="9c1b9-118">Grupos</span><span class="sxs-lookup"><span data-stu-id="9c1b9-118">Groups</span></span>                      | <span data-ttu-id="9c1b9-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c1b9-119">Group.Read.All</span></span>      |
| <span data-ttu-id="9c1b9-120">Usuários</span><span class="sxs-lookup"><span data-stu-id="9c1b9-120">Users</span></span>                       | <span data-ttu-id="9c1b9-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c1b9-121">User.Read.All</span></span>       |
| <span data-ttu-id="9c1b9-122">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="9c1b9-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="9c1b9-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c1b9-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="9c1b9-124">Drives (conteúdo do SharePoint shared e unidades)</span><span class="sxs-lookup"><span data-stu-id="9c1b9-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="9c1b9-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c1b9-125">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="9c1b9-126">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="9c1b9-126">Security alert</span></span>| <span data-ttu-id="9c1b9-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c1b9-127">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c1b9-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c1b9-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9c1b9-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9c1b9-129">Optional query parameters</span></span>

<span data-ttu-id="9c1b9-130">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9c1b9-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c1b9-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c1b9-131">Request headers</span></span>

| <span data-ttu-id="9c1b9-132">Nome</span><span class="sxs-lookup"><span data-stu-id="9c1b9-132">Name</span></span>       | <span data-ttu-id="9c1b9-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c1b9-133">Type</span></span> | <span data-ttu-id="9c1b9-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c1b9-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9c1b9-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c1b9-135">Authorization</span></span>  | <span data-ttu-id="9c1b9-136">string</span><span class="sxs-lookup"><span data-stu-id="9c1b9-136">string</span></span>  | <span data-ttu-id="9c1b9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c1b9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c1b9-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c1b9-139">Request body</span></span>

<span data-ttu-id="9c1b9-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9c1b9-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c1b9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c1b9-141">Response</span></span>

<span data-ttu-id="9c1b9-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c1b9-142">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c1b9-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c1b9-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9c1b9-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c1b9-144">Request</span></span>

<span data-ttu-id="9c1b9-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c1b9-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="9c1b9-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c1b9-146">Response</span></span>

<span data-ttu-id="9c1b9-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c1b9-147">Here is an example of the response.</span></span>
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
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
