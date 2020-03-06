---
title: Criar calendário
description: Use esta API para criar um novo calendário para um usuário.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c9084cfa69c967471307c6db7f45f5bdd2c7b772
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509000"
---
# <a name="create-calendar"></a><span data-ttu-id="36373-103">Criar calendário</span><span class="sxs-lookup"><span data-stu-id="36373-103">Create Calendar</span></span>

<span data-ttu-id="36373-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36373-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="36373-105">Use esta API para criar um novo Calendar para um [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="36373-105">Use this API to create a new calendar for a [user](../resources/user.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="36373-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="36373-106">Permissions</span></span>
<span data-ttu-id="36373-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36373-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36373-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36373-109">Permission type</span></span>      | <span data-ttu-id="36373-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36373-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36373-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36373-111">Delegated (work or school account)</span></span> | <span data-ttu-id="36373-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36373-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="36373-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36373-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36373-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36373-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="36373-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36373-115">Application</span></span> | <span data-ttu-id="36373-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36373-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="36373-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36373-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="36373-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36373-118">Request headers</span></span>
| <span data-ttu-id="36373-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="36373-119">Header</span></span>       | <span data-ttu-id="36373-120">Valor</span><span class="sxs-lookup"><span data-stu-id="36373-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="36373-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="36373-121">Authorization</span></span>  | <span data-ttu-id="36373-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36373-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="36373-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="36373-124">Content-Type</span></span>  | <span data-ttu-id="36373-125">application/json</span><span class="sxs-lookup"><span data-stu-id="36373-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="36373-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36373-126">Request body</span></span>
<span data-ttu-id="36373-127">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="36373-127">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="36373-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="36373-128">Response</span></span>

<span data-ttu-id="36373-129">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36373-129">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36373-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36373-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36373-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36373-131">Request</span></span>
<span data-ttu-id="36373-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36373-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="36373-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="36373-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars
Content-type: application/json

{
  "name": "Volunteer"
}
```
# <a name="c"></a>[<span data-ttu-id="36373-134">C#</span><span class="sxs-lookup"><span data-stu-id="36373-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendar-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36373-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36373-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendar-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36373-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36373-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendar-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36373-137">Java</span><span class="sxs-lookup"><span data-stu-id="36373-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-calendar-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="36373-138">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="36373-138">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="36373-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="36373-139">Response</span></span>
<span data-ttu-id="36373-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36373-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Volunteer",
    "color":"auto",
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
    "canShare":true,
    "canViewPrivateItems":true,
    "canEdit":true,
    "owner":{
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
