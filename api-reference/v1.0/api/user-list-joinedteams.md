---
title: Listar joinedTeams
description: Obtenha as equipes do Microsoft Teams das quais o usuário é um membro direto.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 597274fdd37f93c16d6d5f73e19bff79b207b223
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601798"
---
# <a name="list-joinedteams"></a><span data-ttu-id="43b07-103">Listar joinedTeams</span><span class="sxs-lookup"><span data-stu-id="43b07-103">List joinedTeams</span></span>



<span data-ttu-id="43b07-104">Obtenha as [equipes](../resources/team.md) do Microsoft Teams das quais o usuário é um membro direto.</span><span class="sxs-lookup"><span data-stu-id="43b07-104">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="43b07-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="43b07-105">Permissions</span></span>
<span data-ttu-id="43b07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43b07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43b07-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43b07-108">Permission type</span></span>      | <span data-ttu-id="43b07-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43b07-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43b07-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43b07-110">Delegated (work or school account)</span></span> | <span data-ttu-id="43b07-111">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43b07-111">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="43b07-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43b07-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43b07-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43b07-113">Not supported.</span></span>    |
|<span data-ttu-id="43b07-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43b07-114">Application</span></span> | <span data-ttu-id="43b07-115">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43b07-115">User.Read.All, User.ReadWrite.All</span></span> |

> <span data-ttu-id="43b07-116">Com permissões de usuário delegado esta operação só funciona para o usuário "eu".</span><span class="sxs-lookup"><span data-stu-id="43b07-116">With user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="43b07-117">Com permissões de aplicativo, funciona para todos os usuários especificando a id de usuário específico. ("eu" alias não é compatível com permissões de aplicativo)</span><span class="sxs-lookup"><span data-stu-id="43b07-117">With application permissions, it works for all users by specifying  the specific user id. ('me' alias is not supported with application permissions)</span></span>

## <a name="http-request"></a><span data-ttu-id="43b07-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43b07-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43b07-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="43b07-119">Optional query parameters</span></span>
<span data-ttu-id="43b07-120">Atualmente, os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="43b07-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43b07-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43b07-121">Request headers</span></span>
| <span data-ttu-id="43b07-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43b07-122">Header</span></span>       | <span data-ttu-id="43b07-123">Valor</span><span class="sxs-lookup"><span data-stu-id="43b07-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="43b07-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="43b07-124">Authorization</span></span>  | <span data-ttu-id="43b07-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43b07-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="43b07-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="43b07-127">Accept</span></span>  | <span data-ttu-id="43b07-128">application/json</span><span class="sxs-lookup"><span data-stu-id="43b07-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43b07-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43b07-129">Request body</span></span>
<span data-ttu-id="43b07-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="43b07-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43b07-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="43b07-131">Response</span></span>

<span data-ttu-id="43b07-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43b07-132">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="43b07-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43b07-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="43b07-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43b07-134">Request</span></span>
<span data-ttu-id="43b07-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="43b07-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/joinedTeams
```
##### <a name="response"></a><span data-ttu-id="43b07-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="43b07-136">Response</span></span>
<span data-ttu-id="43b07-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43b07-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="43b07-140">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="43b07-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="43b07-141">C#</span><span class="sxs-lookup"><span data-stu-id="43b07-141">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_joinedteams-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="43b07-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="43b07-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_joinedteams-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="43b07-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="43b07-143">See also</span></span>
[<span data-ttu-id="43b07-144">Listar todas as equipes</span><span class="sxs-lookup"><span data-stu-id="43b07-144">List all teams</span></span>](/graph/teams-list-all-teams)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-list-joinedteams.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list-joinedteams.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
