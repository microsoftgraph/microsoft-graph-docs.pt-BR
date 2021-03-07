---
title: Listar calendários
description: 'Obtenha calendários de todos do usuário (`/calendars` propriedade de navegação ), obtenha os calendários do grupo padrão de calendários ou de um grupo de calendários específico. '
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 277a7d9e1c5389ecde9f49c6d367a4589f37b591
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516718"
---
# <a name="list-calendars"></a><span data-ttu-id="a6844-103">Listar calendários</span><span class="sxs-lookup"><span data-stu-id="a6844-103">List calendars</span></span>

<span data-ttu-id="a6844-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6844-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a6844-105">Obtenha calendários de todos do usuário (`/calendars` propriedade de navegação ), obtenha os calendários do grupo padrão de calendários ou de um grupo de calendários específico.</span><span class="sxs-lookup"><span data-stu-id="a6844-105">Get all the user's calendars (`/calendars` navigation property), get the calendars from the default calendar group or from a specific calendar group.</span></span> 
## <a name="permissions"></a><span data-ttu-id="a6844-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a6844-106">Permissions</span></span>
<span data-ttu-id="a6844-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6844-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6844-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6844-109">Permission type</span></span>      | <span data-ttu-id="a6844-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6844-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6844-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6844-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a6844-112">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6844-112">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a6844-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6844-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6844-114">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6844-114">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a6844-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6844-115">Application</span></span> | <span data-ttu-id="a6844-116">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6844-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6844-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6844-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="a6844-118">Calendários de todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="a6844-118">All the user's calendars.</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="a6844-119">Os calendários do usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="a6844-119">The user's calendars in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a6844-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a6844-120">Optional query parameters</span></span>
<span data-ttu-id="a6844-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a6844-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a6844-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6844-122">Request headers</span></span>
| <span data-ttu-id="a6844-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6844-123">Header</span></span>       | <span data-ttu-id="a6844-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a6844-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a6844-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6844-125">Authorization</span></span>  | <span data-ttu-id="a6844-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6844-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a6844-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a6844-128">Content-Type</span></span>   | <span data-ttu-id="a6844-129">application/json</span><span class="sxs-lookup"><span data-stu-id="a6844-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6844-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6844-130">Request body</span></span>
<span data-ttu-id="a6844-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a6844-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6844-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6844-132">Response</span></span>

<span data-ttu-id="a6844-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6844-133">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a6844-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6844-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="a6844-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6844-135">Request</span></span>
<span data-ttu-id="a6844-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6844-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a6844-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6844-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_calendars"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendars
```
# <a name="c"></a>[<span data-ttu-id="a6844-138">C#</span><span class="sxs-lookup"><span data-stu-id="a6844-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6844-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6844-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6844-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6844-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6844-141">Java</span><span class="sxs-lookup"><span data-stu-id="a6844-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-calendars-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a6844-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6844-142">Response</span></span>
<span data-ttu-id="a6844-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6844-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
            "hexColor": "",
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
<!-- {
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
