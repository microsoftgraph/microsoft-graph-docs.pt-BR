---
title: Listar grupos de roteamento de áudio
description: Recupere uma lista de objetos **audioRoutingGroup** .
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f526363176163185870ed92eb38388c41890a8f6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864763"
---
# <a name="list-audio-routing-groups"></a><span data-ttu-id="3e2b0-103">Listar grupos de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="3e2b0-103">List audio routing groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e2b0-104">Recupere uma lista de objetos **audioRoutingGroup** .</span><span class="sxs-lookup"><span data-stu-id="3e2b0-104">Retrieve a list of **audioRoutingGroup** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e2b0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e2b0-105">Permissions</span></span>
<span data-ttu-id="3e2b0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e2b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e2b0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e2b0-108">Permission type</span></span>                        | <span data-ttu-id="3e2b0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e2b0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3e2b0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e2b0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e2b0-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e2b0-111">Not Supported.</span></span>                               |
| <span data-ttu-id="3e2b0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e2b0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e2b0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e2b0-113">Not Supported.</span></span>                               |
| <span data-ttu-id="3e2b0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e2b0-114">Application</span></span>     | <span data-ttu-id="3e2b0-115">Calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="3e2b0-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e2b0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e2b0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups
GET /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3e2b0-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3e2b0-117">Optional query parameters</span></span>
<span data-ttu-id="3e2b0-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3e2b0-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e2b0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e2b0-119">Request headers</span></span>
| <span data-ttu-id="3e2b0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3e2b0-120">Name</span></span>          | <span data-ttu-id="3e2b0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e2b0-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3e2b0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e2b0-122">Authorization</span></span> | <span data-ttu-id="3e2b0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e2b0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e2b0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e2b0-125">Request body</span></span>
<span data-ttu-id="3e2b0-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3e2b0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e2b0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e2b0-127">Response</span></span>
<span data-ttu-id="3e2b0-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e2b0-128">If successful, this method returns a `200 OK` response code and a collection of [audioRoutingGroup](../resources/audioroutinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e2b0-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e2b0-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3e2b0-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e2b0-130">Request</span></span>
<span data-ttu-id="3e2b0-131">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e2b0-131">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3e2b0-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e2b0-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroups"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3e2b0-133">C#</span><span class="sxs-lookup"><span data-stu-id="3e2b0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-audioroutinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e2b0-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="3e2b0-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-audioroutinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3e2b0-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3e2b0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-audioroutinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3e2b0-136">Java</span><span class="sxs-lookup"><span data-stu-id="3e2b0-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-audioroutinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3e2b0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e2b0-137">Response</span></span>

> <span data-ttu-id="3e2b0-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e2b0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}
-->
