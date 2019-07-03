---
title: Atualizar CalendarGroup
description: Use esta API para criar um novo CalendarGroup.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b6f34fa7dc2fa289dd2890a579b049c81f282c27
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460165"
---
# <a name="create-calendargroup"></a><span data-ttu-id="5d559-103">Atualizar CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="5d559-103">Create CalendarGroup</span></span>

<span data-ttu-id="5d559-104">Use esta API para criar um novo CalendarGroup.</span><span class="sxs-lookup"><span data-stu-id="5d559-104">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="5d559-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d559-105">Permissions</span></span>
<span data-ttu-id="5d559-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d559-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d559-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d559-108">Permission type</span></span>      | <span data-ttu-id="5d559-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d559-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d559-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d559-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5d559-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d559-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5d559-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d559-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d559-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d559-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5d559-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d559-114">Application</span></span> | <span data-ttu-id="5d559-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d559-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d559-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d559-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendarGroups
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="5d559-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d559-117">Request headers</span></span>
| <span data-ttu-id="5d559-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5d559-118">Header</span></span>       | <span data-ttu-id="5d559-119">Valor</span><span class="sxs-lookup"><span data-stu-id="5d559-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5d559-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d559-120">Authorization</span></span>  | <span data-ttu-id="5d559-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d559-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5d559-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d559-123">Content-Type</span></span>  | <span data-ttu-id="5d559-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5d559-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5d559-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d559-125">Request body</span></span>
<span data-ttu-id="5d559-126">No corpo da solicitação, forneça uma representação JSON do objeto [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="5d559-126">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5d559-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d559-127">Response</span></span>

<span data-ttu-id="5d559-128">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [CalendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d559-128">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d559-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d559-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d559-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d559-130">Request</span></span>
<span data-ttu-id="5d559-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d559-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5d559-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d559-132">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="5d559-133">C#</span><span class="sxs-lookup"><span data-stu-id="5d559-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendargroup-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5d559-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="5d559-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendargroup-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5d559-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5d559-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendargroup-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="5d559-136">No corpo da solicitação, forneça uma representação JSON do objeto [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="5d559-136">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5d559-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d559-137">Response</span></span>
<span data-ttu-id="5d559-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d559-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
