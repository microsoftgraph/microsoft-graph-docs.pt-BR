---
title: Grupos de roteamento áudio de lista
description: Recupere uma lista de objetos **audioRoutingGroup** .
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 02a782af2bb7690cc55dd3a4632aeb0cf93734da
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518524"
---
# <a name="list-audio-routing-groups"></a><span data-ttu-id="fa94a-103">Grupos de roteamento áudio de lista</span><span class="sxs-lookup"><span data-stu-id="fa94a-103">List audio routing groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa94a-104">Recupere uma lista de objetos **audioRoutingGroup** .</span><span class="sxs-lookup"><span data-stu-id="fa94a-104">Retrieve a list of **audioRoutingGroup** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa94a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa94a-105">Permissions</span></span>
<span data-ttu-id="fa94a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa94a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa94a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa94a-108">Permission type</span></span>                        | <span data-ttu-id="fa94a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa94a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fa94a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa94a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa94a-111">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="fa94a-111">Not Supported.</span></span>                               |
| <span data-ttu-id="fa94a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa94a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa94a-113">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="fa94a-113">Not Supported.</span></span>                               |
| <span data-ttu-id="fa94a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa94a-114">Application</span></span>     | <span data-ttu-id="fa94a-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="fa94a-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa94a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa94a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups
GET /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa94a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fa94a-117">Optional query parameters</span></span>
<span data-ttu-id="fa94a-118">Este método oferece suporte para os [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fa94a-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa94a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa94a-119">Request headers</span></span>
| <span data-ttu-id="fa94a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="fa94a-120">Name</span></span>          | <span data-ttu-id="fa94a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa94a-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="fa94a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa94a-122">Authorization</span></span> | <span data-ttu-id="fa94a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa94a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa94a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa94a-125">Request body</span></span>
<span data-ttu-id="fa94a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa94a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa94a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa94a-127">Response</span></span>
<span data-ttu-id="fa94a-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa94a-128">If successful, this method returns a `200 OK` response code and a collection of [audioRoutingGroup](../resources/audioroutinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa94a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa94a-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fa94a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa94a-130">Request</span></span>
<span data-ttu-id="fa94a-131">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa94a-131">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroups"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
```

##### <a name="response"></a><span data-ttu-id="fa94a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa94a-132">Response</span></span>

> <span data-ttu-id="fa94a-p103">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa94a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup",
  "isCollection": true 
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "value": [
    {
      "id": "oneToOne",
      "routingMode": "oneToOne",
      "sources": [
        "632899f8-2ea1-4604-8413-27bd2892079f"
      ],
      "receivers": [
        "550fae72-d251-43ec-868c-373732c2704f",
        "72f988bf-86f1-41af-91ab-2d7cd011db47"
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List audioRoutingGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-list-audioroutinggroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
