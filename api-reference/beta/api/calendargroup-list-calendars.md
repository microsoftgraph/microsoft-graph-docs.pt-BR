---
title: Listar calendários
description: Recupera uma lista de calendários que pertencem a um grupo de calendários.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d1dc7c556f304b15935f2c1ec14c16d035dfdf64
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047704"
---
# <a name="list-calendars"></a><span data-ttu-id="618a5-103">Listar calendários</span><span class="sxs-lookup"><span data-stu-id="618a5-103">List calendars</span></span>

<span data-ttu-id="618a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="618a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="618a5-105">Recupera uma lista de calendários que pertencem a um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="618a5-105">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="618a5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="618a5-106">Permissions</span></span>

<span data-ttu-id="618a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="618a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="618a5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="618a5-109">Permission type</span></span>                        | <span data-ttu-id="618a5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="618a5-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="618a5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="618a5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="618a5-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="618a5-112">Calendars.Read</span></span>                              |
| <span data-ttu-id="618a5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="618a5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="618a5-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="618a5-114">Calendars.Read</span></span>                              |
| <span data-ttu-id="618a5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="618a5-115">Application</span></span>                            | <span data-ttu-id="618a5-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="618a5-116">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="618a5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="618a5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="618a5-118">Um [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="618a5-118">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="618a5-119">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="618a5-119">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="618a5-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="618a5-120">Optional query parameters</span></span>

<span data-ttu-id="618a5-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="618a5-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="618a5-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="618a5-122">Request headers</span></span>

| <span data-ttu-id="618a5-123">Nome</span><span class="sxs-lookup"><span data-stu-id="618a5-123">Name</span></span>          | <span data-ttu-id="618a5-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="618a5-124">Type</span></span>   | <span data-ttu-id="618a5-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="618a5-125">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="618a5-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="618a5-126">Authorization</span></span> | <span data-ttu-id="618a5-127">string</span><span class="sxs-lookup"><span data-stu-id="618a5-127">string</span></span> | <span data-ttu-id="618a5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="618a5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="618a5-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="618a5-130">Request body</span></span>

<span data-ttu-id="618a5-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="618a5-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="618a5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="618a5-132">Response</span></span>

<span data-ttu-id="618a5-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="618a5-133">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="618a5-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="618a5-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="618a5-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="618a5-135">Request</span></span>

<span data-ttu-id="618a5-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="618a5-136">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="618a5-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="618a5-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendargroup_get_calendars"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```
# <a name="c"></a>[<span data-ttu-id="618a5-138">C#</span><span class="sxs-lookup"><span data-stu-id="618a5-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendargroup-get-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="618a5-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="618a5-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendargroup-get-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="618a5-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="618a5-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendargroup-get-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="618a5-141">Java</span><span class="sxs-lookup"><span data-stu-id="618a5-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendargroup-get-calendars-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="618a5-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="618a5-142">Response</span></span>

<span data-ttu-id="618a5-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="618a5-143">Here is an example of the response.</span></span> <span data-ttu-id="618a5-144">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="618a5-144">Note: The response object shown here might be shortened for readability.</span></span>

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
      "calendarGroupId":"calendarGroupId-value",
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
