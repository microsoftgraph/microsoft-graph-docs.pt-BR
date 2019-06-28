---
title: 'user: findRooms'
description: 'Veja todas as salas de reunião no locatário do usuário ou em uma lista de salas específica. '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a7e4db27796a50b17819c1858e1d18e3dd7746f1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270333"
---
# <a name="user-findrooms"></a><span data-ttu-id="2ffd2-103">user: findRooms</span><span class="sxs-lookup"><span data-stu-id="2ffd2-103">user: findRooms</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ffd2-104">Obter os objetos [emailAddress](../resources/emailaddress.md) que representam todas as salas de reunião no locatário do usuário ou em uma lista de salas específica.</span><span class="sxs-lookup"><span data-stu-id="2ffd2-104">Get all the meeting rooms in the user's tenant or in a specific room list.</span></span> 

<span data-ttu-id="2ffd2-105">Os locatários podem organizar salas de reunião em listas de salas.</span><span class="sxs-lookup"><span data-stu-id="2ffd2-105">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="2ffd2-106">Nesta API, cada sala de reunião e lista de salas é representada por uma instância de [emailAddress](../resources/emailaddress.md).</span><span class="sxs-lookup"><span data-stu-id="2ffd2-106">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span> <span data-ttu-id="2ffd2-107">Você pode [ver todas as listas de salas](user-findroomlists.md) no locatário, obter todas as salas no locatário ou todas as salas em uma lista de salas específica.</span><span class="sxs-lookup"><span data-stu-id="2ffd2-107">You can [get all the room lists](user-findroomlists.md) in the tenant, get all the rooms in the tenant, or get all the rooms in a specific room list.</span></span> <span data-ttu-id="2ffd2-108">É possível ter acesso até as primeiras 100 salas do locatário.</span><span class="sxs-lookup"><span data-stu-id="2ffd2-108">You can get up to the first 100 rooms in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ffd2-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ffd2-109">Permissions</span></span>
<span data-ttu-id="2ffd2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ffd2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2ffd2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ffd2-112">Permission type</span></span>      | <span data-ttu-id="2ffd2-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ffd2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ffd2-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ffd2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2ffd2-115">User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ffd2-115">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="2ffd2-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ffd2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ffd2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ffd2-117">Not supported.</span></span>    |
|<span data-ttu-id="2ffd2-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ffd2-118">Application</span></span> | <span data-ttu-id="2ffd2-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ffd2-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ffd2-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ffd2-120">HTTP request</span></span>

<span data-ttu-id="2ffd2-121">Para ver todas as salas no locatário:</span><span class="sxs-lookup"><span data-stu-id="2ffd2-121">To get all the rooms in the tenant:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/<id>/findRooms
```

<span data-ttu-id="2ffd2-122">Para ver todas as salas em uma lista de salas específicas do locatário:</span><span class="sxs-lookup"><span data-stu-id="2ffd2-122">To get all the rooms in a specific room list of the tenant's:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list_emailAddress}')
GET /users/<id>/findRooms(RoomList='{room_list_emailAddress}')
```

## <a name="query-parameters"></a><span data-ttu-id="2ffd2-123">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="2ffd2-123">Query parameters</span></span>

