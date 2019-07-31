---
title: Atualizar CalendarGroup
description: Use esta API para criar um novo CalendarGroup.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 802c76350af0e8e8a1811b3ef992cdf88bcda47d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987513"
---
# <a name="create-calendargroup"></a><span data-ttu-id="8029a-103">Atualizar CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="8029a-103">Create CalendarGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8029a-104">Use esta API para criar um novo CalendarGroup.</span><span class="sxs-lookup"><span data-stu-id="8029a-104">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="8029a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8029a-105">Permissions</span></span>
<span data-ttu-id="8029a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8029a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8029a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8029a-108">Permission type</span></span>      | <span data-ttu-id="8029a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8029a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8029a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8029a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8029a-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8029a-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8029a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8029a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8029a-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8029a-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8029a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8029a-114">Application</span></span> | <span data-ttu-id="8029a-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8029a-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8029a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8029a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendarGroups
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="8029a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8029a-117">Request headers</span></span>
| <span data-ttu-id="8029a-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8029a-118">Header</span></span>       | <span data-ttu-id="8029a-119">Valor</span><span class="sxs-lookup"><span data-stu-id="8029a-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8029a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8029a-120">Authorization</span></span>  | <span data-ttu-id="8029a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8029a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8029a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8029a-123">Content-Type</span></span>  | <span data-ttu-id="8029a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8029a-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8029a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8029a-125">Request body</span></span>
<span data-ttu-id="8029a-126">No corpo da solicitação, forneça uma representação JSON do objeto [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="8029a-126">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8029a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8029a-127">Response</span></span>

<span data-ttu-id="8029a-128">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [CalendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8029a-128">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8029a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8029a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8029a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8029a-130">Request</span></span>
<span data-ttu-id="8029a-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8029a-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8029a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8029a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendarGroups
Content-type: application/json
Content-length: 90

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8029a-133">C#</span><span class="sxs-lookup"><span data-stu-id="8029a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendargroup-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8029a-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="8029a-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendargroup-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8029a-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8029a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendargroup-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8029a-136">Java</span><span class="sxs-lookup"><span data-stu-id="8029a-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-calendargroup-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="8029a-137">No corpo da solicitação, forneça uma representação JSON do objeto [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="8029a-137">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8029a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8029a-138">Response</span></span>
<span data-ttu-id="8029a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8029a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
