---
title: Obter grupo de roteamento de áudio
description: Recupere as propriedades e as relações de um objeto audioRoutingGroup.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: cdb32816f05e9edd92850830627863fa72759229
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048012"
---
# <a name="get-audio-routing-group"></a><span data-ttu-id="e0119-103">Obter grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="e0119-103">Get audio routing group</span></span>

<span data-ttu-id="e0119-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0119-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0119-105">Recupere as propriedades e as relações de um [objeto audioRoutingGroup.](../resources/audioroutinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="e0119-105">Retrieve the properties and relationships of an [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0119-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0119-106">Permissions</span></span>
<span data-ttu-id="e0119-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0119-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e0119-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0119-109">Permission type</span></span>                        | <span data-ttu-id="e0119-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0119-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e0119-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0119-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0119-112">Não suportado</span><span class="sxs-lookup"><span data-stu-id="e0119-112">Not Supported</span></span>                               |
| <span data-ttu-id="e0119-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0119-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0119-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="e0119-114">Not Supported</span></span>                               |
| <span data-ttu-id="e0119-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0119-115">Application</span></span>                            | <span data-ttu-id="e0119-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="e0119-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0119-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0119-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups/{id}
GET /communications/calls/{id}/audioRoutingGroups/{id}
```
> <span data-ttu-id="e0119-118">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="e0119-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="e0119-119">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="e0119-119">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="e0119-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e0119-120">Optional query parameters</span></span>
<span data-ttu-id="e0119-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e0119-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0119-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0119-122">Request headers</span></span>
| <span data-ttu-id="e0119-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e0119-123">Name</span></span>          | <span data-ttu-id="e0119-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0119-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e0119-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0119-125">Authorization</span></span> | <span data-ttu-id="e0119-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0119-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0119-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0119-128">Request body</span></span>
<span data-ttu-id="e0119-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e0119-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0119-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0119-130">Response</span></span>
<span data-ttu-id="e0119-131">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0119-131">If successful, this method returns a `200 OK` response code and an [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0119-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0119-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e0119-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0119-133">Request</span></span>
<span data-ttu-id="e0119-134">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0119-134">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e0119-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0119-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="e0119-136">C#</span><span class="sxs-lookup"><span data-stu-id="e0119-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0119-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0119-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0119-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0119-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e0119-139">Java</span><span class="sxs-lookup"><span data-stu-id="e0119-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-audioroutinggroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e0119-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0119-140">Response</span></span>

> <span data-ttu-id="e0119-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e0119-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


