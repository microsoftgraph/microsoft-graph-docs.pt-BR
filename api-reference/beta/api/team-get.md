---
title: Obter equipe
description: Recupere as propriedades e relações da equipe especificada.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a1ce7a8eb9e584d9654872f58787de8f51ec3ec6
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332482"
---
# <a name="get-team"></a><span data-ttu-id="93f22-103">Obter equipe</span><span class="sxs-lookup"><span data-stu-id="93f22-103">Get team</span></span>

<span data-ttu-id="93f22-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93f22-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93f22-105">Recupere as propriedades e relações da [equipe](../resources/team.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="93f22-105">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="93f22-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="93f22-106">Permissions</span></span>
<span data-ttu-id="93f22-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93f22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93f22-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93f22-109">Permission type</span></span>      | <span data-ttu-id="93f22-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93f22-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93f22-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93f22-111">Delegated (work or school account)</span></span> | <span data-ttu-id="93f22-112">Team. ReadBasic. All, TeamSettings. Read. All, TeamSettings. ReadWrite. All, Group. Read. All, Group. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="93f22-112">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="93f22-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93f22-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93f22-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93f22-114">Not supported.</span></span>    |
|<span data-ttu-id="93f22-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93f22-115">Application</span></span> | <span data-ttu-id="93f22-116">TeamSettings. Read. Group ([RSC](https://aka.ms/teams-rsc)), Team. ReadBasic. All, TeamSettings. Read. All, TeamSettings. ReadWrite. All, TeamSettings. Edit. Group ([RSC](https://aka.ms/teams-rsc)), Group. Read. All, Group. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="93f22-116">TeamSettings.Read.Group ([RSC](https://aka.ms/teams-rsc)), Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, TeamSettings.Edit.Group ([RSC](https://aka.ms/teams-rsc)), Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |

> <span data-ttu-id="93f22-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="93f22-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="93f22-118">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="93f22-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="93f22-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93f22-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="93f22-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="93f22-120">Optional query parameters</span></span>
<span data-ttu-id="93f22-121">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="93f22-121">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93f22-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93f22-122">Request headers</span></span>
| <span data-ttu-id="93f22-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="93f22-123">Header</span></span>       | <span data-ttu-id="93f22-124">Valor</span><span class="sxs-lookup"><span data-stu-id="93f22-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="93f22-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="93f22-125">Authorization</span></span>  | <span data-ttu-id="93f22-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93f22-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="93f22-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93f22-128">Request body</span></span>
<span data-ttu-id="93f22-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="93f22-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93f22-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="93f22-130">Response</span></span>

<span data-ttu-id="93f22-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [team](../resources/team.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93f22-131">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="93f22-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93f22-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="93f22-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93f22-133">Request</span></span>
<span data-ttu-id="93f22-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="93f22-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="93f22-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="93f22-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_team"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}
```
# <a name="c"></a>[<span data-ttu-id="93f22-136">C#</span><span class="sxs-lookup"><span data-stu-id="93f22-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93f22-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93f22-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93f22-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93f22-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="93f22-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="93f22-139">Response</span></span>
<span data-ttu-id="93f22-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="93f22-140">The following is an example of the response.</span></span> 

><span data-ttu-id="93f22-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93f22-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "isArchived" : false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true    
  },
  "guestSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true 
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true    
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  },
  "discoverySettings": {
    "showInTeamsSearchAndSuggestions": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
