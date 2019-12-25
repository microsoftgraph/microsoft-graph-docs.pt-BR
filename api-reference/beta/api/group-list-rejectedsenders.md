---
title: Listar rejectedSenders
description: 'Obtenha uma lista de usuários ou grupos que estão na lista de remetentes rejeitados para este grupo. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5ca0286101076852e3efeecba9a3937ed4cc19ee
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869616"
---
# <a name="list-rejectedsenders"></a><span data-ttu-id="d0aba-103">Listar rejectedSenders</span><span class="sxs-lookup"><span data-stu-id="d0aba-103">List rejectedSenders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0aba-104">Obtenha uma lista de usuários ou grupos que estão na lista de remetentes rejeitados para este grupo.</span><span class="sxs-lookup"><span data-stu-id="d0aba-104">Get a list of users or groups that are in the rejected-senders list for this group.</span></span> 

<span data-ttu-id="d0aba-p101">Os usuários na lista de remetentes rejeitados não podem postar em conversas do grupo (identificado na URL da solicitação GET). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="d0aba-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0aba-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0aba-107">Permissions</span></span>
<span data-ttu-id="d0aba-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0aba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0aba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0aba-110">Permission type</span></span>      | <span data-ttu-id="d0aba-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0aba-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0aba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0aba-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d0aba-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0aba-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0aba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0aba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0aba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0aba-115">Not supported.</span></span>    |
|<span data-ttu-id="d0aba-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0aba-116">Application</span></span> | <span data-ttu-id="d0aba-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0aba-117">Not supported.</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="d0aba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0aba-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d0aba-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d0aba-119">Optional query parameters</span></span>
<span data-ttu-id="d0aba-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d0aba-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0aba-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0aba-121">Request headers</span></span>
| <span data-ttu-id="d0aba-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0aba-122">Header</span></span>       | <span data-ttu-id="d0aba-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d0aba-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d0aba-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0aba-124">Authorization</span></span>  | <span data-ttu-id="d0aba-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0aba-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d0aba-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0aba-127">Request body</span></span>
<span data-ttu-id="d0aba-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d0aba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0aba-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0aba-129">Response</span></span>
<span data-ttu-id="d0aba-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0aba-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0aba-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0aba-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d0aba-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0aba-132">Request</span></span>
<span data-ttu-id="d0aba-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0aba-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d0aba-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0aba-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/rejectedSenders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d0aba-135">C#</span><span class="sxs-lookup"><span data-stu-id="d0aba-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rejectedsenders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d0aba-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0aba-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rejectedsenders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d0aba-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0aba-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rejectedsenders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d0aba-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0aba-138">Response</span></span>
<span data-ttu-id="d0aba-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d0aba-139">The following is an example of the response.</span></span>
><span data-ttu-id="d0aba-140">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d0aba-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d0aba-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0aba-141">All the properties will be returned from an actual call.</span></span>
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
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
