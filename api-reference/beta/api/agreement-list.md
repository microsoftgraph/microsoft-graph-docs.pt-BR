---
title: Listar contratos
description: Recupere uma lista de objetos de contrato.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 620ca66a2f443f1cf935cb9b5accc35c68d7eb1d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773960"
---
# <a name="list-agreements"></a><span data-ttu-id="83164-103">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="83164-103">List agreements</span></span>

<span data-ttu-id="83164-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83164-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83164-105">Recupere uma lista de objetos [de](../resources/agreement.md) contrato.</span><span class="sxs-lookup"><span data-stu-id="83164-105">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="83164-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="83164-106">Permissions</span></span>
<span data-ttu-id="83164-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83164-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83164-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83164-109">Permission type</span></span>                        | <span data-ttu-id="83164-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83164-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="83164-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83164-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="83164-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="83164-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="83164-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83164-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83164-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83164-114">Not supported.</span></span> |
|<span data-ttu-id="83164-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83164-115">Application</span></span>                            | <span data-ttu-id="83164-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83164-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="83164-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83164-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/termsOfUse/agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="83164-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83164-118">Request headers</span></span>
| <span data-ttu-id="83164-119">Nome</span><span class="sxs-lookup"><span data-stu-id="83164-119">Name</span></span>         | <span data-ttu-id="83164-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="83164-120">Type</span></span>        | <span data-ttu-id="83164-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="83164-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="83164-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="83164-122">Authorization</span></span> | <span data-ttu-id="83164-123">string</span><span class="sxs-lookup"><span data-stu-id="83164-123">string</span></span> | <span data-ttu-id="83164-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83164-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83164-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83164-126">Request body</span></span>
<span data-ttu-id="83164-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="83164-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="83164-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="83164-128">Response</span></span>
<span data-ttu-id="83164-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [de](../resources/agreement.md) contrato no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83164-129">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="83164-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83164-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83164-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83164-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="83164-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="83164-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements
```
# <a name="c"></a>[<span data-ttu-id="83164-133">C#</span><span class="sxs-lookup"><span data-stu-id="83164-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83164-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83164-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83164-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83164-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="83164-136">Java</span><span class="sxs-lookup"><span data-stu-id="83164-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="83164-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="83164-137">Response</span></span>
><span data-ttu-id="83164-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83164-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "value": [
    {
      "displayName": "displayName-value",
      "isViewingBeforeAcceptanceRequired": true,
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
  "description": "List agreements",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
