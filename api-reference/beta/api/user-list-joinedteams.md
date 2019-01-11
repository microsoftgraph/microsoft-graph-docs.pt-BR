---
title: Listar joinedTeams
description: Obtenha as equipes no Microsoft Teams que o usuário é um membro direto.
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 4f412d8721439a948bec1b07f628ce1f27dcf717
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839442"
---
# <a name="list-joinedteams"></a><span data-ttu-id="2907a-103">Listar joinedTeams</span><span class="sxs-lookup"><span data-stu-id="2907a-103">List joinedTeams</span></span>

> <span data-ttu-id="2907a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2907a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2907a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2907a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2907a-106">Obtenha as [equipes](../resources/team.md) no Microsoft Teams que o usuário é um membro direto.</span><span class="sxs-lookup"><span data-stu-id="2907a-106">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="2907a-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="2907a-107">Permissions</span></span>
<span data-ttu-id="2907a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2907a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2907a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2907a-110">Permission type</span></span>      | <span data-ttu-id="2907a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2907a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2907a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2907a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2907a-113">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2907a-113">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="2907a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2907a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2907a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2907a-115">Not supported.</span></span>    |
|<span data-ttu-id="2907a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2907a-116">Application</span></span> | <span data-ttu-id="2907a-117">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2907a-117">User.Read.All, User.ReadWrite.All</span></span> |

> <span data-ttu-id="2907a-118">Atualmente, com permissões de usuário delegado essa operação só funciona para 'me' usuário.</span><span class="sxs-lookup"><span data-stu-id="2907a-118">Currently, with user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="2907a-119">Com as permissões de aplicativo, ele funciona para todos os usuários, especificando a id de usuário específico. ('me' alias não é suportado com permissões de aplicativo) Para obter detalhes, consulte [problemas conhecidos](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview).</span><span class="sxs-lookup"><span data-stu-id="2907a-119">With application permissions, it works for all users by specifying  the specific user  id. ('me' alias is not supported with application permissions) For details, see [Known issues](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview).</span></span>

## <a name="http-request"></a><span data-ttu-id="2907a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2907a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2907a-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2907a-121">Optional query parameters</span></span>
<span data-ttu-id="2907a-122">Os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) não são suportados no momento.</span><span class="sxs-lookup"><span data-stu-id="2907a-122">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2907a-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2907a-123">Request headers</span></span>
| <span data-ttu-id="2907a-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2907a-124">Header</span></span>       | <span data-ttu-id="2907a-125">Valor</span><span class="sxs-lookup"><span data-stu-id="2907a-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2907a-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="2907a-126">Authorization</span></span>  | <span data-ttu-id="2907a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2907a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2907a-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2907a-129">Accept</span></span>  | <span data-ttu-id="2907a-130">application/json</span><span class="sxs-lookup"><span data-stu-id="2907a-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2907a-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2907a-131">Request body</span></span>
<span data-ttu-id="2907a-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2907a-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2907a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2907a-133">Response</span></span>

<span data-ttu-id="2907a-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2907a-134">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2907a-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2907a-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2907a-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2907a-136">Request</span></span>
<span data-ttu-id="2907a-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2907a-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```http
GET https://graph.microsoft.com/beta/me/joinedTeams
```
##### <a name="response"></a><span data-ttu-id="2907a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2907a-138">Response</span></span>
<span data-ttu-id="2907a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2907a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="2907a-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="2907a-142">See also</span></span>
[<span data-ttu-id="2907a-143">Liste todas as equipes</span><span class="sxs-lookup"><span data-stu-id="2907a-143">List all teams</span></span>](/graph/teams-list-all-teams)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
