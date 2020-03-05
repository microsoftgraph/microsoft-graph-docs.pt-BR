---
title: Listar acceptedSenders
description: Obtenha uma lista de usuários ou grupos que estão na lista de remetentes aceitos para este grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3f3c367335a941d6275b9c2d1178387a5efbc357
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419846"
---
# <a name="list-acceptedsenders"></a><span data-ttu-id="e91c6-103">Listar acceptedSenders</span><span class="sxs-lookup"><span data-stu-id="e91c6-103">List acceptedSenders</span></span>

<span data-ttu-id="e91c6-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e91c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e91c6-105">Obtenha uma lista de usuários ou grupos que estão na lista de remetentes aceitos para este grupo.</span><span class="sxs-lookup"><span data-stu-id="e91c6-105">Get a list of users or groups that are in the accepted-senders list for this group.</span></span>

<span data-ttu-id="e91c6-p101">Os usuários na lista de remetentes aceitos podem postar em conversas do grupo (identificado na URL da solicitação GET). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="e91c6-p101">Users in the accepted senders list can post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="e91c6-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e91c6-108">Permissions</span></span>
<span data-ttu-id="e91c6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e91c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e91c6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e91c6-111">Permission type</span></span>      | <span data-ttu-id="e91c6-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e91c6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e91c6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e91c6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e91c6-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e91c6-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e91c6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e91c6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e91c6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e91c6-116">Not supported.</span></span>    |
|<span data-ttu-id="e91c6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e91c6-117">Application</span></span> | <span data-ttu-id="e91c6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e91c6-118">Not supported.</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="e91c6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e91c6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/acceptedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e91c6-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e91c6-120">Optional query parameters</span></span>
<span data-ttu-id="e91c6-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e91c6-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e91c6-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e91c6-122">Request headers</span></span>
| <span data-ttu-id="e91c6-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e91c6-123">Header</span></span>       | <span data-ttu-id="e91c6-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e91c6-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e91c6-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e91c6-125">Authorization</span></span>  | <span data-ttu-id="e91c6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e91c6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e91c6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e91c6-128">Request body</span></span>
<span data-ttu-id="e91c6-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e91c6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e91c6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e91c6-130">Response</span></span>
<span data-ttu-id="e91c6-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e91c6-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e91c6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e91c6-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e91c6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e91c6-133">Request</span></span>
<span data-ttu-id="e91c6-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e91c6-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e91c6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e91c6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_acceptedsenders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/acceptedSenders
```
# <a name="c"></a>[<span data-ttu-id="e91c6-136">C#</span><span class="sxs-lookup"><span data-stu-id="e91c6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-acceptedsenders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e91c6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e91c6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-acceptedsenders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e91c6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e91c6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-acceptedsenders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e91c6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e91c6-139">Response</span></span>
<span data-ttu-id="e91c6-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e91c6-140">The following is an example of the response.</span></span>
><span data-ttu-id="e91c6-141">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e91c6-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e91c6-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e91c6-142">All the properties will be returned from an actual call.</span></span>
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
