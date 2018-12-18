---
title: Obtenha a equipe
description: Recupere as propriedades e relacionamentos da equipe especificado.
author: nkramer
ms.openlocfilehash: dfa59948a9bffce77c98a3462f919e75fe18042e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329229"
---
# <a name="get-team"></a><span data-ttu-id="25cfe-103">Obtenha a equipe</span><span class="sxs-lookup"><span data-stu-id="25cfe-103">Get team</span></span>

> <span data-ttu-id="25cfe-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="25cfe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="25cfe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="25cfe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="25cfe-106">Recupere as propriedades e relacionamentos da [equipe](../resources/team.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="25cfe-106">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="25cfe-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="25cfe-107">Permissions</span></span>
<span data-ttu-id="25cfe-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25cfe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25cfe-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25cfe-110">Permission type</span></span>      | <span data-ttu-id="25cfe-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="25cfe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25cfe-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25cfe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="25cfe-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25cfe-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="25cfe-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25cfe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25cfe-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25cfe-115">Not supported.</span></span>    |
|<span data-ttu-id="25cfe-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25cfe-116">Application</span></span> | <span data-ttu-id="25cfe-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25cfe-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="25cfe-118">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="25cfe-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="25cfe-119">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="25cfe-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="25cfe-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25cfe-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="25cfe-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="25cfe-121">Optional query parameters</span></span>
<span data-ttu-id="25cfe-122">Este método oferece suporte a $select e $expand [OData parâmetros de consulta](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="25cfe-122">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25cfe-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25cfe-123">Request headers</span></span>
| <span data-ttu-id="25cfe-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="25cfe-124">Header</span></span>       | <span data-ttu-id="25cfe-125">Valor</span><span class="sxs-lookup"><span data-stu-id="25cfe-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="25cfe-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="25cfe-126">Authorization</span></span>  | <span data-ttu-id="25cfe-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25cfe-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="25cfe-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25cfe-129">Request body</span></span>
<span data-ttu-id="25cfe-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="25cfe-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25cfe-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="25cfe-131">Response</span></span>

<span data-ttu-id="25cfe-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de [equipe](../resources/team.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25cfe-132">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="25cfe-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25cfe-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="25cfe-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25cfe-134">Request</span></span>
<span data-ttu-id="25cfe-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="25cfe-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="25cfe-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="25cfe-136">Response</span></span>
<span data-ttu-id="25cfe-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="25cfe-137">The following is an example of the response.</span></span> 

><span data-ttu-id="25cfe-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25cfe-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
