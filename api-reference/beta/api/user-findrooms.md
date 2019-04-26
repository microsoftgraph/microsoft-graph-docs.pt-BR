---
title: 'user: findRooms'
description: 'Veja todas as salas de reunião no locatário do usuário ou em uma lista de salas específica. '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 63538341e72b293b2a90baa27d7b7617f6181207
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334951"
---
# <a name="user-findrooms"></a><span data-ttu-id="5c7bd-103">user: findRooms</span><span class="sxs-lookup"><span data-stu-id="5c7bd-103">user: findRooms</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c7bd-104">Veja todas as salas de reunião no locatário do usuário ou em uma lista de salas específica.</span><span class="sxs-lookup"><span data-stu-id="5c7bd-104">Get all the meeting rooms in the user's tenant or in a specific room list.</span></span> 

<span data-ttu-id="5c7bd-105">Os locatários podem organizar salas de reunião em listas de salas.</span><span class="sxs-lookup"><span data-stu-id="5c7bd-105">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="5c7bd-106">Cada sala de reunião e a lista de salas são representadas por uma instância [emailAddress](../resources/emailaddress.md).</span><span class="sxs-lookup"><span data-stu-id="5c7bd-106">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span> <span data-ttu-id="5c7bd-107">Você pode [ver todas as listas de salas](user-findroomlists.md) no locatário, obter todas as salas no locatário ou todas as salas em uma lista de salas específica.</span><span class="sxs-lookup"><span data-stu-id="5c7bd-107">You can [get all the room lists](user-findroomlists.md) in the tenant, get all the rooms in the tenant, or get all the rooms in a specific room list.</span></span> <span data-ttu-id="5c7bd-108">É possível ter acesso até as primeiras 100 salas do locatário.</span><span class="sxs-lookup"><span data-stu-id="5c7bd-108">You can get up to the first 100 rooms in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c7bd-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c7bd-109">Permissions</span></span>
<span data-ttu-id="5c7bd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c7bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5c7bd-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c7bd-112">Permission type</span></span>      | <span data-ttu-id="5c7bd-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c7bd-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c7bd-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c7bd-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5c7bd-115">User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c7bd-115">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="5c7bd-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c7bd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c7bd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c7bd-117">Not supported.</span></span>    |
|<span data-ttu-id="5c7bd-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c7bd-118">Application</span></span> | <span data-ttu-id="5c7bd-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c7bd-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c7bd-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c7bd-120">HTTP request</span></span>

<span data-ttu-id="5c7bd-121">Para ver todas as salas no locatário:</span><span class="sxs-lookup"><span data-stu-id="5c7bd-121">To get all the rooms in the tenant:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/<id>/findRooms
```

<span data-ttu-id="5c7bd-122">Para ver todas as salas em uma lista de salas específicas do locatário:</span><span class="sxs-lookup"><span data-stu-id="5c7bd-122">To get all the rooms in a specific room list of the tenant's:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list}')
GET /users/<id>/findRooms(RoomList='{room_list}')
```

## <a name="query-parameters"></a><span data-ttu-id="5c7bd-123">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="5c7bd-123">Query parameters</span></span>

| <span data-ttu-id="5c7bd-124">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="5c7bd-124">Query parameter</span></span>       | <span data-ttu-id="5c7bd-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c7bd-125">Type</span></span> | <span data-ttu-id="5c7bd-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c7bd-126">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="5c7bd-127">RoomList</span><span class="sxs-lookup"><span data-stu-id="5c7bd-127">RoomList</span></span> | <span data-ttu-id="5c7bd-128">string</span><span class="sxs-lookup"><span data-stu-id="5c7bd-128">string</span></span> | <span data-ttu-id="5c7bd-129">O endereço SMTP associado à lista de salas.</span><span class="sxs-lookup"><span data-stu-id="5c7bd-129">The SMTP address associated with the room list.</span></span> <span data-ttu-id="5c7bd-130">Cada lista de salas é representada por uma instância [emailAddress](../resources/emailaddress.md) que inclui um endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="5c7bd-130">Each room list is represented by an [emailAddress](../resources/emailaddress.md) instance that includes an SMTP address.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5c7bd-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c7bd-131">Request headers</span></span>
| <span data-ttu-id="5c7bd-132">Nome</span><span class="sxs-lookup"><span data-stu-id="5c7bd-132">Name</span></span>       | <span data-ttu-id="5c7bd-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c7bd-133">Type</span></span> | <span data-ttu-id="5c7bd-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c7bd-134">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="5c7bd-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c7bd-135">Authorization</span></span>  | <span data-ttu-id="5c7bd-136">string</span><span class="sxs-lookup"><span data-stu-id="5c7bd-136">string</span></span>  | <span data-ttu-id="5c7bd-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c7bd-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5c7bd-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5c7bd-139">Content-Type</span></span>  | <span data-ttu-id="5c7bd-140">string</span><span class="sxs-lookup"><span data-stu-id="5c7bd-140">string</span></span>  | <span data-ttu-id="5c7bd-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c7bd-p105">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="5c7bd-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c7bd-143">Request body</span></span>
<span data-ttu-id="5c7bd-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c7bd-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c7bd-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c7bd-145">Response</span></span>

<span data-ttu-id="5c7bd-146">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [emailAddress](../resources/emailaddress.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c7bd-146">If successful, this method returns a `200 OK` response code and [emailAddress](../resources/emailaddress.md) collection object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="5c7bd-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c7bd-147">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="5c7bd-148">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="5c7bd-148">Request 1</span></span>

<span data-ttu-id="5c7bd-149">O primeiro exemplo obtém todas as salas definidas no locatário do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="5c7bd-149">The first example gets all the rooms defined in the signed-in user's tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms
```

##### <a name="response-1"></a><span data-ttu-id="5c7bd-150">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="5c7bd-150">Response 1</span></span>
<span data-ttu-id="5c7bd-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c7bd-151">Here is an example of the response.</span></span> 

<span data-ttu-id="5c7bd-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c7bd-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="5c7bd-154">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="5c7bd-154">Request 2</span></span>

<span data-ttu-id="5c7bd-155">O segundo exemplo recebe as salas na lista de salas especificada identificada pelo endereço de email Building2Rooms@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="5c7bd-155">The second example gets the rooms in the specified room list identified by the email address Building2Rooms@contoso.onmicrosoft.com.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```

##### <a name="response-2"></a><span data-ttu-id="5c7bd-156">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="5c7bd-156">Response 2</span></span>
<span data-ttu-id="5c7bd-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c7bd-157">Here is an example of the response.</span></span> 

<span data-ttu-id="5c7bd-p107">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c7bd-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
