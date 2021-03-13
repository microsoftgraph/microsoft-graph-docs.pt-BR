---
title: Obter contrato
description: Recupere as propriedades e as relações de um objeto de contrato.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 9ef1bf8cd56cd603b685949a28a04e08d4ecb364
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775238"
---
# <a name="get-agreement"></a><span data-ttu-id="6431e-103">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="6431e-103">Get agreement</span></span>

<span data-ttu-id="6431e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6431e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6431e-105">Recupere as propriedades e as relações de um [objeto de](../resources/agreement.md) contrato.</span><span class="sxs-lookup"><span data-stu-id="6431e-105">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6431e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6431e-106">Permissions</span></span>
<span data-ttu-id="6431e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6431e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6431e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6431e-109">Permission type</span></span>                        | <span data-ttu-id="6431e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6431e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6431e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6431e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6431e-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="6431e-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="6431e-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6431e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6431e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6431e-114">Not supported.</span></span> |
|<span data-ttu-id="6431e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6431e-115">Application</span></span>                            | <span data-ttu-id="6431e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6431e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6431e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6431e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/termsOfUse/agreements/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6431e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6431e-118">Optional query parameters</span></span>
<span data-ttu-id="6431e-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6431e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6431e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6431e-120">Request headers</span></span>
| <span data-ttu-id="6431e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="6431e-121">Name</span></span>         | <span data-ttu-id="6431e-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="6431e-122">Type</span></span>        | <span data-ttu-id="6431e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6431e-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6431e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6431e-124">Authorization</span></span> | <span data-ttu-id="6431e-125">string</span><span class="sxs-lookup"><span data-stu-id="6431e-125">string</span></span> | <span data-ttu-id="6431e-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6431e-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6431e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6431e-128">Request body</span></span>
<span data-ttu-id="6431e-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6431e-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6431e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6431e-130">Response</span></span>
<span data-ttu-id="6431e-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [agreement](../resources/agreement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6431e-131">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6431e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6431e-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="6431e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6431e-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6431e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6431e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/termsOfUse/agreements/093b947f-8363-4979-a47d-4c52b33ee1be?$expand=files
```
# <a name="c"></a>[<span data-ttu-id="6431e-135">C#</span><span class="sxs-lookup"><span data-stu-id="6431e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6431e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6431e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6431e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6431e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6431e-138">Java</span><span class="sxs-lookup"><span data-stu-id="6431e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6431e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6431e-139">Response</span></span>
><span data-ttu-id="6431e-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6431e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value",
  "files": [
    {
      "id": "093b947f-8363-4979-a47d-4c52b33ee1be",
      "language": "en",
      "fileName": "TOU.pdf",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
