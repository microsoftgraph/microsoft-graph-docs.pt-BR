---
title: 'user: findRooms'
description: 'Veja todas as salas de reunião no locatário do usuário ou em uma lista de salas específica. '
localization_priority: Priority
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 292634327717d720a80d55065041de7571660858
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970096"
---
# <a name="user-findrooms"></a><span data-ttu-id="37c63-103">user: findRooms</span><span class="sxs-lookup"><span data-stu-id="37c63-103">user: findRooms</span></span>

<span data-ttu-id="37c63-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37c63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37c63-105">Obter os objetos [emailAddress](../resources/emailaddress.md) que representam todas as salas de reunião no locatário do usuário ou em uma lista de salas específica.</span><span class="sxs-lookup"><span data-stu-id="37c63-105">Get the [emailAddress](../resources/emailaddress.md) objects that represent all the meeting rooms in the user's tenant or in a specific room list.</span></span> 

<span data-ttu-id="37c63-106">Os locatários podem organizar salas de reunião em listas de salas.</span><span class="sxs-lookup"><span data-stu-id="37c63-106">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="37c63-107">Nesta API, cada sala de reunião e lista de salas é representada por uma instância de [emailAddress](../resources/emailaddress.md).</span><span class="sxs-lookup"><span data-stu-id="37c63-107">In this API, each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span> <span data-ttu-id="37c63-108">Você pode [ver todas as listas de salas](user-findroomlists.md) no locatário, obter todas as salas no locatário ou todas as salas em uma lista de salas específica.</span><span class="sxs-lookup"><span data-stu-id="37c63-108">You can [get all the room lists](user-findroomlists.md) in the tenant, get all the rooms in the tenant, or get all the rooms in a specific room list.</span></span> <span data-ttu-id="37c63-109">É possível ter acesso até as primeiras 100 salas do locatário.</span><span class="sxs-lookup"><span data-stu-id="37c63-109">You can get up to the first 100 rooms in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="37c63-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="37c63-110">Permissions</span></span>
<span data-ttu-id="37c63-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37c63-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="37c63-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37c63-113">Permission type</span></span>      | <span data-ttu-id="37c63-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37c63-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37c63-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37c63-115">Delegated (work or school account)</span></span> | <span data-ttu-id="37c63-116">User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="37c63-116">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="37c63-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37c63-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37c63-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37c63-118">Not supported.</span></span>    |
|<span data-ttu-id="37c63-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37c63-119">Application</span></span> | <span data-ttu-id="37c63-120">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="37c63-120">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37c63-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37c63-121">HTTP request</span></span>

<span data-ttu-id="37c63-122">Para ver todas as salas no locatário:</span><span class="sxs-lookup"><span data-stu-id="37c63-122">To get all the rooms in the tenant:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/{id}/findRooms
```

<span data-ttu-id="37c63-123">Para ver todas as salas em uma lista de salas específicas do locatário:</span><span class="sxs-lookup"><span data-stu-id="37c63-123">To get all the rooms in a specific room list of the tenant's:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list_emailAddress}')
GET /users/{id}/findRooms(RoomList='{room_list_emailAddress}')
```

## <a name="query-parameters"></a><span data-ttu-id="37c63-124">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="37c63-124">Query parameters</span></span>

| <span data-ttu-id="37c63-125">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="37c63-125">Query parameter</span></span>       | <span data-ttu-id="37c63-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="37c63-126">Type</span></span> | <span data-ttu-id="37c63-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="37c63-127">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="37c63-128">RoomList</span><span class="sxs-lookup"><span data-stu-id="37c63-128">RoomList</span></span> | <span data-ttu-id="37c63-129">string</span><span class="sxs-lookup"><span data-stu-id="37c63-129">string</span></span> | <span data-ttu-id="37c63-130">O endereço SMTP associado à lista de salas.</span><span class="sxs-lookup"><span data-stu-id="37c63-130">The SMTP address associated with the room list.</span></span> <span data-ttu-id="37c63-131">Cada lista de salas é representada por uma instância [emailAddress](../resources/emailaddress.md) que inclui um endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="37c63-131">Each room list is represented by an [emailAddress](../resources/emailaddress.md) instance that includes an SMTP address.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="37c63-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37c63-132">Request headers</span></span>
| <span data-ttu-id="37c63-133">Nome</span><span class="sxs-lookup"><span data-stu-id="37c63-133">Name</span></span>       | <span data-ttu-id="37c63-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="37c63-134">Type</span></span> | <span data-ttu-id="37c63-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="37c63-135">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="37c63-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="37c63-136">Authorization</span></span>  | <span data-ttu-id="37c63-137">string</span><span class="sxs-lookup"><span data-stu-id="37c63-137">string</span></span>  | <span data-ttu-id="37c63-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37c63-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="37c63-140">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37c63-140">Content-Type</span></span>  | <span data-ttu-id="37c63-141">string</span><span class="sxs-lookup"><span data-stu-id="37c63-141">string</span></span>  | <span data-ttu-id="37c63-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37c63-p105">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="37c63-144">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37c63-144">Request body</span></span>
<span data-ttu-id="37c63-145">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37c63-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37c63-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="37c63-146">Response</span></span>

<span data-ttu-id="37c63-147">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [emailAddress](../resources/emailaddress.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37c63-147">If successful, this method returns a `200 OK` response code and a collection of [emailAddress](../resources/emailaddress.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="37c63-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37c63-148">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="37c63-149">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="37c63-149">Request 1</span></span>

<span data-ttu-id="37c63-150">O primeiro exemplo obtém os objetos [emailAddress](../resources/emailaddress.md) que representam todas as salas definidas no locatário do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="37c63-150">The first example gets the [emailAddress](../resources/emailaddress.md) objects that represent all the rooms defined in the signed-in user's tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="37c63-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="37c63-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/findRooms
```
# <a name="c"></a>[<span data-ttu-id="37c63-152">C#</span><span class="sxs-lookup"><span data-stu-id="37c63-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-rooms-in-tenant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37c63-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37c63-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-rooms-in-tenant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37c63-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37c63-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-rooms-in-tenant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37c63-155">Java</span><span class="sxs-lookup"><span data-stu-id="37c63-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-rooms-in-tenant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="37c63-156">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="37c63-156">Response 1</span></span>
<span data-ttu-id="37c63-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37c63-157">Here is an example of the response.</span></span> 

<span data-ttu-id="37c63-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37c63-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="37c63-160">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="37c63-160">Request 2</span></span>

<span data-ttu-id="37c63-161">O segundo exemplo obtém os objetos [emailAddress](../resources/emailaddress.md) que representam as salas na lista de salas especificadas, identificadas pelo endereço de email Building2Rooms@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="37c63-161">The second example gets the [emailAddress](../resources/emailaddress.md) objects that represent the rooms in the specified room list identified by the email address Building2Rooms@contoso.onmicrosoft.com.</span></span>


# <a name="http"></a>[<span data-ttu-id="37c63-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="37c63-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```
# <a name="c"></a>[<span data-ttu-id="37c63-163">C#</span><span class="sxs-lookup"><span data-stu-id="37c63-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-rooms-from-specific-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37c63-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37c63-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-rooms-from-specific-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37c63-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37c63-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-rooms-from-specific-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37c63-166">Java</span><span class="sxs-lookup"><span data-stu-id="37c63-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-rooms-from-specific-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="37c63-167">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="37c63-167">Response 2</span></span>
<span data-ttu-id="37c63-168">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37c63-168">Here is an example of the response.</span></span> 

<span data-ttu-id="37c63-p107">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37c63-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


