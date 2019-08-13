---
title: Listar acceptedSenders
description: Obtenha uma lista de usuários ou grupos que estão na lista de remetentes aceitos para este grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f39208c80967f6768f27f88d0d8436c1e35de8b4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323413"
---
# <a name="list-acceptedsenders"></a><span data-ttu-id="747c9-103">Listar acceptedSenders</span><span class="sxs-lookup"><span data-stu-id="747c9-103">List acceptedSenders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="747c9-104">Obtenha uma lista de usuários ou grupos que estão na lista de remetentes aceitos para este grupo.</span><span class="sxs-lookup"><span data-stu-id="747c9-104">Get a list of users or groups that are in the accepted-senders list for this group.</span></span>

<span data-ttu-id="747c9-p101">Os usuários na lista de remetentes aceitos podem postar em conversas do grupo (identificado na URL da solicitação GET). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="747c9-p101">Users in the accepted senders list can post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="747c9-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="747c9-107">Permissions</span></span>
<span data-ttu-id="747c9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="747c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="747c9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="747c9-110">Permission type</span></span>      | <span data-ttu-id="747c9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="747c9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="747c9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="747c9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="747c9-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="747c9-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="747c9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="747c9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="747c9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="747c9-115">Not supported.</span></span>    |
|<span data-ttu-id="747c9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="747c9-116">Application</span></span> | <span data-ttu-id="747c9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="747c9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="747c9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="747c9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/acceptedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="747c9-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="747c9-119">Optional query parameters</span></span>
<span data-ttu-id="747c9-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="747c9-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="747c9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="747c9-121">Request headers</span></span>
| <span data-ttu-id="747c9-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="747c9-122">Header</span></span>       | <span data-ttu-id="747c9-123">Valor</span><span class="sxs-lookup"><span data-stu-id="747c9-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="747c9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="747c9-124">Authorization</span></span>  | <span data-ttu-id="747c9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="747c9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="747c9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="747c9-127">Request body</span></span>
<span data-ttu-id="747c9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="747c9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="747c9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="747c9-129">Response</span></span>
<span data-ttu-id="747c9-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="747c9-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="747c9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="747c9-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="747c9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="747c9-132">Request</span></span>
<span data-ttu-id="747c9-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="747c9-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="747c9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="747c9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_acceptedsenders"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/acceptedSenders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="747c9-135">C#</span><span class="sxs-lookup"><span data-stu-id="747c9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-acceptedsenders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="747c9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="747c9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-acceptedsenders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="747c9-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="747c9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-acceptedsenders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="747c9-138">Java</span><span class="sxs-lookup"><span data-stu-id="747c9-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-acceptedsenders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="747c9-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="747c9-139">Response</span></span>
<span data-ttu-id="747c9-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="747c9-140">The following is an example of the response.</span></span>
><span data-ttu-id="747c9-141">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="747c9-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="747c9-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="747c9-142">All the properties will be returned from an actual call.</span></span>
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