| <span data-ttu-id="2ffd2-124">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="2ffd2-124">Query parameter</span></span>       | <span data-ttu-id="2ffd2-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ffd2-125">Type</span></span> | <span data-ttu-id="2ffd2-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ffd2-126">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="2ffd2-127">RoomList</span><span class="sxs-lookup"><span data-stu-id="2ffd2-127">RoomList</span></span> | <span data-ttu-id="2ffd2-128">string</span><span class="sxs-lookup"><span data-stu-id="2ffd2-128">string</span></span> | <span data-ttu-id="2ffd2-129">O endereço SMTP associado à lista de salas.</span><span class="sxs-lookup"><span data-stu-id="2ffd2-129">The SMTP address associated with the room list.</span></span> <span data-ttu-id="2ffd2-130">Cada lista de salas é representada por uma instância [emailAddress](../resources/emailaddress.md) que inclui um endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="2ffd2-130">Each room list is represented by an [emailAddress](../resources/emailaddress.md) instance that includes an SMTP address.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="2ffd2-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ffd2-131">Request headers</span></span>
| <span data-ttu-id="2ffd2-132">Nome</span><span class="sxs-lookup"><span data-stu-id="2ffd2-132">Name</span></span>       | <span data-ttu-id="2ffd2-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ffd2-133">Type</span></span> | <span data-ttu-id="2ffd2-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ffd2-134">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="2ffd2-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ffd2-135">Authorization</span></span>  | <span data-ttu-id="2ffd2-136">string</span><span class="sxs-lookup"><span data-stu-id="2ffd2-136">string</span></span>  | <span data-ttu-id="2ffd2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ffd2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2ffd2-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2ffd2-139">Content-Type</span></span>  | <span data-ttu-id="2ffd2-140">string</span><span class="sxs-lookup"><span data-stu-id="2ffd2-140">string</span></span>  | <span data-ttu-id="2ffd2-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ffd2-p105">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="2ffd2-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ffd2-143">Request body</span></span>
<span data-ttu-id="2ffd2-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2ffd2-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ffd2-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ffd2-145">Response</span></span>

<span data-ttu-id="2ffd2-146">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [emailAddress](../resources/emailaddress.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ffd2-146">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/emailaddress.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="2ffd2-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ffd2-147">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="2ffd2-148">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="2ffd2-148">Request 1</span></span>

<span data-ttu-id="2ffd2-149">O primeiro exemplo obtém os objetos [emailAddress](../resources/emailaddress.md) que representam todas as salas definidas no locatário do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="2ffd2-149">The first example gets all the rooms defined in the signed-in user's tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms
```

##### <a name="response-1"></a><span data-ttu-id="2ffd2-150">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="2ffd2-150">Response 1</span></span>
<span data-ttu-id="2ffd2-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ffd2-151">Here is an example of the response.</span></span> 

<span data-ttu-id="2ffd2-p106">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ffd2-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_get_rooms_in_tenant",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAddress",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAddress)",
    "value": [
        {
            "name": "Conf Room Adams",
            "address": "Adams@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Baker",
            "address": "Baker@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Crystal",
            "address": "Crystal@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Hood",
            "address": "Hood@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Rainier",
            "address": "Rainier@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Stevens",
            "address": "Stevens@contoso.onmicrosoft.com"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2ffd2-154">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="2ffd2-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2ffd2-155">C#</span><span class="sxs-lookup"><span data-stu-id="2ffd2-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_get_rooms_in_tenant-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ffd2-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="2ffd2-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_get_rooms_in_tenant-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2ffd2-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ffd2-157">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_get_rooms_in_tenant-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="2ffd2-158">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="2ffd2-158">Request 2</span></span>

<span data-ttu-id="2ffd2-159">O segundo exemplo obtém os objetos [emailAddress](../resources/emailaddress.md) que representam as salas na lista de salas especificadas, identificadas pelo endereço de email Building2Rooms@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="2ffd2-159">The second example gets the rooms in the specified room list identified by the email address Building2Rooms@contoso.onmicrosoft.com.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```

##### <a name="response-2"></a><span data-ttu-id="2ffd2-160">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="2ffd2-160">Response 2</span></span>
<span data-ttu-id="2ffd2-161">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ffd2-161">Here is an example of the response.</span></span> 

<span data-ttu-id="2ffd2-p107">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ffd2-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_get_rooms_from_specific_list",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAddress",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAddress)",
    "value": [
        {
            "name": "Conf Room Baker",
            "address": "Baker@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Hood",
            "address": "Hood@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Rainier",
            "address": "Rainier@contoso.onmicrosoft.com"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2ffd2-164">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="2ffd2-164">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2ffd2-165">C#</span><span class="sxs-lookup"><span data-stu-id="2ffd2-165">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_get_rooms_from_specific_list-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ffd2-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="2ffd2-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_get_rooms_from_specific_list-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2ffd2-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ffd2-167">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_get_rooms_from_specific_list-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: findRooms",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-findrooms.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-findrooms.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-findrooms.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-findrooms.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-findrooms.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
