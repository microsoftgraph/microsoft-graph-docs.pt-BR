---
title: Obter contrato
description: Recupere as propriedades e as relações de um objeto de contrato.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 39d99236ec59b38a72a98524bc3211aa616f0bce
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773995"
---
# <a name="get-agreement"></a><span data-ttu-id="19710-103">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="19710-103">Get agreement</span></span>

<span data-ttu-id="19710-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19710-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19710-105">Recupere as propriedades e as relações de um [objeto de](../resources/agreement.md) contrato.</span><span class="sxs-lookup"><span data-stu-id="19710-105">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="19710-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="19710-106">Permissions</span></span>
<span data-ttu-id="19710-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19710-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19710-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19710-109">Permission type</span></span>                        | <span data-ttu-id="19710-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19710-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="19710-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19710-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="19710-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="19710-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="19710-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19710-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19710-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19710-114">Not supported.</span></span> |
|<span data-ttu-id="19710-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19710-115">Application</span></span>                            | <span data-ttu-id="19710-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19710-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19710-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19710-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/termsOfUse/agreements/{id}
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="19710-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19710-118">Request headers</span></span>
| <span data-ttu-id="19710-119">Nome</span><span class="sxs-lookup"><span data-stu-id="19710-119">Name</span></span>         | <span data-ttu-id="19710-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="19710-120">Type</span></span>        | <span data-ttu-id="19710-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="19710-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="19710-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="19710-122">Authorization</span></span> | <span data-ttu-id="19710-123">string</span><span class="sxs-lookup"><span data-stu-id="19710-123">string</span></span> | <span data-ttu-id="19710-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19710-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19710-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19710-126">Request body</span></span>
<span data-ttu-id="19710-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="19710-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="19710-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="19710-128">Response</span></span>
<span data-ttu-id="19710-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [agreement](../resources/agreement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19710-129">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="19710-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19710-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19710-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19710-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="19710-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="19710-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/{id}?$expand=files
```
# <a name="c"></a>[<span data-ttu-id="19710-133">C#</span><span class="sxs-lookup"><span data-stu-id="19710-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19710-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19710-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19710-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19710-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="19710-136">Java</span><span class="sxs-lookup"><span data-stu-id="19710-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="19710-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="19710-137">Response</span></span>
><span data-ttu-id="19710-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19710-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
      "id": "id-value",
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
