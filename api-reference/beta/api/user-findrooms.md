---
title: 'usuário: findRooms'
description: 'Obtenha todas as salas de reunião no locatário do usuário ou em uma lista de salas específico. '
localization_priority: Priority
ms.openlocfilehash: 12ddd4c6956d743322ff86c93c5d445f6966e29a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845413"
---
# <a name="user-findrooms"></a><span data-ttu-id="d4226-103">usuário: findRooms</span><span class="sxs-lookup"><span data-stu-id="d4226-103">user: findRooms</span></span>

> <span data-ttu-id="d4226-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d4226-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4226-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d4226-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d4226-106">Obtenha todas as salas de reunião no locatário do usuário ou em uma lista de salas específico.</span><span class="sxs-lookup"><span data-stu-id="d4226-106">Get all the meeting rooms in the user's tenant or in a specific room list.</span></span> 

<span data-ttu-id="d4226-107">Inquilinos podem organizar as salas de reunião em listas de salas.</span><span class="sxs-lookup"><span data-stu-id="d4226-107">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="d4226-108">Cada sala de reunião e a lista de salas é representado por uma instância de [emailAddress](../resources/emailaddress.md) .</span><span class="sxs-lookup"><span data-stu-id="d4226-108">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span> <span data-ttu-id="d4226-109">Você pode [fazer todas as listas de sala](user-findroomlists.md) no locatário, fazer todas as salas no locatário ou fazer todas as salas em uma lista de sala específico.</span><span class="sxs-lookup"><span data-stu-id="d4226-109">You can [get all the room lists](user-findroomlists.md) in the tenant, get all the rooms in the tenant, or get all the rooms in a specific room list.</span></span> <span data-ttu-id="d4226-110">Você pode acessar as primeiras 100 salas no inquilino.</span><span class="sxs-lookup"><span data-stu-id="d4226-110">You can get up to the first 100 rooms in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4226-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="d4226-111">Permissions</span></span>
<span data-ttu-id="d4226-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4226-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d4226-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4226-114">Permission type</span></span>      | <span data-ttu-id="d4226-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4226-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4226-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4226-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d4226-117">User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4226-117">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="d4226-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4226-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4226-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4226-119">Not supported.</span></span>    |
|<span data-ttu-id="d4226-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4226-120">Application</span></span> | <span data-ttu-id="d4226-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4226-121">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4226-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4226-122">HTTP request</span></span>

<span data-ttu-id="d4226-123">Para obter todas as salas no locatário:</span><span class="sxs-lookup"><span data-stu-id="d4226-123">To get all the rooms in the tenant:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/<id>/findRooms
```

<span data-ttu-id="d4226-124">Para obter todas as salas em uma lista de sala específico de locatário:</span><span class="sxs-lookup"><span data-stu-id="d4226-124">To get all the rooms in a specific room list of the tenant's:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list}')
GET /users/<id>/findRooms(RoomList='{room_list}')
```

## <a name="query-parameters"></a><span data-ttu-id="d4226-125">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="d4226-125">Query parameters</span></span>

| <span data-ttu-id="d4226-126">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="d4226-126">Query parameter</span></span>       | <span data-ttu-id="d4226-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4226-127">Type</span></span> | <span data-ttu-id="d4226-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4226-128">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="d4226-129">RoomList</span><span class="sxs-lookup"><span data-stu-id="d4226-129">RoomList</span></span> | <span data-ttu-id="d4226-130">string</span><span class="sxs-lookup"><span data-stu-id="d4226-130">string</span></span> | <span data-ttu-id="d4226-131">Endereço SMTP associado à lista de salas.</span><span class="sxs-lookup"><span data-stu-id="d4226-131">The SMTP address associated with the room list.</span></span> <span data-ttu-id="d4226-132">Cada lista de salas é representada por uma instância de [emailAddress](../resources/emailaddress.md) que inclui um endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="d4226-132">Each room list is represented by an [emailAddress](../resources/emailaddress.md) instance that includes an SMTP address.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d4226-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4226-133">Request headers</span></span>
| <span data-ttu-id="d4226-134">Nome</span><span class="sxs-lookup"><span data-stu-id="d4226-134">Name</span></span>       | <span data-ttu-id="d4226-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4226-135">Type</span></span> | <span data-ttu-id="d4226-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4226-136">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="d4226-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4226-137">Authorization</span></span>  | <span data-ttu-id="d4226-138">string</span><span class="sxs-lookup"><span data-stu-id="d4226-138">string</span></span>  | <span data-ttu-id="d4226-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4226-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d4226-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d4226-141">Content-Type</span></span>  | <span data-ttu-id="d4226-142">string</span><span class="sxs-lookup"><span data-stu-id="d4226-142">string</span></span>  | <span data-ttu-id="d4226-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4226-p106">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="d4226-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4226-145">Request body</span></span>
<span data-ttu-id="d4226-146">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4226-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4226-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4226-147">Response</span></span>

<span data-ttu-id="d4226-148">Se tiver êxito, este método retornará um `200 OK` objeto de coleção [emailAddress](../resources/emailaddress.md) e código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4226-148">If successful, this method returns a `200 OK` response code and [emailAddress](../resources/emailaddress.md) collection object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="d4226-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4226-149">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="d4226-150">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="d4226-150">Request 1</span></span>

<span data-ttu-id="d4226-151">O exemplo primeiro obtém todas as salas definidas no locatário do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="d4226-151">The first example gets all the rooms defined in the signed-in user's tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms
```

##### <a name="response-1"></a><span data-ttu-id="d4226-152">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="d4226-152">Response 1</span></span>
<span data-ttu-id="d4226-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4226-153">Here is an example of the response.</span></span> 

<span data-ttu-id="d4226-p107">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4226-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="d4226-156">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="d4226-156">Request 2</span></span>

<span data-ttu-id="d4226-157">O segundo exemplo obtém as salas na lista de sala especificado identificado pelo endereço de email Building2Rooms@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="d4226-157">The second example gets the rooms in the specified room list identified by the email address Building2Rooms@contoso.onmicrosoft.com.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```

##### <a name="response-2"></a><span data-ttu-id="d4226-158">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="d4226-158">Response 2</span></span>
<span data-ttu-id="d4226-159">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4226-159">Here is an example of the response.</span></span> 

<span data-ttu-id="d4226-p108">Observação: o objeto da resposta mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4226-p108">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "user: findRooms",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
