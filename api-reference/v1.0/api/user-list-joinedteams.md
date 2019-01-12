---
title: Listar joinedTeams
description: Obtenha as equipes no Microsoft Teams que o usuário é um membro direto.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f2c5c67234a6e847327c28e61e7ccb2294b36d54
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980853"
---
# <a name="list-joinedteams"></a><span data-ttu-id="2c105-103">Listar joinedTeams</span><span class="sxs-lookup"><span data-stu-id="2c105-103">List joinedTeams</span></span>



<span data-ttu-id="2c105-104">Obtenha as [equipes](../resources/team.md) no Microsoft Teams que o usuário é um membro direto.</span><span class="sxs-lookup"><span data-stu-id="2c105-104">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="2c105-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2c105-105">Permissions</span></span>
<span data-ttu-id="2c105-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c105-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c105-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c105-108">Permission type</span></span>      | <span data-ttu-id="2c105-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c105-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c105-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c105-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2c105-111">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c105-111">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c105-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c105-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c105-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c105-113">Not supported.</span></span>    |
|<span data-ttu-id="2c105-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c105-114">Application</span></span> | <span data-ttu-id="2c105-115">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c105-115">User.Read.All, User.ReadWrite.All</span></span> |

> <span data-ttu-id="2c105-116">Com as permissões de usuário delegado essa operação só funciona para 'me' usuário.</span><span class="sxs-lookup"><span data-stu-id="2c105-116">With user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="2c105-117">Com as permissões de aplicativo, ele funciona para todos os usuários, especificando a id de usuário específico. ('me' alias não é suportado com permissões de aplicativo)</span><span class="sxs-lookup"><span data-stu-id="2c105-117">With application permissions, it works for all users by specifying  the specific user id. ('me' alias is not supported with application permissions)</span></span>

## <a name="http-request"></a><span data-ttu-id="2c105-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c105-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2c105-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2c105-119">Optional query parameters</span></span>
<span data-ttu-id="2c105-120">Os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) não são suportados no momento.</span><span class="sxs-lookup"><span data-stu-id="2c105-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c105-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c105-121">Request headers</span></span>
| <span data-ttu-id="2c105-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2c105-122">Header</span></span>       | <span data-ttu-id="2c105-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2c105-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2c105-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c105-124">Authorization</span></span>  | <span data-ttu-id="2c105-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c105-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2c105-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2c105-127">Accept</span></span>  | <span data-ttu-id="2c105-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2c105-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c105-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c105-129">Request body</span></span>
<span data-ttu-id="2c105-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2c105-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c105-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c105-131">Response</span></span>

<span data-ttu-id="2c105-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c105-132">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2c105-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c105-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c105-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c105-134">Request</span></span>
<span data-ttu-id="2c105-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c105-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```http
GET https://graph.microsoft.com/beta/me/joinedTeams
```
##### <a name="response"></a><span data-ttu-id="2c105-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c105-136">Response</span></span>
<span data-ttu-id="2c105-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2c105-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="2c105-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="2c105-140">See also</span></span>
[<span data-ttu-id="2c105-141">Liste todas as equipes</span><span class="sxs-lookup"><span data-stu-id="2c105-141">List all teams</span></span>](/graph/teams-list-all-teams)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
