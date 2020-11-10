---
title: Listar grupos de roteamento de áudio
description: Recupere uma lista de objetos **audioRoutingGroup** .
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 0ebdf20f757af275a0903ddfe474cf69cb6b72ba
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959694"
---
# <a name="list-audio-routing-groups"></a><span data-ttu-id="5512d-103">Listar grupos de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="5512d-103">List audio routing groups</span></span>

<span data-ttu-id="5512d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5512d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5512d-105">Recupere uma lista de objetos **audioRoutingGroup** .</span><span class="sxs-lookup"><span data-stu-id="5512d-105">Retrieve a list of **audioRoutingGroup** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="5512d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5512d-106">Permissions</span></span>
<span data-ttu-id="5512d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5512d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5512d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5512d-109">Permission type</span></span>                        | <span data-ttu-id="5512d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5512d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5512d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5512d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5512d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5512d-112">Not Supported.</span></span>                               |
| <span data-ttu-id="5512d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5512d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5512d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5512d-114">Not Supported.</span></span>                               |
| <span data-ttu-id="5512d-115">Application</span><span class="sxs-lookup"><span data-stu-id="5512d-115">Application</span></span>     | <span data-ttu-id="5512d-116">Calls. JoinGroupCalls. All, Calls.InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="5512d-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5512d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5512d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups
GET /communications/calls/{id}/audioRoutingGroups
```
> <span data-ttu-id="5512d-118">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="5512d-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="5512d-119">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="5512d-119">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="5512d-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5512d-120">Optional query parameters</span></span>
<span data-ttu-id="5512d-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5512d-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5512d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5512d-122">Request headers</span></span>
| <span data-ttu-id="5512d-123">Nome</span><span class="sxs-lookup"><span data-stu-id="5512d-123">Name</span></span>          | <span data-ttu-id="5512d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5512d-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5512d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5512d-125">Authorization</span></span> | <span data-ttu-id="5512d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5512d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5512d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5512d-128">Request body</span></span>
<span data-ttu-id="5512d-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5512d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5512d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5512d-130">Response</span></span>
<span data-ttu-id="5512d-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5512d-131">If successful, this method returns a `200 OK` response code and a collection of [audioRoutingGroup](../resources/audioroutinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5512d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5512d-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5512d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5512d-133">Request</span></span>
<span data-ttu-id="5512d-134">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="5512d-134">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5512d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5512d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups
```
# <a name="c"></a>[<span data-ttu-id="5512d-136">C#</span><span class="sxs-lookup"><span data-stu-id="5512d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-audioroutinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5512d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5512d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-audioroutinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5512d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5512d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-audioroutinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5512d-139">Java</span><span class="sxs-lookup"><span data-stu-id="5512d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-audioroutinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5512d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5512d-140">Response</span></span>

> <span data-ttu-id="5512d-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5512d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


