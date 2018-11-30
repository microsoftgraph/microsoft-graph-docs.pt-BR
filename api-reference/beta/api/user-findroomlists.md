---
title: 'usuário: findRoomLists'
description: Obtenha as listas de salas definidas em um locatário.
ms.openlocfilehash: 5857d5381252fc00c9b159c8a0a7eecd71de2a08
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27032924"
---
# <a name="user-findroomlists"></a><span data-ttu-id="e1540-103">usuário: findRoomLists</span><span class="sxs-lookup"><span data-stu-id="e1540-103">user: findRoomLists</span></span>

> <span data-ttu-id="e1540-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e1540-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1540-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e1540-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e1540-106">Obtenha as listas de salas definidas em um locatário.</span><span class="sxs-lookup"><span data-stu-id="e1540-106">Get the room lists defined in a tenant.</span></span>

<span data-ttu-id="e1540-107">Inquilinos podem organizar as salas de reunião em listas de salas.</span><span class="sxs-lookup"><span data-stu-id="e1540-107">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="e1540-108">Cada sala de reunião e a lista de salas é representado por uma instância de [emailAddress](../resources/emailaddress.md) .</span><span class="sxs-lookup"><span data-stu-id="e1540-108">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span>
<span data-ttu-id="e1540-109">Você pode obter todas as listas de sala no locatário, [fazer todas as salas](user-findrooms.md) no locatário ou [fazer todas as salas](user-findrooms.md) em uma lista de sala específico.</span><span class="sxs-lookup"><span data-stu-id="e1540-109">You can get all the room lists in the tenant, [get all the rooms](user-findrooms.md) in the tenant, or [get all the rooms](user-findrooms.md) in a specific room list.</span></span>


## <a name="permissions"></a><span data-ttu-id="e1540-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="e1540-110">Permissions</span></span>
<span data-ttu-id="e1540-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1540-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e1540-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1540-113">Permission type</span></span>      | <span data-ttu-id="e1540-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1540-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1540-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1540-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e1540-116">User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1540-116">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="e1540-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1540-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1540-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1540-118">Not supported.</span></span>    |
|<span data-ttu-id="e1540-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1540-119">Application</span></span> | <span data-ttu-id="e1540-120">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1540-120">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1540-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1540-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/findRoomLists
GET /users/<id>/findRoomLists

```

## <a name="request-headers"></a><span data-ttu-id="e1540-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1540-122">Request headers</span></span>
| <span data-ttu-id="e1540-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e1540-123">Name</span></span>       | <span data-ttu-id="e1540-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1540-124">Type</span></span> | <span data-ttu-id="e1540-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1540-125">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="e1540-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1540-126">Authorization</span></span>  | <span data-ttu-id="e1540-127">string</span><span class="sxs-lookup"><span data-stu-id="e1540-127">string</span></span>  | <span data-ttu-id="e1540-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1540-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e1540-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e1540-130">Content-Type</span></span>  | <span data-ttu-id="e1540-131">string</span><span class="sxs-lookup"><span data-stu-id="e1540-131">string</span></span>  | <span data-ttu-id="e1540-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1540-p105">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e1540-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1540-134">Request body</span></span>
<span data-ttu-id="e1540-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1540-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1540-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1540-136">Response</span></span>

<span data-ttu-id="e1540-137">Se tiver êxito, este método retornará um `200 OK` objeto de coleção [emailAddress](../resources/emailaddress.md) e código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1540-137">If successful, this method returns a `200 OK` response code and [emailAddress](../resources/emailaddress.md) collection object in the response body.</span></span>

<span data-ttu-id="e1540-138">Se nenhuma lista for definida no locatário, uma matriz vazia será retornada.</span><span class="sxs-lookup"><span data-stu-id="e1540-138">If no lists are defined in the tenant, then an empty array is returned.</span></span>

## <a name="example"></a><span data-ttu-id="e1540-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1540-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1540-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1540-140">Request</span></span>

<span data-ttu-id="e1540-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1540-141">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_room_lists"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRoomLists
```

##### <a name="response"></a><span data-ttu-id="e1540-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1540-142">Response</span></span>
<span data-ttu-id="e1540-143">Este é um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1540-143">Here is an example of the response.</span></span> 

<span data-ttu-id="e1540-p106">Observação: o objeto da resposta mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1540-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "user: findRoomLists",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->