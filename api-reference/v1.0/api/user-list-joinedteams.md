---
title: Listar joinedTeams
description: Obtenha as equipes do Microsoft Teams das quais o usuário é um membro direto.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 391753de88ae9a7dd1abd712cec6a711d964d304
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274918"
---
# <a name="list-joinedteams"></a><span data-ttu-id="3c613-103">Listar joinedTeams</span><span class="sxs-lookup"><span data-stu-id="3c613-103">List joinedTeams</span></span>



<span data-ttu-id="3c613-104">Obtenha as [equipes](../resources/team.md) do Microsoft Teams das quais o usuário é um membro direto.</span><span class="sxs-lookup"><span data-stu-id="3c613-104">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="3c613-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c613-105">Permissions</span></span>
<span data-ttu-id="3c613-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c613-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c613-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c613-108">Permission type</span></span>      | <span data-ttu-id="3c613-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c613-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c613-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c613-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3c613-111">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c613-111">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="3c613-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c613-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c613-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c613-113">Not supported.</span></span>    |
|<span data-ttu-id="3c613-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c613-114">Application</span></span> | <span data-ttu-id="3c613-115">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c613-115">User.Read.All, User.ReadWrite.All</span></span> |

> <span data-ttu-id="3c613-116">Com permissões de usuário delegado esta operação só funciona para o usuário "eu".</span><span class="sxs-lookup"><span data-stu-id="3c613-116">With user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="3c613-117">Com permissões de aplicativo, funciona para todos os usuários especificando a id de usuário específico. ("eu" alias não é compatível com permissões de aplicativo)</span><span class="sxs-lookup"><span data-stu-id="3c613-117">With application permissions, it works for all users by specifying  the specific user id. ('me' alias is not supported with application permissions)</span></span>

## <a name="http-request"></a><span data-ttu-id="3c613-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c613-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c613-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3c613-119">Optional query parameters</span></span>
<span data-ttu-id="3c613-120">Atualmente, os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="3c613-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c613-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c613-121">Request headers</span></span>
| <span data-ttu-id="3c613-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c613-122">Header</span></span>       | <span data-ttu-id="3c613-123">Valor</span><span class="sxs-lookup"><span data-stu-id="3c613-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3c613-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c613-124">Authorization</span></span>  | <span data-ttu-id="3c613-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c613-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3c613-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3c613-127">Accept</span></span>  | <span data-ttu-id="3c613-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3c613-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c613-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c613-129">Request body</span></span>
<span data-ttu-id="3c613-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c613-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c613-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c613-131">Response</span></span>

<span data-ttu-id="3c613-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c613-132">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3c613-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c613-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c613-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c613-134">Request</span></span>
<span data-ttu-id="3c613-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c613-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/joinedTeams
```
##### <a name="response"></a><span data-ttu-id="3c613-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c613-136">Response</span></span>
<span data-ttu-id="3c613-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c613-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3c613-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3c613-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3c613-141">C#</span><span class="sxs-lookup"><span data-stu-id="3c613-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_joinedteams-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c613-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="3c613-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_joinedteams-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3c613-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c613-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_joinedteams-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="3c613-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="3c613-144">See also</span></span>
[<span data-ttu-id="3c613-145">Listar todas as equipes</span><span class="sxs-lookup"><span data-stu-id="3c613-145">List all teams</span></span>](/graph/teams-list-all-teams)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-list-joinedteams.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-list-joinedteams.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list-joinedteams.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
