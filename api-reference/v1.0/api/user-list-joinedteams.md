---
title: Listar joinedTeams
description: Obtenha as equipes do Microsoft Teams das quais o usuário é um membro direto.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 629ec201a93c1947637143785d61f2a2f971a307
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460368"
---
# <a name="list-joinedteams"></a><span data-ttu-id="ac235-103">Listar joinedTeams</span><span class="sxs-lookup"><span data-stu-id="ac235-103">List joinedTeams</span></span>



<span data-ttu-id="ac235-104">Obtenha as [equipes](../resources/team.md) do Microsoft Teams das quais o usuário é um membro direto.</span><span class="sxs-lookup"><span data-stu-id="ac235-104">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="ac235-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac235-105">Permissions</span></span>
<span data-ttu-id="ac235-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac235-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac235-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac235-108">Permission type</span></span>      | <span data-ttu-id="ac235-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac235-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac235-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac235-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ac235-111">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac235-111">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="ac235-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac235-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac235-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac235-113">Not supported.</span></span>    |
|<span data-ttu-id="ac235-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac235-114">Application</span></span> | <span data-ttu-id="ac235-115">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac235-115">User.Read.All, User.ReadWrite.All</span></span> |

> <span data-ttu-id="ac235-116">Com permissões de usuário delegado esta operação só funciona para o usuário "eu".</span><span class="sxs-lookup"><span data-stu-id="ac235-116">With user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="ac235-117">Com permissões de aplicativo, funciona para todos os usuários especificando a id de usuário específico. ("eu" alias não é compatível com permissões de aplicativo)</span><span class="sxs-lookup"><span data-stu-id="ac235-117">With application permissions, it works for all users by specifying  the specific user id. ('me' alias is not supported with application permissions)</span></span>

## <a name="http-request"></a><span data-ttu-id="ac235-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac235-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ac235-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ac235-119">Optional query parameters</span></span>
<span data-ttu-id="ac235-120">Atualmente, os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="ac235-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac235-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac235-121">Request headers</span></span>
| <span data-ttu-id="ac235-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ac235-122">Header</span></span>       | <span data-ttu-id="ac235-123">Valor</span><span class="sxs-lookup"><span data-stu-id="ac235-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ac235-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac235-124">Authorization</span></span>  | <span data-ttu-id="ac235-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac235-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ac235-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ac235-127">Accept</span></span>  | <span data-ttu-id="ac235-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ac235-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac235-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac235-129">Request body</span></span>
<span data-ttu-id="ac235-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ac235-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac235-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac235-131">Response</span></span>

<span data-ttu-id="ac235-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac235-132">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ac235-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac235-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ac235-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac235-134">Request</span></span>
<span data-ttu-id="ac235-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac235-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ac235-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac235-136">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/joinedTeams
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ac235-137">C#</span><span class="sxs-lookup"><span data-stu-id="ac235-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-joinedteams-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ac235-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="ac235-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-joinedteams-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ac235-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac235-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-joinedteams-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ac235-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac235-140">Response</span></span>
<span data-ttu-id="ac235-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac235-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ac235-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="ac235-144">See also</span></span>
[<span data-ttu-id="ac235-145">Listar todas as equipes</span><span class="sxs-lookup"><span data-stu-id="ac235-145">List all teams</span></span>](/graph/teams-list-all-teams)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
