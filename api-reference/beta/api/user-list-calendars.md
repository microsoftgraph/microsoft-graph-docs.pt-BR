---
title: Listar calendários
description: 'Obtenha calendários de todos do usuário (`/calendars` propriedade de navegação ), obtenha os calendários do grupo padrão de calendários ou de um grupo de calendários específico. '
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2b6c9089f0f839d59dcaaab61690b5bbf760dd56
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052604"
---
# <a name="list-calendars"></a><span data-ttu-id="a5fed-103">Listar calendários</span><span class="sxs-lookup"><span data-stu-id="a5fed-103">List calendars</span></span>

<span data-ttu-id="a5fed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5fed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5fed-105">Obtenha calendários de todos do usuário (`/calendars` propriedade de navegação ), obtenha os calendários do grupo padrão de calendários ou de um grupo de calendários específico.</span><span class="sxs-lookup"><span data-stu-id="a5fed-105">Get all the user's calendars (`/calendars` navigation property), get the calendars from the default calendar group or from a specific calendar group.</span></span> 
## <a name="permissions"></a><span data-ttu-id="a5fed-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5fed-106">Permissions</span></span>
<span data-ttu-id="a5fed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5fed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5fed-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5fed-109">Permission type</span></span>      | <span data-ttu-id="a5fed-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5fed-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5fed-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5fed-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a5fed-112">Calendars.Read, Calendars.Read.Shared, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5fed-112">Calendars.Read, Calendars.Read.Shared, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a5fed-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5fed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5fed-114">Calendars.Read, Calendars.Read.Shared, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5fed-114">Calendars.Read, Calendars.Read.Shared, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a5fed-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5fed-115">Application</span></span> | <span data-ttu-id="a5fed-116">Calendars.Read, Calendars.Read.Shared, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5fed-116">Calendars.Read, Calendars.Read.Shared, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5fed-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5fed-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="a5fed-118">Calendários de todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="a5fed-118">All the user's calendars.</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="a5fed-119">Os calendários do usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="a5fed-119">The user's calendars in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5fed-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a5fed-120">Optional query parameters</span></span>
<span data-ttu-id="a5fed-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a5fed-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a5fed-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5fed-122">Request headers</span></span>
| <span data-ttu-id="a5fed-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a5fed-123">Header</span></span>       | <span data-ttu-id="a5fed-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a5fed-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a5fed-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5fed-125">Authorization</span></span>  | <span data-ttu-id="a5fed-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5fed-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a5fed-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5fed-128">Content-Type</span></span>   | <span data-ttu-id="a5fed-129">application/json</span><span class="sxs-lookup"><span data-stu-id="a5fed-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5fed-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5fed-130">Request body</span></span>
<span data-ttu-id="a5fed-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a5fed-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5fed-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5fed-132">Response</span></span>

<span data-ttu-id="a5fed-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5fed-133">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a5fed-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5fed-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="a5fed-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5fed-135">Request</span></span>
<span data-ttu-id="a5fed-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5fed-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a5fed-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5fed-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_calendars"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendars
```
# <a name="c"></a>[<span data-ttu-id="a5fed-138">C#</span><span class="sxs-lookup"><span data-stu-id="a5fed-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5fed-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5fed-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5fed-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5fed-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5fed-141">Java</span><span class="sxs-lookup"><span data-stu-id="a5fed-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-calendars-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a5fed-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5fed-142">Response</span></span>
<span data-ttu-id="a5fed-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5fed-143">Here is an example of the response.</span></span> <span data-ttu-id="a5fed-144">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a5fed-144">Note: The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#me/calendars",
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
            "id": "AAMkAGI2TGuLAAA=",
            "name": "Calendar",
            "color": "auto",
            "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
            "calendarGroupId":null,
            "isDefaultCalendar": true,
            "canShare":true,
            "canViewPrivateItems":true,
            "hexColor": "",
            "isShared":false,
            "isSharedWithMe":false,
            "canEdit":true,
            "allowedOnlineMeetingProviders": [
                "teamsForBusiness"
            ],
            "defaultOnlineMeetingProvider": "teamsForBusiness",
            "isTallyingResponses": true,
            "isRemovable": false,
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
