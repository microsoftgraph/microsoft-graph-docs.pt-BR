---
title: Obter equipe
description: Recupere as propriedades e relações da equipe especificada.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3f66f20dd41da6212cda37c9a3f45c9f9dc90b26
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452572"
---
# <a name="get-team"></a><span data-ttu-id="af148-103">Obter equipe</span><span class="sxs-lookup"><span data-stu-id="af148-103">Get team</span></span>

<span data-ttu-id="af148-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af148-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af148-105">Recupere as propriedades e relações da [equipe](../resources/team.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="af148-105">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="af148-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="af148-106">Permissions</span></span>
<span data-ttu-id="af148-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af148-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af148-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af148-109">Permission type</span></span>      | <span data-ttu-id="af148-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af148-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af148-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af148-111">Delegated (work or school account)</span></span> | <span data-ttu-id="af148-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af148-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="af148-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af148-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af148-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af148-114">Not supported.</span></span>    |
|<span data-ttu-id="af148-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af148-115">Application</span></span> | <span data-ttu-id="af148-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af148-116">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="af148-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="af148-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="af148-118">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="af148-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="af148-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af148-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="af148-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="af148-120">Optional query parameters</span></span>
<span data-ttu-id="af148-121">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="af148-121">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="af148-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af148-122">Request headers</span></span>
| <span data-ttu-id="af148-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="af148-123">Header</span></span>       | <span data-ttu-id="af148-124">Valor</span><span class="sxs-lookup"><span data-stu-id="af148-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="af148-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="af148-125">Authorization</span></span>  | <span data-ttu-id="af148-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af148-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="af148-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af148-128">Request body</span></span>
<span data-ttu-id="af148-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="af148-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af148-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="af148-130">Response</span></span>

<span data-ttu-id="af148-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [team](../resources/team.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af148-131">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="af148-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af148-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="af148-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af148-133">Request</span></span>
<span data-ttu-id="af148-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="af148-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="af148-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="af148-135">Response</span></span>
<span data-ttu-id="af148-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="af148-136">The following is an example of the response.</span></span> 

><span data-ttu-id="af148-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af148-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
