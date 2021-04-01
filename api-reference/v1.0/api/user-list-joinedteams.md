---
title: Listar joinedTeams
description: Obtenha as equipes do Microsoft Teams das quais o usuário é um membro direto.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ccf12a37db65770106397b2ba4547902529b26e7
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51474099"
---
# <a name="list-joinedteams"></a><span data-ttu-id="d8dcd-103">Listar joinedTeams</span><span class="sxs-lookup"><span data-stu-id="d8dcd-103">List joinedTeams</span></span>

<span data-ttu-id="d8dcd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8dcd-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="d8dcd-105">Obtenha as [equipes](../resources/team.md) do Microsoft Teams das quais o usuário é um membro direto.</span><span class="sxs-lookup"><span data-stu-id="d8dcd-105">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="d8dcd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8dcd-106">Permissions</span></span>
<span data-ttu-id="d8dcd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8dcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8dcd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8dcd-109">Permission type</span></span>      | <span data-ttu-id="d8dcd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8dcd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8dcd-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8dcd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d8dcd-112">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8dcd-112">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="d8dcd-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8dcd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8dcd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8dcd-114">Not supported.</span></span>    |
|<span data-ttu-id="d8dcd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8dcd-115">Application</span></span> | <span data-ttu-id="d8dcd-116">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8dcd-116">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="d8dcd-117">Com permissões de usuário delegado esta operação só funciona para o usuário "eu".</span><span class="sxs-lookup"><span data-stu-id="d8dcd-117">With user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="d8dcd-118">Com permissões de aplicativo, funciona para todos os usuários especificando a id de usuário específico. ("eu" alias não é compatível com permissões de aplicativo)</span><span class="sxs-lookup"><span data-stu-id="d8dcd-118">With application permissions, it works for all users by specifying  the specific user id. ('me' alias is not supported with application permissions)</span></span>

## <a name="http-request"></a><span data-ttu-id="d8dcd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8dcd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d8dcd-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d8dcd-120">Optional query parameters</span></span>
<span data-ttu-id="d8dcd-121">Atualmente, os [Parâmetros de consulta OData](/graph/query-parameters) não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="d8dcd-121">The [OData Query Parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d8dcd-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8dcd-122">Request headers</span></span>
| <span data-ttu-id="d8dcd-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8dcd-123">Header</span></span>       | <span data-ttu-id="d8dcd-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d8dcd-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d8dcd-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8dcd-125">Authorization</span></span>  | <span data-ttu-id="d8dcd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8dcd-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d8dcd-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d8dcd-128">Accept</span></span>  | <span data-ttu-id="d8dcd-129">application/json</span><span class="sxs-lookup"><span data-stu-id="d8dcd-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8dcd-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8dcd-130">Request body</span></span>
<span data-ttu-id="d8dcd-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d8dcd-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8dcd-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8dcd-132">Response</span></span>

<span data-ttu-id="d8dcd-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8dcd-133">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d8dcd-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8dcd-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8dcd-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8dcd-135">Request</span></span>
<span data-ttu-id="d8dcd-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8dcd-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d8dcd-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8dcd-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/joinedTeams
```
# <a name="c"></a>[<span data-ttu-id="d8dcd-138">C#</span><span class="sxs-lookup"><span data-stu-id="d8dcd-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-joinedteams-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8dcd-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8dcd-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-joinedteams-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8dcd-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8dcd-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-joinedteams-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d8dcd-141">Java</span><span class="sxs-lookup"><span data-stu-id="d8dcd-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-joinedteams-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d8dcd-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8dcd-142">Response</span></span>
<span data-ttu-id="d8dcd-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8dcd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "31aa74dd-dd65-43ac-8c4e-0ec1ae5a8ee1"
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="d8dcd-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="d8dcd-146">See also</span></span>
[<span data-ttu-id="d8dcd-147">Listar todas as equipes</span><span class="sxs-lookup"><span data-stu-id="d8dcd-147">List all teams</span></span>](/graph/teams-list-all-teams)

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
