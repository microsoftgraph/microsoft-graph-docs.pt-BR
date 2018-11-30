---
title: Obter assinatura
description: Recupere as propriedades e os relacionamentos da uma assinatura.
ms.openlocfilehash: 5694015fe7e8cbf87b5d62f7ae4af35d1773532b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036328"
---
# <a name="get-subscription"></a><span data-ttu-id="b82fb-103">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="b82fb-103">Get subscription</span></span>

> <span data-ttu-id="b82fb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b82fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b82fb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b82fb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b82fb-106">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="b82fb-106">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="b82fb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b82fb-107">Permissions</span></span>

<span data-ttu-id="b82fb-p102">A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b82fb-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b82fb-110">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="b82fb-110">Resource type / Item</span></span>        | <span data-ttu-id="b82fb-111">Permissão</span><span class="sxs-lookup"><span data-stu-id="b82fb-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="b82fb-112">Contatos</span><span class="sxs-lookup"><span data-stu-id="b82fb-112">Contacts</span></span>                    | <span data-ttu-id="b82fb-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b82fb-113">Contacts.Read</span></span>       |
| <span data-ttu-id="b82fb-114">Conversas</span><span class="sxs-lookup"><span data-stu-id="b82fb-114">Conversations</span></span>               | <span data-ttu-id="b82fb-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b82fb-115">Group.Read.All</span></span>      |
| <span data-ttu-id="b82fb-116">Eventos</span><span class="sxs-lookup"><span data-stu-id="b82fb-116">Events</span></span>                      | <span data-ttu-id="b82fb-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b82fb-117">Calendars.Read</span></span>      |
| <span data-ttu-id="b82fb-118">Mensagens</span><span class="sxs-lookup"><span data-stu-id="b82fb-118">Messages</span></span>                    | <span data-ttu-id="b82fb-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b82fb-119">Mail.Read</span></span>           |
| <span data-ttu-id="b82fb-120">Grupos</span><span class="sxs-lookup"><span data-stu-id="b82fb-120">Groups</span></span>                      | <span data-ttu-id="b82fb-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b82fb-121">Group.Read.All</span></span>      |
| <span data-ttu-id="b82fb-122">Usuários</span><span class="sxs-lookup"><span data-stu-id="b82fb-122">Users</span></span>                       | <span data-ttu-id="b82fb-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b82fb-123">User.Read.All</span></span>       |
| <span data-ttu-id="b82fb-124">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="b82fb-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="b82fb-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b82fb-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="b82fb-126">Drives (conteúdo do SharePoint shared e unidades)</span><span class="sxs-lookup"><span data-stu-id="b82fb-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="b82fb-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b82fb-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="b82fb-128">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="b82fb-128">Security alert</span></span>              | <span data-ttu-id="b82fb-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b82fb-129">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="b82fb-130">***Observação:*** O ponto de extremidade /beta permite que as permissões de aplicativo para a maioria dos recursos.</span><span class="sxs-lookup"><span data-stu-id="b82fb-130">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="b82fb-131">Não há suporte para conversas em itens de raiz uma unidade OneDrive e de grupo com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b82fb-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="b82fb-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b82fb-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b82fb-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b82fb-133">Optional query parameters</span></span>

<span data-ttu-id="b82fb-134">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b82fb-134">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b82fb-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b82fb-135">Request headers</span></span>

| <span data-ttu-id="b82fb-136">Nome</span><span class="sxs-lookup"><span data-stu-id="b82fb-136">Name</span></span>       | <span data-ttu-id="b82fb-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="b82fb-137">Type</span></span> | <span data-ttu-id="b82fb-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="b82fb-138">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="b82fb-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="b82fb-139">Authorization</span></span>  | <span data-ttu-id="b82fb-140">string</span><span class="sxs-lookup"><span data-stu-id="b82fb-140">string</span></span>  | <span data-ttu-id="b82fb-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b82fb-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b82fb-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b82fb-143">Request body</span></span>

<span data-ttu-id="b82fb-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b82fb-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b82fb-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b82fb-145">Response</span></span>

<span data-ttu-id="b82fb-146">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b82fb-146">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b82fb-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b82fb-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b82fb-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b82fb-148">Request</span></span>

<span data-ttu-id="b82fb-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b82fb-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="b82fb-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b82fb-150">Response</span></span>

<span data-ttu-id="b82fb-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b82fb-151">Here is an example of the response.</span></span>
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
