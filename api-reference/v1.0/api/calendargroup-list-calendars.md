---
title: Listar calendários
description: Recupera uma lista de calendários que pertencem a um grupo de calendários.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4b228fbeefeb345514874b9493c6768bab8621a3
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726498"
---
# <a name="list-calendars"></a><span data-ttu-id="86941-103">Listar calendários</span><span class="sxs-lookup"><span data-stu-id="86941-103">List calendars</span></span>

<span data-ttu-id="86941-104">Recupera uma lista de calendários que pertencem a um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="86941-104">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="86941-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="86941-105">Permissions</span></span>

<span data-ttu-id="86941-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86941-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="86941-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86941-108">Permission type</span></span>                        | <span data-ttu-id="86941-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86941-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="86941-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86941-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="86941-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="86941-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="86941-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86941-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86941-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="86941-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="86941-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86941-114">Application</span></span>                            | <span data-ttu-id="86941-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="86941-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="86941-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86941-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="86941-117">Um [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="86941-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="86941-118">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="86941-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="86941-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="86941-119">Optional query parameters</span></span>

<span data-ttu-id="86941-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="86941-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86941-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86941-121">Request headers</span></span>

| <span data-ttu-id="86941-122">Nome</span><span class="sxs-lookup"><span data-stu-id="86941-122">Name</span></span>          | <span data-ttu-id="86941-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="86941-123">Type</span></span>   | <span data-ttu-id="86941-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="86941-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="86941-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="86941-125">Authorization</span></span> | <span data-ttu-id="86941-126">string</span><span class="sxs-lookup"><span data-stu-id="86941-126">string</span></span> | <span data-ttu-id="86941-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86941-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86941-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86941-129">Request body</span></span>

<span data-ttu-id="86941-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86941-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86941-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="86941-131">Response</span></span>

<span data-ttu-id="86941-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86941-132">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86941-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86941-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="86941-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86941-134">Request</span></span>

<span data-ttu-id="86941-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86941-135">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="86941-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="86941-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendargroup_get_calendars"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="86941-137">C#</span><span class="sxs-lookup"><span data-stu-id="86941-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendargroup-get-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="86941-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86941-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendargroup-get-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="86941-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="86941-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendargroup-get-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="86941-140">Java</span><span class="sxs-lookup"><span data-stu-id="86941-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendargroup-get-calendars-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="86941-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="86941-141">Response</span></span>

<span data-ttu-id="86941-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86941-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 147

{
  "value": [
    {
      "name": "name-value",
      "color": {
      },
      "changeKey": "changeKey-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
