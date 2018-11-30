---
title: Obtenha a equipe
description: Recupere as propriedades e relacionamentos da equipe especificado.
ms.openlocfilehash: 4ace6ef068eeafffe10af029b3193805abd8a532
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034716"
---
# <a name="get-team"></a><span data-ttu-id="bdf60-103">Obtenha a equipe</span><span class="sxs-lookup"><span data-stu-id="bdf60-103">Get team</span></span>

> <span data-ttu-id="bdf60-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bdf60-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bdf60-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bdf60-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bdf60-106">Recupere as propriedades e relacionamentos da [equipe](../resources/team.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="bdf60-106">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bdf60-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="bdf60-107">Permissions</span></span>
<span data-ttu-id="bdf60-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdf60-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdf60-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdf60-110">Permission type</span></span>      | <span data-ttu-id="bdf60-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bdf60-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdf60-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdf60-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bdf60-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdf60-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bdf60-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdf60-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdf60-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdf60-115">Not supported.</span></span>    |
|<span data-ttu-id="bdf60-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdf60-116">Application</span></span> | <span data-ttu-id="bdf60-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdf60-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="bdf60-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdf60-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bdf60-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bdf60-119">Optional query parameters</span></span>
<span data-ttu-id="bdf60-120">Este método oferece suporte a $select e $expand [OData parâmetros de consulta](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bdf60-120">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bdf60-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdf60-121">Request headers</span></span>
| <span data-ttu-id="bdf60-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bdf60-122">Header</span></span>       | <span data-ttu-id="bdf60-123">Valor</span><span class="sxs-lookup"><span data-stu-id="bdf60-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bdf60-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bdf60-124">Authorization</span></span>  | <span data-ttu-id="bdf60-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdf60-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bdf60-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bdf60-127">Request body</span></span>
<span data-ttu-id="bdf60-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bdf60-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdf60-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdf60-129">Response</span></span>

<span data-ttu-id="bdf60-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de [equipe](../resources/team.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdf60-130">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bdf60-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bdf60-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bdf60-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdf60-132">Request</span></span>
<span data-ttu-id="bdf60-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdf60-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="bdf60-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdf60-134">Response</span></span>
<span data-ttu-id="bdf60-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bdf60-135">The following is an example of the response.</span></span> 

><span data-ttu-id="bdf60-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bdf60-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
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
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
