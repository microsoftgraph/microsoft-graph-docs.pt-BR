---
title: Listar grupos de roteamento de áudio
description: Recupere uma lista de objetos **audioRoutingGroup** .
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b1b229316370488a441ad4bacee8b92af42951c8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987390"
---
# <a name="list-audio-routing-groups"></a><span data-ttu-id="396d8-103">Listar grupos de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="396d8-103">List audio routing groups</span></span>

<span data-ttu-id="396d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="396d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="396d8-105">Recupere uma lista de objetos **audioRoutingGroup** .</span><span class="sxs-lookup"><span data-stu-id="396d8-105">Retrieve a list of **audioRoutingGroup** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="396d8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="396d8-106">Permissions</span></span>
<span data-ttu-id="396d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="396d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="396d8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="396d8-109">Permission type</span></span>                        | <span data-ttu-id="396d8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="396d8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="396d8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="396d8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="396d8-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="396d8-112">Not Supported.</span></span>                               |
| <span data-ttu-id="396d8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="396d8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="396d8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="396d8-114">Not Supported.</span></span>                               |
| <span data-ttu-id="396d8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="396d8-115">Application</span></span>     | <span data-ttu-id="396d8-116">Calls. JoinGroupCalls. All, Calls.InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="396d8-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="396d8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="396d8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups
GET /communications/calls/{id}/audioRoutingGroups
```
> <span data-ttu-id="396d8-118">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="396d8-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="396d8-119">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="396d8-119">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="396d8-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="396d8-120">Optional query parameters</span></span>
<span data-ttu-id="396d8-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="396d8-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="396d8-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="396d8-122">Request headers</span></span>
| <span data-ttu-id="396d8-123">Nome</span><span class="sxs-lookup"><span data-stu-id="396d8-123">Name</span></span>          | <span data-ttu-id="396d8-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="396d8-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="396d8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="396d8-125">Authorization</span></span> | <span data-ttu-id="396d8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="396d8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="396d8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="396d8-128">Request body</span></span>
<span data-ttu-id="396d8-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="396d8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="396d8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="396d8-130">Response</span></span>
<span data-ttu-id="396d8-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="396d8-131">If successful, this method returns a `200 OK` response code and a collection of [audioRoutingGroup](../resources/audioroutinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="396d8-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="396d8-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="396d8-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="396d8-133">Request</span></span>
<span data-ttu-id="396d8-134">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="396d8-134">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="396d8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="396d8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups
```
# <a name="c"></a>[<span data-ttu-id="396d8-136">C#</span><span class="sxs-lookup"><span data-stu-id="396d8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-audioroutinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="396d8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="396d8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-audioroutinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="396d8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="396d8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-audioroutinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="396d8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="396d8-139">Response</span></span>

> <span data-ttu-id="396d8-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="396d8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


