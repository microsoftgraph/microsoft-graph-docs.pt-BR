---
title: Listar acceptedSenders
description: Obtenha uma lista de usuários ou grupos que estão na lista de remetentes aceitos para este grupo.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0b5271e7d559ac5326056b4a2ee63ef7cfad7de1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52041775"
---
# <a name="list-acceptedsenders"></a><span data-ttu-id="ad6ad-103">Listar acceptedSenders</span><span class="sxs-lookup"><span data-stu-id="ad6ad-103">List acceptedSenders</span></span>

<span data-ttu-id="ad6ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad6ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad6ad-105">Obtenha uma lista de usuários ou grupos que estão na lista de remetentes aceitos para este grupo.</span><span class="sxs-lookup"><span data-stu-id="ad6ad-105">Get a list of users or groups that are in the accepted-senders list for this group.</span></span>

<span data-ttu-id="ad6ad-p101">Os usuários na lista de remetentes aceitos podem postar em conversas do grupo (identificado na URL da solicitação GET). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="ad6ad-p101">Users in the accepted senders list can post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad6ad-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ad6ad-108">Permissions</span></span>
<span data-ttu-id="ad6ad-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad6ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad6ad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad6ad-111">Permission type</span></span>      | <span data-ttu-id="ad6ad-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ad6ad-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad6ad-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad6ad-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ad6ad-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad6ad-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad6ad-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad6ad-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad6ad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad6ad-116">Not supported.</span></span>    |
|<span data-ttu-id="ad6ad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad6ad-117">Application</span></span> | <span data-ttu-id="ad6ad-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad6ad-118">Not supported.</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="ad6ad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad6ad-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/acceptedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ad6ad-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ad6ad-120">Optional query parameters</span></span>
<span data-ttu-id="ad6ad-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ad6ad-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad6ad-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad6ad-122">Request headers</span></span>
| <span data-ttu-id="ad6ad-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ad6ad-123">Header</span></span>       | <span data-ttu-id="ad6ad-124">Valor</span><span class="sxs-lookup"><span data-stu-id="ad6ad-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ad6ad-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad6ad-125">Authorization</span></span>  | <span data-ttu-id="ad6ad-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad6ad-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ad6ad-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad6ad-128">Request body</span></span>
<span data-ttu-id="ad6ad-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ad6ad-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad6ad-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad6ad-130">Response</span></span>
<span data-ttu-id="ad6ad-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad6ad-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad6ad-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad6ad-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ad6ad-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad6ad-133">Request</span></span>
<span data-ttu-id="ad6ad-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad6ad-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ad6ad-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad6ad-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_acceptedsenders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/acceptedSenders
```
# <a name="c"></a>[<span data-ttu-id="ad6ad-136">C#</span><span class="sxs-lookup"><span data-stu-id="ad6ad-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-acceptedsenders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad6ad-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad6ad-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-acceptedsenders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad6ad-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad6ad-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-acceptedsenders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad6ad-139">Java</span><span class="sxs-lookup"><span data-stu-id="ad6ad-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-acceptedsenders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ad6ad-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad6ad-140">Response</span></span>
<span data-ttu-id="ad6ad-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ad6ad-141">The following is an example of the response.</span></span>
><span data-ttu-id="ad6ad-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ad6ad-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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


