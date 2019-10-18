---
title: 'user: findRooms'
description: 'Veja todas as salas de reunião no locatário do usuário ou em uma lista de salas específica. '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 989ca48a799e27481194f79296aa04311c950dc0
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724306"
---
# <a name="user-findrooms"></a><span data-ttu-id="e25f6-103">user: findRooms</span><span class="sxs-lookup"><span data-stu-id="e25f6-103">user: findRooms</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e25f6-104">Obter os objetos [emailAddress](../resources/emailaddress.md) que representam todas as salas de reunião no locatário do usuário ou em uma lista de salas específica.</span><span class="sxs-lookup"><span data-stu-id="e25f6-104">Get all the meeting rooms in the user's tenant or in a specific room list.</span></span> 

<span data-ttu-id="e25f6-105">Os locatários podem organizar salas de reunião em listas de salas.</span><span class="sxs-lookup"><span data-stu-id="e25f6-105">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="e25f6-106">Nesta API, cada sala de reunião e lista de salas é representada por uma instância de [emailAddress](../resources/emailaddress.md).</span><span class="sxs-lookup"><span data-stu-id="e25f6-106">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span> <span data-ttu-id="e25f6-107">Você pode [ver todas as listas de salas](user-findroomlists.md) no locatário, obter todas as salas no locatário ou todas as salas em uma lista de salas específica.</span><span class="sxs-lookup"><span data-stu-id="e25f6-107">You can [get all the room lists](user-findroomlists.md) in the tenant, get all the rooms in the tenant, or get all the rooms in a specific room list.</span></span> <span data-ttu-id="e25f6-108">É possível ter acesso até as primeiras 100 salas do locatário.</span><span class="sxs-lookup"><span data-stu-id="e25f6-108">You can get up to the first 100 rooms in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="e25f6-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="e25f6-109">Permissions</span></span>
<span data-ttu-id="e25f6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e25f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e25f6-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e25f6-112">Permission type</span></span>      | <span data-ttu-id="e25f6-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e25f6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e25f6-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e25f6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e25f6-115">User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e25f6-115">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="e25f6-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e25f6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e25f6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e25f6-117">Not supported.</span></span>    |
|<span data-ttu-id="e25f6-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e25f6-118">Application</span></span> | <span data-ttu-id="e25f6-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e25f6-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e25f6-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e25f6-120">HTTP request</span></span>

<span data-ttu-id="e25f6-121">Para ver todas as salas no locatário:</span><span class="sxs-lookup"><span data-stu-id="e25f6-121">To get all the rooms in the tenant:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/{id}/findRooms
```

<span data-ttu-id="e25f6-122">Para ver todas as salas em uma lista de salas específicas do locatário:</span><span class="sxs-lookup"><span data-stu-id="e25f6-122">To get all the rooms in a specific room list of the tenant's:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list_emailAddress}')
GET /users/{id}/findRooms(RoomList='{room_list_emailAddress}')
```

## <a name="query-parameters"></a><span data-ttu-id="e25f6-123">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="e25f6-123">Query parameters</span></span>

| <span data-ttu-id="e25f6-124">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="e25f6-124">Query parameter</span></span>       | <span data-ttu-id="e25f6-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="e25f6-125">Type</span></span> | <span data-ttu-id="e25f6-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e25f6-126">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="e25f6-127">RoomList</span><span class="sxs-lookup"><span data-stu-id="e25f6-127">RoomList</span></span> | <span data-ttu-id="e25f6-128">string</span><span class="sxs-lookup"><span data-stu-id="e25f6-128">string</span></span> | <span data-ttu-id="e25f6-129">O endereço SMTP associado à lista de salas.</span><span class="sxs-lookup"><span data-stu-id="e25f6-129">The SMTP address associated with the room list.</span></span> <span data-ttu-id="e25f6-130">Cada lista de salas é representada por uma instância [emailAddress](../resources/emailaddress.md) que inclui um endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="e25f6-130">Each room list is represented by an [emailAddress](../resources/emailaddress.md) instance that includes an SMTP address.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="e25f6-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e25f6-131">Request headers</span></span>
| <span data-ttu-id="e25f6-132">Nome</span><span class="sxs-lookup"><span data-stu-id="e25f6-132">Name</span></span>       | <span data-ttu-id="e25f6-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="e25f6-133">Type</span></span> | <span data-ttu-id="e25f6-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="e25f6-134">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="e25f6-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="e25f6-135">Authorization</span></span>  | <span data-ttu-id="e25f6-136">string</span><span class="sxs-lookup"><span data-stu-id="e25f6-136">string</span></span>  | <span data-ttu-id="e25f6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e25f6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e25f6-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e25f6-139">Content-Type</span></span>  | <span data-ttu-id="e25f6-140">string</span><span class="sxs-lookup"><span data-stu-id="e25f6-140">string</span></span>  | <span data-ttu-id="e25f6-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e25f6-p105">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e25f6-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e25f6-143">Request body</span></span>
<span data-ttu-id="e25f6-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e25f6-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e25f6-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e25f6-145">Response</span></span>

<span data-ttu-id="e25f6-146">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [emailAddress](../resources/emailaddress.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e25f6-146">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/emailaddress.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="e25f6-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e25f6-147">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="e25f6-148">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="e25f6-148">Request 1</span></span>

<span data-ttu-id="e25f6-149">O primeiro exemplo obtém os objetos [emailAddress](../resources/emailaddress.md) que representam todas as salas definidas no locatário do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="e25f6-149">The first example gets all the rooms defined in the signed-in user's tenant.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e25f6-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="e25f6-150">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/findRooms
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e25f6-151">C#</span><span class="sxs-lookup"><span data-stu-id="e25f6-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-rooms-in-tenant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e25f6-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e25f6-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-rooms-in-tenant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e25f6-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e25f6-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-rooms-in-tenant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="e25f6-154">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="e25f6-154">Response 1</span></span>
<span data-ttu-id="e25f6-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e25f6-155">Here is an example of the response.</span></span> 

<span data-ttu-id="e25f6-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e25f6-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="e25f6-158">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="e25f6-158">Request 2</span></span>

<span data-ttu-id="e25f6-159">O segundo exemplo obtém os objetos [emailAddress](../resources/emailaddress.md) que representam as salas na lista de salas especificadas, identificadas pelo endereço de email Building2Rooms@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="e25f6-159">The second example gets the rooms in the specified room list identified by the email address Building2Rooms@contoso.onmicrosoft.com.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e25f6-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="e25f6-160">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e25f6-161">C#</span><span class="sxs-lookup"><span data-stu-id="e25f6-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-rooms-from-specific-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e25f6-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e25f6-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-rooms-from-specific-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e25f6-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e25f6-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-rooms-from-specific-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="e25f6-164">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="e25f6-164">Response 2</span></span>
<span data-ttu-id="e25f6-165">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e25f6-165">Here is an example of the response.</span></span> 

<span data-ttu-id="e25f6-p107">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e25f6-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
