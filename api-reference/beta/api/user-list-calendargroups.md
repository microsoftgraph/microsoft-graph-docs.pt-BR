---
title: Listar calendarGroups
description: Obter os grupos de calendários do usuário.
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f53b92b5ee2c771910a6098374896b3b0808a3b9
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107771"
---
# <a name="list-calendargroups"></a><span data-ttu-id="f8db3-103">Listar calendarGroups</span><span class="sxs-lookup"><span data-stu-id="f8db3-103">List calendarGroups</span></span>

<span data-ttu-id="f8db3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8db3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8db3-105">Obter os grupos de calendários do usuário.</span><span class="sxs-lookup"><span data-stu-id="f8db3-105">Get the user's calendar groups.</span></span>
## <a name="permissions"></a><span data-ttu-id="f8db3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f8db3-106">Permissions</span></span>
<span data-ttu-id="f8db3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8db3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8db3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8db3-109">Permission type</span></span>      | <span data-ttu-id="f8db3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f8db3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8db3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8db3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f8db3-112">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8db3-112">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f8db3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8db3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8db3-114">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8db3-114">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f8db3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8db3-115">Application</span></span> | <span data-ttu-id="f8db3-116">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8db3-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8db3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8db3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups
GET /users/{id | userPrincipalName}/calendarGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f8db3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f8db3-118">Optional query parameters</span></span>
<span data-ttu-id="f8db3-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f8db3-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f8db3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8db3-120">Request headers</span></span>
| <span data-ttu-id="f8db3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8db3-121">Header</span></span>       | <span data-ttu-id="f8db3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f8db3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f8db3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8db3-123">Authorization</span></span>  | <span data-ttu-id="f8db3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8db3-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f8db3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f8db3-126">Content-Type</span></span>  | <span data-ttu-id="f8db3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f8db3-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f8db3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8db3-128">Request body</span></span>
<span data-ttu-id="f8db3-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f8db3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8db3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8db3-130">Response</span></span>

<span data-ttu-id="f8db3-131">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [CalendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8db3-131">If successful, this method returns a `200 OK` response code and collection of [CalendarGroup](../resources/calendargroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f8db3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8db3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f8db3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8db3-133">Request</span></span>
<span data-ttu-id="f8db3-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8db3-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f8db3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8db3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendargroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendarGroups
```
# <a name="c"></a>[<span data-ttu-id="f8db3-136">C#</span><span class="sxs-lookup"><span data-stu-id="f8db3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendargroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8db3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8db3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendargroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8db3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8db3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendargroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f8db3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8db3-139">Response</span></span>
<span data-ttu-id="f8db3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8db3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
