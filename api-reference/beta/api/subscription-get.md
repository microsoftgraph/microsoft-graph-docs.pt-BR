---
title: Obter assinatura
description: Recupere as propriedades e os relacionamentos da uma assinatura.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: c7dd20810cd9fdacec697345d42690f85bc3b8b1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522361"
---
# <a name="get-subscription"></a><span data-ttu-id="c3285-103">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="c3285-103">Get subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3285-104">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="c3285-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3285-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3285-105">Permissions</span></span>

<span data-ttu-id="c3285-p101">A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3285-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c3285-108">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="c3285-108">Resource type / Item</span></span>        | <span data-ttu-id="c3285-109">Permissão</span><span class="sxs-lookup"><span data-stu-id="c3285-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="c3285-110">Contatos</span><span class="sxs-lookup"><span data-stu-id="c3285-110">Contacts</span></span>                    | <span data-ttu-id="c3285-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c3285-111">Contacts.Read</span></span>       |
| <span data-ttu-id="c3285-112">Conversas</span><span class="sxs-lookup"><span data-stu-id="c3285-112">Conversations</span></span>               | <span data-ttu-id="c3285-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3285-113">Group.Read.All</span></span>      |
| <span data-ttu-id="c3285-114">Eventos</span><span class="sxs-lookup"><span data-stu-id="c3285-114">Events</span></span>                      | <span data-ttu-id="c3285-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c3285-115">Calendars.Read</span></span>      |
| <span data-ttu-id="c3285-116">Mensagens</span><span class="sxs-lookup"><span data-stu-id="c3285-116">Messages</span></span>                    | <span data-ttu-id="c3285-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c3285-117">Mail.Read</span></span>           |
| <span data-ttu-id="c3285-118">Grupos</span><span class="sxs-lookup"><span data-stu-id="c3285-118">Groups</span></span>                      | <span data-ttu-id="c3285-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3285-119">Group.Read.All</span></span>      |
| <span data-ttu-id="c3285-120">Usuários</span><span class="sxs-lookup"><span data-stu-id="c3285-120">Users</span></span>                       | <span data-ttu-id="c3285-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3285-121">User.Read.All</span></span>       |
| <span data-ttu-id="c3285-122">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="c3285-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="c3285-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3285-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="c3285-124">Drives (conteúdo do SharePoint shared e unidades)</span><span class="sxs-lookup"><span data-stu-id="c3285-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="c3285-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3285-125">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="c3285-126">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="c3285-126">Security alert</span></span>              | <span data-ttu-id="c3285-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3285-127">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="c3285-128">***Observação:*** O ponto de extremidade /beta permite que as permissões de aplicativo para a maioria dos recursos.</span><span class="sxs-lookup"><span data-stu-id="c3285-128">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="c3285-129">Não há suporte para conversas em itens de raiz uma unidade OneDrive e de grupo com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c3285-129">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="c3285-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3285-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c3285-131">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c3285-131">Optional query parameters</span></span>

<span data-ttu-id="c3285-132">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c3285-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3285-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3285-133">Request headers</span></span>

| <span data-ttu-id="c3285-134">Nome</span><span class="sxs-lookup"><span data-stu-id="c3285-134">Name</span></span>       | <span data-ttu-id="c3285-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3285-135">Type</span></span> | <span data-ttu-id="c3285-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3285-136">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="c3285-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3285-137">Authorization</span></span>  | <span data-ttu-id="c3285-138">string</span><span class="sxs-lookup"><span data-stu-id="c3285-138">string</span></span>  | <span data-ttu-id="c3285-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3285-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3285-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3285-141">Request body</span></span>

<span data-ttu-id="c3285-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c3285-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3285-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3285-143">Response</span></span>

<span data-ttu-id="c3285-144">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3285-144">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3285-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3285-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c3285-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3285-146">Request</span></span>

<span data-ttu-id="c3285-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3285-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="c3285-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3285-148">Response</span></span>

<span data-ttu-id="c3285-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3285-149">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
