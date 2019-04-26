---
title: 'user: findRoomLists'
description: Obtenha as listas de salas definidas em um locatário.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9cdbfbdaaa09c8c311f3b8806da7c432f60ad626
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329883"
---
# <a name="user-findroomlists"></a><span data-ttu-id="ff021-103">user: findRoomLists</span><span class="sxs-lookup"><span data-stu-id="ff021-103">user: findRoomLists</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff021-104">Obtenha as listas de salas definidas em um locatário.</span><span class="sxs-lookup"><span data-stu-id="ff021-104">Get the room lists defined in a tenant.</span></span>

<span data-ttu-id="ff021-105">Os locatários podem organizar salas de reunião em listas de salas.</span><span class="sxs-lookup"><span data-stu-id="ff021-105">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="ff021-106">Cada sala de reunião e a lista de salas são representadas por uma instância [emailAddress](../resources/emailaddress.md).</span><span class="sxs-lookup"><span data-stu-id="ff021-106">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span>
<span data-ttu-id="ff021-107">Você pode ver todas as listas de salas no locatário, [obter todas as salas](user-findrooms.md) no locatário ou [todas as salas](user-findrooms.md) em uma lista de salas específica.</span><span class="sxs-lookup"><span data-stu-id="ff021-107">You can get all the room lists in the tenant, [get all the rooms](user-findrooms.md) in the tenant, or [get all the rooms](user-findrooms.md) in a specific room list.</span></span>


## <a name="permissions"></a><span data-ttu-id="ff021-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff021-108">Permissions</span></span>
<span data-ttu-id="ff021-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff021-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ff021-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff021-111">Permission type</span></span>      | <span data-ttu-id="ff021-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff021-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff021-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff021-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ff021-114">User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff021-114">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="ff021-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff021-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff021-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff021-116">Not supported.</span></span>    |
|<span data-ttu-id="ff021-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff021-117">Application</span></span> | <span data-ttu-id="ff021-118">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff021-118">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff021-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff021-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/findRoomLists
GET /users/<id>/findRoomLists

```

## <a name="request-headers"></a><span data-ttu-id="ff021-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff021-120">Request headers</span></span>
| <span data-ttu-id="ff021-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ff021-121">Name</span></span>       | <span data-ttu-id="ff021-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff021-122">Type</span></span> | <span data-ttu-id="ff021-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff021-123">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="ff021-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff021-124">Authorization</span></span>  | <span data-ttu-id="ff021-125">string</span><span class="sxs-lookup"><span data-stu-id="ff021-125">string</span></span>  | <span data-ttu-id="ff021-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff021-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ff021-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ff021-128">Content-Type</span></span>  | <span data-ttu-id="ff021-129">string</span><span class="sxs-lookup"><span data-stu-id="ff021-129">string</span></span>  | <span data-ttu-id="ff021-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff021-p104">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="ff021-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff021-132">Request body</span></span>
<span data-ttu-id="ff021-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ff021-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff021-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff021-134">Response</span></span>

<span data-ttu-id="ff021-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [emailAddress](../resources/emailaddress.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff021-135">If successful, this method returns a `200 OK` response code and [emailAddress](../resources/emailaddress.md) collection object in the response body.</span></span>

<span data-ttu-id="ff021-136">Se nenhuma lista for definida no locatário, uma matriz vazia será retornada.</span><span class="sxs-lookup"><span data-stu-id="ff021-136">If no lists are defined in the tenant, then an empty array is returned.</span></span>

## <a name="example"></a><span data-ttu-id="ff021-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff021-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff021-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff021-138">Request</span></span>

<span data-ttu-id="ff021-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff021-139">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_room_lists"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRoomLists
```

##### <a name="response"></a><span data-ttu-id="ff021-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff021-140">Response</span></span>
<span data-ttu-id="ff021-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff021-141">Here is an example of the response.</span></span> 

<span data-ttu-id="ff021-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff021-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
