---
title: Listar acceptedSenders
description: Obtenha uma lista de usuários ou grupos que estão na lista de remetentes aceitos para este grupo.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: de7c7216af4e79547db7963e63d9cd60565740c5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43397187"
---
# <a name="list-acceptedsenders"></a><span data-ttu-id="74ca0-103">Listar acceptedSenders</span><span class="sxs-lookup"><span data-stu-id="74ca0-103">List acceptedSenders</span></span>

<span data-ttu-id="74ca0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74ca0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74ca0-105">Obtenha uma lista de usuários ou grupos que estão na lista de remetentes aceitos para este grupo.</span><span class="sxs-lookup"><span data-stu-id="74ca0-105">Get a list of users or groups that are in the accepted-senders list for this group.</span></span>

<span data-ttu-id="74ca0-p101">Os usuários na lista de remetentes aceitos podem postar em conversas do grupo (identificado na URL da solicitação GET). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="74ca0-p101">Users in the accepted senders list can post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="74ca0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="74ca0-108">Permissions</span></span>
<span data-ttu-id="74ca0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74ca0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74ca0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74ca0-111">Permission type</span></span>      | <span data-ttu-id="74ca0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74ca0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74ca0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74ca0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="74ca0-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74ca0-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="74ca0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74ca0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74ca0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74ca0-116">Not supported.</span></span>    |
|<span data-ttu-id="74ca0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74ca0-117">Application</span></span> | <span data-ttu-id="74ca0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74ca0-118">Not supported.</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="74ca0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74ca0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/acceptedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="74ca0-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="74ca0-120">Optional query parameters</span></span>
<span data-ttu-id="74ca0-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="74ca0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74ca0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74ca0-122">Request headers</span></span>
| <span data-ttu-id="74ca0-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="74ca0-123">Header</span></span>       | <span data-ttu-id="74ca0-124">Valor</span><span class="sxs-lookup"><span data-stu-id="74ca0-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="74ca0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="74ca0-125">Authorization</span></span>  | <span data-ttu-id="74ca0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74ca0-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="74ca0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74ca0-128">Request body</span></span>
<span data-ttu-id="74ca0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="74ca0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74ca0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="74ca0-130">Response</span></span>
<span data-ttu-id="74ca0-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74ca0-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74ca0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74ca0-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="74ca0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74ca0-133">Request</span></span>
<span data-ttu-id="74ca0-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="74ca0-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="74ca0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="74ca0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_acceptedsenders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/acceptedSenders
```
# <a name="c"></a>[<span data-ttu-id="74ca0-136">C#</span><span class="sxs-lookup"><span data-stu-id="74ca0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-acceptedsenders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74ca0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74ca0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-acceptedsenders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74ca0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74ca0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-acceptedsenders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="74ca0-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="74ca0-139">Response</span></span>
<span data-ttu-id="74ca0-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="74ca0-140">The following is an example of the response.</span></span>
><span data-ttu-id="74ca0-141">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="74ca0-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="74ca0-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74ca0-142">All the properties will be returned from an actual call.</span></span>
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
