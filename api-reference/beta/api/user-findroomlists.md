---
title: 'user: findRoomLists'
description: Obtenha as listas de salas definidas em um locatário.
author: vrod9429
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c091ac7071ce76dbb59cb69c10da2b6fa519f3cc
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052646"
---
# <a name="user-findroomlists"></a><span data-ttu-id="32545-103">user: findRoomLists</span><span class="sxs-lookup"><span data-stu-id="32545-103">user: findRoomLists</span></span>

<span data-ttu-id="32545-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32545-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32545-105">Obtenha as listas de salas definidas em um locatário, conforme representado por seus objetos [emailAddress](../resources/emailaddress.md).</span><span class="sxs-lookup"><span data-stu-id="32545-105">Get the room lists defined in a tenant, as represented by their [emailAddress](../resources/emailaddress.md) objects.</span></span>

<span data-ttu-id="32545-106">Os locatários podem organizar salas de reunião em listas de salas.</span><span class="sxs-lookup"><span data-stu-id="32545-106">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="32545-107">Nesta API, cada sala de reunião e lista de salas é representada por uma instância de [emailAddress](../resources/emailaddress.md).</span><span class="sxs-lookup"><span data-stu-id="32545-107">In this API, each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span>
<span data-ttu-id="32545-108">Você pode ver todas as listas de salas no locatário, [obter todas as salas](user-findrooms.md) no locatário ou [todas as salas](user-findrooms.md) em uma lista de salas específica.</span><span class="sxs-lookup"><span data-stu-id="32545-108">You can get all the room lists in the tenant, [get all the rooms](user-findrooms.md) in the tenant, or [get all the rooms](user-findrooms.md) in a specific room list.</span></span>


## <a name="permissions"></a><span data-ttu-id="32545-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="32545-109">Permissions</span></span>
<span data-ttu-id="32545-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32545-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="32545-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32545-112">Permission type</span></span>      | <span data-ttu-id="32545-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32545-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32545-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32545-114">Delegated (work or school account)</span></span> | <span data-ttu-id="32545-115">User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="32545-115">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="32545-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32545-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32545-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32545-117">Not supported.</span></span>    |
|<span data-ttu-id="32545-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32545-118">Application</span></span> | <span data-ttu-id="32545-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="32545-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="32545-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32545-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/findRoomLists
GET /users/{id}/findRoomLists

```

## <a name="request-headers"></a><span data-ttu-id="32545-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32545-121">Request headers</span></span>
| <span data-ttu-id="32545-122">Nome</span><span class="sxs-lookup"><span data-stu-id="32545-122">Name</span></span>       | <span data-ttu-id="32545-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="32545-123">Type</span></span> | <span data-ttu-id="32545-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="32545-124">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="32545-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="32545-125">Authorization</span></span>  | <span data-ttu-id="32545-126">string</span><span class="sxs-lookup"><span data-stu-id="32545-126">string</span></span>  | <span data-ttu-id="32545-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32545-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="32545-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32545-129">Content-Type</span></span>  | <span data-ttu-id="32545-130">string</span><span class="sxs-lookup"><span data-stu-id="32545-130">string</span></span>  | <span data-ttu-id="32545-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32545-p104">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="32545-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32545-133">Request body</span></span>
<span data-ttu-id="32545-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="32545-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32545-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="32545-135">Response</span></span>

<span data-ttu-id="32545-136">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [emailAddress](../resources/emailaddress.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32545-136">If successful, this method returns a `200 OK` response code and a collection of [emailAddress](../resources/emailaddress.md) objects in the response body.</span></span>

<span data-ttu-id="32545-137">Se nenhuma lista for definida no locatário, uma matriz vazia será retornada.</span><span class="sxs-lookup"><span data-stu-id="32545-137">If no lists are defined in the tenant, then an empty array is returned.</span></span>

## <a name="example"></a><span data-ttu-id="32545-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32545-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="32545-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32545-139">Request</span></span>

<span data-ttu-id="32545-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32545-140">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="32545-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="32545-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_room_lists"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/findRoomLists
```
# <a name="c"></a>[<span data-ttu-id="32545-142">C#</span><span class="sxs-lookup"><span data-stu-id="32545-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-room-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32545-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32545-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-room-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32545-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32545-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-room-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32545-145">Java</span><span class="sxs-lookup"><span data-stu-id="32545-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-room-lists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="32545-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="32545-146">Response</span></span>
<span data-ttu-id="32545-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32545-147">Here is an example of the response.</span></span> 

<span data-ttu-id="32545-148">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="32545-148">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_get_room_lists",
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
            "name": "Building 1 Rooms",
            "address": "Building1Rooms@contoso.onmicrosoft.com"
        },
        {
            "name": "Building 2 Rooms",
            "address": "Building2Rooms@contoso.onmicrosoft.com"
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: findRoomLists",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


