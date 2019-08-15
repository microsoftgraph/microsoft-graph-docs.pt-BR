---
title: Listar acceptedSenders
description: Obtenha uma lista de usuários ou grupos que estão na lista de remetentes aceitos para este grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9573bb4eb0ba24fc9945d70d6f68a7a06b75958d
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420753"
---
# <a name="list-acceptedsenders"></a><span data-ttu-id="d767f-103">Listar acceptedSenders</span><span class="sxs-lookup"><span data-stu-id="d767f-103">List acceptedSenders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d767f-104">Obtenha uma lista de usuários ou grupos que estão na lista de remetentes aceitos para este grupo.</span><span class="sxs-lookup"><span data-stu-id="d767f-104">Get a list of users or groups that are in the accepted-senders list for this group.</span></span>

<span data-ttu-id="d767f-p101">Os usuários na lista de remetentes aceitos podem postar em conversas do grupo (identificado na URL da solicitação GET). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="d767f-p101">Users in the accepted senders list can post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="d767f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d767f-107">Permissions</span></span>
<span data-ttu-id="d767f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d767f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d767f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d767f-110">Permission type</span></span>      | <span data-ttu-id="d767f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d767f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d767f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d767f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d767f-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d767f-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d767f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d767f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d767f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d767f-115">Not supported.</span></span>    |
|<span data-ttu-id="d767f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d767f-116">Application</span></span> | <span data-ttu-id="d767f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d767f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d767f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d767f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/acceptedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d767f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d767f-119">Optional query parameters</span></span>
<span data-ttu-id="d767f-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d767f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d767f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d767f-121">Request headers</span></span>
| <span data-ttu-id="d767f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d767f-122">Header</span></span>       | <span data-ttu-id="d767f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d767f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d767f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d767f-124">Authorization</span></span>  | <span data-ttu-id="d767f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d767f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d767f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d767f-127">Request body</span></span>
<span data-ttu-id="d767f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d767f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d767f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d767f-129">Response</span></span>
<span data-ttu-id="d767f-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d767f-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d767f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d767f-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d767f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d767f-132">Request</span></span>
<span data-ttu-id="d767f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d767f-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d767f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d767f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_acceptedsenders"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/acceptedSenders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d767f-135">C#</span><span class="sxs-lookup"><span data-stu-id="d767f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-acceptedsenders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d767f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d767f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-acceptedsenders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d767f-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d767f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-acceptedsenders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d767f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d767f-138">Response</span></span>
<span data-ttu-id="d767f-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d767f-139">The following is an example of the response.</span></span>
><span data-ttu-id="d767f-140">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d767f-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d767f-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d767f-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List acceptedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
