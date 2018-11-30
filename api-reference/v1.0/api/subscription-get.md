---
title: Obter assinatura
description: Recupere as propriedades e os relacionamentos da uma assinatura.
ms.openlocfilehash: 62bcb730a5743146113cda30d6dafa022afa4fc1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004887"
---
# <a name="get-subscription"></a><span data-ttu-id="97b3e-103">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="97b3e-103">Get subscription</span></span>

<span data-ttu-id="97b3e-104">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="97b3e-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="97b3e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="97b3e-105">Permissions</span></span>

<span data-ttu-id="97b3e-p101">A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97b3e-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97b3e-108">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="97b3e-108">Resource type / Item</span></span>        | <span data-ttu-id="97b3e-109">Permissão</span><span class="sxs-lookup"><span data-stu-id="97b3e-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="97b3e-110">Contatos</span><span class="sxs-lookup"><span data-stu-id="97b3e-110">Contacts</span></span>                    | <span data-ttu-id="97b3e-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="97b3e-111">Contacts.Read</span></span>       |
| <span data-ttu-id="97b3e-112">Conversas</span><span class="sxs-lookup"><span data-stu-id="97b3e-112">Conversations</span></span>               | <span data-ttu-id="97b3e-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="97b3e-113">Group.Read.All</span></span>      |
| <span data-ttu-id="97b3e-114">Eventos</span><span class="sxs-lookup"><span data-stu-id="97b3e-114">Events</span></span>                      | <span data-ttu-id="97b3e-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="97b3e-115">Calendars.Read</span></span>      |
| <span data-ttu-id="97b3e-116">Mensagens</span><span class="sxs-lookup"><span data-stu-id="97b3e-116">Messages</span></span>                    | <span data-ttu-id="97b3e-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="97b3e-117">Mail.Read</span></span>           |
| <span data-ttu-id="97b3e-118">Grupos</span><span class="sxs-lookup"><span data-stu-id="97b3e-118">Groups</span></span>                      | <span data-ttu-id="97b3e-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="97b3e-119">Group.Read.All</span></span>      |
| <span data-ttu-id="97b3e-120">Usuários</span><span class="sxs-lookup"><span data-stu-id="97b3e-120">Users</span></span>                       | <span data-ttu-id="97b3e-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="97b3e-121">User.Read.All</span></span>       |
| <span data-ttu-id="97b3e-122">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="97b3e-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="97b3e-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97b3e-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="97b3e-124">Drives (conteúdo do SharePoint shared e unidades)</span><span class="sxs-lookup"><span data-stu-id="97b3e-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="97b3e-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97b3e-125">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="97b3e-126">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="97b3e-126">Security alert</span></span>| <span data-ttu-id="97b3e-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97b3e-127">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97b3e-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97b3e-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="97b3e-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="97b3e-129">Optional query parameters</span></span>

<span data-ttu-id="97b3e-130">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="97b3e-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="97b3e-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97b3e-131">Request headers</span></span>

| <span data-ttu-id="97b3e-132">Nome</span><span class="sxs-lookup"><span data-stu-id="97b3e-132">Name</span></span>       | <span data-ttu-id="97b3e-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="97b3e-133">Type</span></span> | <span data-ttu-id="97b3e-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="97b3e-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="97b3e-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="97b3e-135">Authorization</span></span>  | <span data-ttu-id="97b3e-136">string</span><span class="sxs-lookup"><span data-stu-id="97b3e-136">string</span></span>  | <span data-ttu-id="97b3e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97b3e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97b3e-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97b3e-139">Request body</span></span>

<span data-ttu-id="97b3e-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97b3e-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97b3e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="97b3e-141">Response</span></span>

<span data-ttu-id="97b3e-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97b3e-142">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97b3e-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97b3e-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="97b3e-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97b3e-144">Request</span></span>

<span data-ttu-id="97b3e-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97b3e-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="97b3e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="97b3e-146">Response</span></span>

<span data-ttu-id="97b3e-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97b3e-147">Here is an example of the response.</span></span>
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
