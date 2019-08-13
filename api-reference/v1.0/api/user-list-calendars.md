---
title: Listar calendários
description: 'Obtenha calendários de todos do usuário (`/calendars` propriedade de navegação ), obtenha os calendários do grupo padrão de calendários ou de um grupo de calendários específico. '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c7c88a798306fb2ccb78d91ec5b64ddc7f92478d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372647"
---
# <a name="list-calendars"></a><span data-ttu-id="50810-103">Listar calendários</span><span class="sxs-lookup"><span data-stu-id="50810-103">List calendars</span></span>

<span data-ttu-id="50810-104">Obtenha calendários de todos do usuário (propriedade de navegação `/calendars`), obtenha os calendários do grupo padrão de calendários ou de um grupo de calendários específico.</span><span class="sxs-lookup"><span data-stu-id="50810-104">Get all the user's calendars (`/calendars` navigation property), get the calendars from the default calendar group or from a specific calendar group.</span></span> 
## <a name="permissions"></a><span data-ttu-id="50810-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="50810-105">Permissions</span></span>
<span data-ttu-id="50810-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50810-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50810-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50810-108">Permission type</span></span>      | <span data-ttu-id="50810-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="50810-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50810-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50810-110">Delegated (work or school account)</span></span> | <span data-ttu-id="50810-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50810-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="50810-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50810-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50810-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50810-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="50810-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50810-114">Application</span></span> | <span data-ttu-id="50810-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50810-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="50810-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50810-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="50810-117">Calendários de todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="50810-117">All the user's calendars.</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="50810-118">Os calendários do usuário no [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="50810-118">The user's calendars in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendargroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="50810-119">Os calendários do usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="50810-119">The user's calendars in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="50810-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="50810-120">Optional query parameters</span></span>
<span data-ttu-id="50810-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="50810-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="50810-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50810-122">Request headers</span></span>
| <span data-ttu-id="50810-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50810-123">Header</span></span>       | <span data-ttu-id="50810-124">Valor</span><span class="sxs-lookup"><span data-stu-id="50810-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="50810-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="50810-125">Authorization</span></span>  | <span data-ttu-id="50810-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50810-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="50810-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="50810-128">Content-Type</span></span>   | <span data-ttu-id="50810-129">application/json</span><span class="sxs-lookup"><span data-stu-id="50810-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="50810-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50810-130">Request body</span></span>
<span data-ttu-id="50810-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="50810-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50810-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="50810-132">Response</span></span>

<span data-ttu-id="50810-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50810-133">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="50810-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50810-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50810-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50810-135">Request</span></span>
<span data-ttu-id="50810-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50810-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="50810-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="50810-137">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_calendars"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendars
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="50810-138">C#</span><span class="sxs-lookup"><span data-stu-id="50810-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="50810-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50810-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="50810-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50810-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="50810-141">Java</span><span class="sxs-lookup"><span data-stu-id="50810-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-calendars-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="50810-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="50810-142">Response</span></span>
<span data-ttu-id="50810-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50810-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#me/calendars",
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
            "id": "AAMkAGI2TGuLAAA=",
            "name": "Calendar",
            "color": "auto",
            "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
            "canShare":true,
            "canViewPrivateItems":true,
            "canEdit":true,
            "owner":{
                "name":"Samantha Booth",
                "address":"samanthab@adatum.onmicrosoft.com"
            }
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
