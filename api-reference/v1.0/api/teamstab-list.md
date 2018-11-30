---
title: Guias de lista no canal
description: 'Recupere a lista das guias no canal especificado dentro de uma equipe. '
ms.openlocfilehash: 3d86b9fd4980309adeb952c71affd943b1587808
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006000"
---
# <a name="list-tabs-in-channel"></a><span data-ttu-id="8b3e7-103">Guias de lista no canal</span><span class="sxs-lookup"><span data-stu-id="8b3e7-103">List tabs in channel</span></span>



<span data-ttu-id="8b3e7-104">Recupere a lista das [guias](../resources/teamstab.md) no [canal](../resources/channel.md) especificado dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="8b3e7-104">Retrieve the list of [tabs](../resources/teamstab.md) in the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="8b3e7-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="8b3e7-105">Permissions</span></span>
<span data-ttu-id="8b3e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b3e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b3e7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b3e7-108">Permission type</span></span>      | <span data-ttu-id="8b3e7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b3e7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b3e7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b3e7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8b3e7-111">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b3e7-111">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="8b3e7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b3e7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b3e7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b3e7-113">Not supported.</span></span>    |
| <span data-ttu-id="8b3e7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b3e7-114">Application</span></span>                            | <span data-ttu-id="8b3e7-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b3e7-115">Group.Read.All, Group.ReadWrite.All</span></span>         |

## <a name="http-request"></a><span data-ttu-id="8b3e7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b3e7-116">HTTP request</span></span>

```http
GET /teams/{id}/channels/{id}/tabs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8b3e7-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8b3e7-117">Optional query parameters</span></span>

<span data-ttu-id="8b3e7-118">Este método oferece suporte a $filter, $select, e $expand [OData parâmetros de consulta](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8b3e7-118">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b3e7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b3e7-119">Request headers</span></span>
| <span data-ttu-id="8b3e7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8b3e7-120">Header</span></span>       | <span data-ttu-id="8b3e7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8b3e7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8b3e7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b3e7-122">Authorization</span></span>  | <span data-ttu-id="8b3e7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b3e7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8b3e7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b3e7-125">Request body</span></span>
<span data-ttu-id="8b3e7-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8b3e7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b3e7-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b3e7-127">Response</span></span>
<span data-ttu-id="8b3e7-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos de [guias](../resources/teamstab.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b3e7-128">If successful, this method returns a `200 OK` response code and collection of [tabs](../resources/teamstab.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b3e7-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b3e7-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8b3e7-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b3e7-130">Request</span></span>
<span data-ttu-id="8b3e7-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b3e7-131">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
```

#### <a name="response"></a><span data-ttu-id="8b3e7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b3e7-132">Response</span></span>
<span data-ttu-id="8b3e7-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8b3e7-133">The following is an example of the response.</span></span>
><span data-ttu-id="8b3e7-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8b3e7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "value": [
    {
      "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
      "name": "My Contoso Tab - updated",
      "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
      "configuration": {
        "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
        "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
        "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
        "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
      },
      "sortOrderIndex": 20,
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
    },
    {
      "id": "b5d5f001-0471-49a5-aac4-04ef96683be0",
      "name": "My Trello Tab",
      "teamsAppId": "23134c6b-5e4b-439c-8f70-3ded1df20805",
      "configuration": null,
      "sortOrderIndex": 21,
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3a3709b35c-a0ba-467c-8001-0f66895fb9d3?label=My%20Trello%Tab"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List all tabs in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
