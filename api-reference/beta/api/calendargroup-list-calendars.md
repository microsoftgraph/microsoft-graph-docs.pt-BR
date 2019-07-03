---
title: Listar calendários
description: Recupera uma lista de calendários que pertencem a um grupo de calendários.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: fc9bef43093bbcb301ec17f3c6d12da0552cf055
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438843"
---
# <a name="list-calendars"></a><span data-ttu-id="f25bc-103">Listar calendários</span><span class="sxs-lookup"><span data-stu-id="f25bc-103">List calendars</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f25bc-104">Recupera uma lista de calendários que pertencem a um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="f25bc-104">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="f25bc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f25bc-105">Permissions</span></span>

<span data-ttu-id="f25bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f25bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f25bc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f25bc-108">Permission type</span></span>                        | <span data-ttu-id="f25bc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f25bc-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f25bc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f25bc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f25bc-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f25bc-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="f25bc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f25bc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f25bc-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f25bc-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="f25bc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f25bc-114">Application</span></span>                            | <span data-ttu-id="f25bc-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f25bc-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="f25bc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f25bc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="f25bc-117">Um [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="f25bc-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="f25bc-118">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f25bc-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f25bc-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f25bc-119">Optional query parameters</span></span>

<span data-ttu-id="f25bc-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f25bc-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f25bc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f25bc-121">Request headers</span></span>

| <span data-ttu-id="f25bc-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f25bc-122">Name</span></span>          | <span data-ttu-id="f25bc-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f25bc-123">Type</span></span>   | <span data-ttu-id="f25bc-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f25bc-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="f25bc-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f25bc-125">Authorization</span></span> | <span data-ttu-id="f25bc-126">string</span><span class="sxs-lookup"><span data-stu-id="f25bc-126">string</span></span> | <span data-ttu-id="f25bc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f25bc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f25bc-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f25bc-129">Request body</span></span>

<span data-ttu-id="f25bc-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f25bc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f25bc-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f25bc-131">Response</span></span>

<span data-ttu-id="f25bc-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f25bc-132">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f25bc-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f25bc-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f25bc-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f25bc-134">Request</span></span>

<span data-ttu-id="f25bc-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f25bc-135">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f25bc-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f25bc-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f25bc-137">C#</span><span class="sxs-lookup"><span data-stu-id="f25bc-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f25bc-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="f25bc-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f25bc-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f25bc-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f25bc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f25bc-140">Response</span></span>

<span data-ttu-id="f25bc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f25bc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
