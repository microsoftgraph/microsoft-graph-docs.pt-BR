---
title: Obter calendarGroup
description: Recupera as propriedades e os relacionamentos de um objeto de grupo de calendários.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 3cc37dffaa7c98d8bb851429908c58b279f45bec
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443760"
---
# <a name="get-calendargroup"></a><span data-ttu-id="549e3-103">Obter calendarGroup</span><span class="sxs-lookup"><span data-stu-id="549e3-103">Get calendarGroup</span></span>

<span data-ttu-id="549e3-104">Recupera as propriedades e os relacionamentos de um objeto de grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="549e3-104">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="549e3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="549e3-105">Permissions</span></span>

<span data-ttu-id="549e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="549e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="549e3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="549e3-108">Permission type</span></span>                        | <span data-ttu-id="549e3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="549e3-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="549e3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="549e3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="549e3-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="549e3-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="549e3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="549e3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="549e3-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="549e3-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="549e3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="549e3-114">Application</span></span>                            | <span data-ttu-id="549e3-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="549e3-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="549e3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="549e3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="549e3-117">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="549e3-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="549e3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="549e3-118">Optional query parameters</span></span>

<span data-ttu-id="549e3-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="549e3-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="549e3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="549e3-120">Request headers</span></span>

| <span data-ttu-id="549e3-121">Nome</span><span class="sxs-lookup"><span data-stu-id="549e3-121">Name</span></span>          | <span data-ttu-id="549e3-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="549e3-122">Type</span></span>   | <span data-ttu-id="549e3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="549e3-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="549e3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="549e3-124">Authorization</span></span> | <span data-ttu-id="549e3-125">string</span><span class="sxs-lookup"><span data-stu-id="549e3-125">string</span></span> | <span data-ttu-id="549e3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="549e3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="549e3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="549e3-128">Request body</span></span>

<span data-ttu-id="549e3-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="549e3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="549e3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="549e3-130">Response</span></span>

<span data-ttu-id="549e3-131">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="549e3-131">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="549e3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="549e3-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="549e3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="549e3-133">Request</span></span>

<span data-ttu-id="549e3-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="549e3-134">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="549e3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="549e3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="549e3-136">C#</span><span class="sxs-lookup"><span data-stu-id="549e3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="549e3-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="549e3-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="549e3-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="549e3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="549e3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="549e3-139">Response</span></span>

<span data-ttu-id="549e3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="549e3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
