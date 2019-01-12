---
title: Obter assinatura
description: Recupere as propriedades e os relacionamentos da uma assinatura.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 165fd990d7dbec64eb61b9e06d05b51b40bf1212
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934881"
---
# <a name="get-subscription"></a><span data-ttu-id="54e5f-103">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="54e5f-103">Get subscription</span></span>

> <span data-ttu-id="54e5f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="54e5f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54e5f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="54e5f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="54e5f-106">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="54e5f-106">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="54e5f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="54e5f-107">Permissions</span></span>

<span data-ttu-id="54e5f-p102">A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54e5f-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54e5f-110">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="54e5f-110">Resource type / Item</span></span>        | <span data-ttu-id="54e5f-111">Permissão</span><span class="sxs-lookup"><span data-stu-id="54e5f-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="54e5f-112">Contatos</span><span class="sxs-lookup"><span data-stu-id="54e5f-112">Contacts</span></span>                    | <span data-ttu-id="54e5f-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="54e5f-113">Contacts.Read</span></span>       |
| <span data-ttu-id="54e5f-114">Conversas</span><span class="sxs-lookup"><span data-stu-id="54e5f-114">Conversations</span></span>               | <span data-ttu-id="54e5f-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="54e5f-115">Group.Read.All</span></span>      |
| <span data-ttu-id="54e5f-116">Eventos</span><span class="sxs-lookup"><span data-stu-id="54e5f-116">Events</span></span>                      | <span data-ttu-id="54e5f-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="54e5f-117">Calendars.Read</span></span>      |
| <span data-ttu-id="54e5f-118">Mensagens</span><span class="sxs-lookup"><span data-stu-id="54e5f-118">Messages</span></span>                    | <span data-ttu-id="54e5f-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="54e5f-119">Mail.Read</span></span>           |
| <span data-ttu-id="54e5f-120">Grupos</span><span class="sxs-lookup"><span data-stu-id="54e5f-120">Groups</span></span>                      | <span data-ttu-id="54e5f-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="54e5f-121">Group.Read.All</span></span>      |
| <span data-ttu-id="54e5f-122">Usuários</span><span class="sxs-lookup"><span data-stu-id="54e5f-122">Users</span></span>                       | <span data-ttu-id="54e5f-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="54e5f-123">User.Read.All</span></span>       |
| <span data-ttu-id="54e5f-124">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="54e5f-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="54e5f-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="54e5f-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="54e5f-126">Drives (conteúdo do SharePoint shared e unidades)</span><span class="sxs-lookup"><span data-stu-id="54e5f-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="54e5f-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54e5f-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="54e5f-128">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="54e5f-128">Security alert</span></span>              | <span data-ttu-id="54e5f-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54e5f-129">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="54e5f-130">***Observação:*** O ponto de extremidade /beta permite que as permissões de aplicativo para a maioria dos recursos.</span><span class="sxs-lookup"><span data-stu-id="54e5f-130">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="54e5f-131">Não há suporte para conversas em itens de raiz uma unidade OneDrive e de grupo com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="54e5f-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="54e5f-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54e5f-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54e5f-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="54e5f-133">Optional query parameters</span></span>

<span data-ttu-id="54e5f-134">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="54e5f-134">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54e5f-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54e5f-135">Request headers</span></span>

| <span data-ttu-id="54e5f-136">Nome</span><span class="sxs-lookup"><span data-stu-id="54e5f-136">Name</span></span>       | <span data-ttu-id="54e5f-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="54e5f-137">Type</span></span> | <span data-ttu-id="54e5f-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="54e5f-138">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="54e5f-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="54e5f-139">Authorization</span></span>  | <span data-ttu-id="54e5f-140">string</span><span class="sxs-lookup"><span data-stu-id="54e5f-140">string</span></span>  | <span data-ttu-id="54e5f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54e5f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54e5f-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54e5f-143">Request body</span></span>

<span data-ttu-id="54e5f-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="54e5f-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54e5f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="54e5f-145">Response</span></span>

<span data-ttu-id="54e5f-146">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54e5f-146">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54e5f-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54e5f-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="54e5f-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54e5f-148">Request</span></span>

<span data-ttu-id="54e5f-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54e5f-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="54e5f-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="54e5f-150">Response</span></span>

<span data-ttu-id="54e5f-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54e5f-151">Here is an example of the response.</span></span>
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
