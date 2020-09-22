---
title: Atualizar CalendarGroup
description: Use esta API para criar um novo CalendarGroup.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4f6a13072727a31be56912bdaebe84bb251c697c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992010"
---
# <a name="create-calendargroup"></a><span data-ttu-id="fc5ee-103">Atualizar CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="fc5ee-103">Create CalendarGroup</span></span>

<span data-ttu-id="fc5ee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc5ee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fc5ee-105">Use esta API para criar um novo CalendarGroup.</span><span class="sxs-lookup"><span data-stu-id="fc5ee-105">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="fc5ee-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc5ee-106">Permissions</span></span>
<span data-ttu-id="fc5ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc5ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc5ee-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc5ee-109">Permission type</span></span>      | <span data-ttu-id="fc5ee-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc5ee-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc5ee-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc5ee-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fc5ee-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc5ee-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fc5ee-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc5ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc5ee-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc5ee-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fc5ee-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc5ee-115">Application</span></span> | <span data-ttu-id="fc5ee-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc5ee-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc5ee-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc5ee-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendarGroups
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="fc5ee-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc5ee-118">Request headers</span></span>
| <span data-ttu-id="fc5ee-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fc5ee-119">Header</span></span>       | <span data-ttu-id="fc5ee-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fc5ee-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fc5ee-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc5ee-121">Authorization</span></span>  | <span data-ttu-id="fc5ee-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc5ee-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fc5ee-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fc5ee-124">Content-Type</span></span>  | <span data-ttu-id="fc5ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fc5ee-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fc5ee-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc5ee-126">Request body</span></span>
<span data-ttu-id="fc5ee-127">No corpo da solicitação, forneça uma representação JSON do objeto [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="fc5ee-127">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fc5ee-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc5ee-128">Response</span></span>

<span data-ttu-id="fc5ee-129">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [CalendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc5ee-129">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc5ee-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc5ee-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc5ee-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc5ee-131">Request</span></span>
<span data-ttu-id="fc5ee-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc5ee-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fc5ee-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc5ee-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups
Content-type: application/json
Content-length: 90

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value"
}
```
# <a name="c"></a>[<span data-ttu-id="fc5ee-134">C#</span><span class="sxs-lookup"><span data-stu-id="fc5ee-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendargroup-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc5ee-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc5ee-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendargroup-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc5ee-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc5ee-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendargroup-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc5ee-137">Java</span><span class="sxs-lookup"><span data-stu-id="fc5ee-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-calendargroup-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="fc5ee-138">No corpo da solicitação, forneça uma representação JSON do objeto [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="fc5ee-138">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fc5ee-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc5ee-139">Response</span></span>
<span data-ttu-id="fc5ee-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc5ee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

