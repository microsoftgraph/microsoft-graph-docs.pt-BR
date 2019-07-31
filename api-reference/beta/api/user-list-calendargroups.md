---
title: Listar calendarGroups
description: Obter os grupos de calendários do usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 230bc066bd4d993e9112497f08f4f98c86216d3d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987697"
---
# <a name="list-calendargroups"></a><span data-ttu-id="b7a79-103">Listar calendarGroups</span><span class="sxs-lookup"><span data-stu-id="b7a79-103">List calendarGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7a79-104">Obter os grupos de calendários do usuário.</span><span class="sxs-lookup"><span data-stu-id="b7a79-104">Get the user's calendar groups.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7a79-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b7a79-105">Permissions</span></span>
<span data-ttu-id="b7a79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7a79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7a79-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7a79-108">Permission type</span></span>      | <span data-ttu-id="b7a79-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7a79-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7a79-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7a79-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b7a79-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7a79-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b7a79-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7a79-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7a79-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7a79-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b7a79-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7a79-114">Application</span></span> | <span data-ttu-id="b7a79-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7a79-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7a79-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7a79-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups
GET /users/{id | userPrincipalName}/calendarGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b7a79-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b7a79-117">Optional query parameters</span></span>
<span data-ttu-id="b7a79-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b7a79-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b7a79-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7a79-119">Request headers</span></span>
| <span data-ttu-id="b7a79-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b7a79-120">Header</span></span>       | <span data-ttu-id="b7a79-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b7a79-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b7a79-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7a79-122">Authorization</span></span>  | <span data-ttu-id="b7a79-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7a79-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b7a79-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b7a79-125">Content-Type</span></span>  | <span data-ttu-id="b7a79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b7a79-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b7a79-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7a79-127">Request body</span></span>
<span data-ttu-id="b7a79-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b7a79-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7a79-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7a79-129">Response</span></span>

<span data-ttu-id="b7a79-130">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [CalendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7a79-130">If successful, this method returns a `200 OK` response code and collection of [CalendarGroup](../resources/calendargroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b7a79-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7a79-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7a79-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7a79-132">Request</span></span>
<span data-ttu-id="b7a79-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7a79-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b7a79-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7a79-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendargroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendarGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b7a79-135">C#</span><span class="sxs-lookup"><span data-stu-id="b7a79-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendargroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b7a79-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="b7a79-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendargroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b7a79-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b7a79-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendargroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b7a79-138">Java</span><span class="sxs-lookup"><span data-stu-id="b7a79-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendargroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b7a79-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7a79-139">Response</span></span>
<span data-ttu-id="b7a79-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7a79-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 155

{
  "value": [
    {
      "name": "name-value",
      "classId": "classId-value",
      "changeKey": "changeKey-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List calendarGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
