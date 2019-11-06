---
title: Obter grupo de roteamento de áudio
description: Recupere as propriedades e os relacionamentos de um objeto audioRoutingGroup.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 316447ce183e47d187af5948af300ead83377e64
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006379"
---
# <a name="get-audio-routing-group"></a><span data-ttu-id="51130-103">Obter grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="51130-103">Get audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51130-104">Recupere as propriedades e os relacionamentos de um objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="51130-104">Retrieve the properties and relationships of an [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="51130-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="51130-105">Permissions</span></span>
<span data-ttu-id="51130-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51130-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="51130-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51130-108">Permission type</span></span>                        | <span data-ttu-id="51130-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="51130-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="51130-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51130-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="51130-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="51130-111">Not Supported</span></span>                               |
| <span data-ttu-id="51130-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51130-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51130-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="51130-113">Not Supported</span></span>                               |
| <span data-ttu-id="51130-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51130-114">Application</span></span>                            | <span data-ttu-id="51130-115">Calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="51130-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="51130-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51130-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups/{id}
GET /communications/calls/{id}/audioRoutingGroups/{id}
```
> <span data-ttu-id="51130-117">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="51130-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="51130-118">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="51130-118">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="51130-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="51130-119">Optional query parameters</span></span>
<span data-ttu-id="51130-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="51130-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51130-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51130-121">Request headers</span></span>
| <span data-ttu-id="51130-122">Nome</span><span class="sxs-lookup"><span data-stu-id="51130-122">Name</span></span>          | <span data-ttu-id="51130-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="51130-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="51130-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="51130-124">Authorization</span></span> | <span data-ttu-id="51130-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51130-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51130-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51130-127">Request body</span></span>
<span data-ttu-id="51130-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="51130-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51130-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="51130-129">Response</span></span>
<span data-ttu-id="51130-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51130-130">If successful, this method returns a `200 OK` response code and an [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51130-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51130-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="51130-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51130-132">Request</span></span>
<span data-ttu-id="51130-133">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="51130-133">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="51130-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="51130-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="51130-135">C#</span><span class="sxs-lookup"><span data-stu-id="51130-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="51130-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51130-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="51130-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51130-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="51130-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="51130-138">Response</span></span>

> <span data-ttu-id="51130-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51130-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
