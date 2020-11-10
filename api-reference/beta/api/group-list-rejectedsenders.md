---
title: Listar rejectedSenders
description: 'Obtenha uma lista de usuários ou grupos que estão na lista de remetentes rejeitados para este grupo. '
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: adacc97fa00880b9be16667b5d04823864b78d15
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953855"
---
# <a name="list-rejectedsenders"></a><span data-ttu-id="3a909-103">Listar rejectedSenders</span><span class="sxs-lookup"><span data-stu-id="3a909-103">List rejectedSenders</span></span>

<span data-ttu-id="3a909-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a909-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a909-105">Obtenha uma lista de usuários ou grupos que estão na lista de remetentes rejeitados para este grupo.</span><span class="sxs-lookup"><span data-stu-id="3a909-105">Get a list of users or groups that are in the rejected-senders list for this group.</span></span> 

<span data-ttu-id="3a909-p101">Os usuários na lista de remetentes rejeitados não podem postar em conversas do grupo (identificado na URL da solicitação GET). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="3a909-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a909-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a909-108">Permissions</span></span>
<span data-ttu-id="3a909-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a909-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a909-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a909-111">Permission type</span></span>      | <span data-ttu-id="3a909-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a909-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a909-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a909-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3a909-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a909-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3a909-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a909-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a909-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a909-116">Not supported.</span></span>    |
|<span data-ttu-id="3a909-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a909-117">Application</span></span> | <span data-ttu-id="3a909-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a909-118">Not supported.</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="3a909-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a909-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3a909-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3a909-120">Optional query parameters</span></span>
<span data-ttu-id="3a909-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3a909-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a909-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a909-122">Request headers</span></span>
| <span data-ttu-id="3a909-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a909-123">Header</span></span>       | <span data-ttu-id="3a909-124">Valor</span><span class="sxs-lookup"><span data-stu-id="3a909-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3a909-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a909-125">Authorization</span></span>  | <span data-ttu-id="3a909-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a909-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3a909-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a909-128">Request body</span></span>
<span data-ttu-id="3a909-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a909-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a909-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a909-130">Response</span></span>
<span data-ttu-id="3a909-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a909-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a909-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a909-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3a909-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a909-133">Request</span></span>
<span data-ttu-id="3a909-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a909-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3a909-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a909-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/rejectedSenders
```
# <a name="c"></a>[<span data-ttu-id="3a909-136">C#</span><span class="sxs-lookup"><span data-stu-id="3a909-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rejectedsenders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a909-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a909-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rejectedsenders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a909-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a909-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rejectedsenders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a909-139">Java</span><span class="sxs-lookup"><span data-stu-id="3a909-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rejectedsenders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3a909-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a909-140">Response</span></span>
<span data-ttu-id="3a909-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3a909-141">The following is an example of the response.</span></span>
><span data-ttu-id="3a909-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a909-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


