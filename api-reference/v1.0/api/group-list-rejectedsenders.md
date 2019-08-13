---
title: Listar rejectedSenders
description: 'Obtenha uma lista de usuários ou grupos que estão na lista de remetentes rejeitados para este grupo. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 408d3942d8f05dd515882181eab1bc501b79f012
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337213"
---
# <a name="list-rejectedsenders"></a><span data-ttu-id="add3d-103">Listar rejectedSenders</span><span class="sxs-lookup"><span data-stu-id="add3d-103">List rejectedSenders</span></span>
<span data-ttu-id="add3d-104">Obtenha uma lista de usuários ou grupos que estão na lista de remetentes rejeitados para este grupo.</span><span class="sxs-lookup"><span data-stu-id="add3d-104">Get a list of users or groups that are in the rejected-senders list for this group.</span></span> 

<span data-ttu-id="add3d-p101">Os usuários na lista de remetentes rejeitados não podem postar em conversas do grupo (identificado na URL da solicitação GET). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="add3d-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="add3d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="add3d-107">Permissions</span></span>
<span data-ttu-id="add3d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="add3d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="add3d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="add3d-110">Permission type</span></span>      | <span data-ttu-id="add3d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="add3d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="add3d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="add3d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="add3d-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="add3d-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="add3d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="add3d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="add3d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="add3d-115">Not supported.</span></span>    |
|<span data-ttu-id="add3d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="add3d-116">Application</span></span> | <span data-ttu-id="add3d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="add3d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="add3d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="add3d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="add3d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="add3d-119">Optional query parameters</span></span>
<span data-ttu-id="add3d-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="add3d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="add3d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="add3d-121">Request headers</span></span>
| <span data-ttu-id="add3d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="add3d-122">Header</span></span>       | <span data-ttu-id="add3d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="add3d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="add3d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="add3d-124">Authorization</span></span>  | <span data-ttu-id="add3d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="add3d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="add3d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="add3d-127">Request body</span></span>
<span data-ttu-id="add3d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="add3d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="add3d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="add3d-129">Response</span></span>
<span data-ttu-id="add3d-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="add3d-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="add3d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="add3d-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="add3d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="add3d-132">Request</span></span>
<span data-ttu-id="add3d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="add3d-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="add3d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="add3d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="add3d-135">C#</span><span class="sxs-lookup"><span data-stu-id="add3d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rejectedsenders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="add3d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="add3d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rejectedsenders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="add3d-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="add3d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rejectedsenders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="add3d-138">Java</span><span class="sxs-lookup"><span data-stu-id="add3d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rejectedsenders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="add3d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="add3d-139">Response</span></span>
<span data-ttu-id="add3d-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="add3d-140">The following is an example of the response.</span></span>
><span data-ttu-id="add3d-141">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="add3d-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="add3d-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="add3d-142">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
