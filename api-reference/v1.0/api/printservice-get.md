---
title: Obter printService
description: Recupere as propriedades e as relações de um serviço de impressão.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 8333777d0d903501515be9ef65ec4b06bd48e226
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771348"
---
# <a name="get-printservice"></a><span data-ttu-id="0ef4d-103">Obter printService</span><span class="sxs-lookup"><span data-stu-id="0ef4d-103">Get printService</span></span>
<span data-ttu-id="0ef4d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ef4d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="0ef4d-105">Recupere as propriedades e as relações de um serviço de impressão.</span><span class="sxs-lookup"><span data-stu-id="0ef4d-105">Retrieve the properties and relationships of a print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ef4d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ef4d-106">Permissions</span></span>
<span data-ttu-id="0ef4d-107">Uma das permissões **de** Impressão Universal delegada [é](/graph/permissions-reference#universal-print-permissions) necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="0ef4d-107">One of the **delegated** Universal Print [permissions](/graph/permissions-reference#universal-print-permissions) is required to call this API.</span></span>

## <a name="http-request"></a><span data-ttu-id="0ef4d-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ef4d-108">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/services/{printServiceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0ef4d-109">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0ef4d-109">Optional query parameters</span></span>
<span data-ttu-id="0ef4d-110">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0ef4d-110">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0ef4d-111">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0ef4d-111">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ef4d-112">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ef4d-112">Request headers</span></span>
|<span data-ttu-id="0ef4d-113">Nome</span><span class="sxs-lookup"><span data-stu-id="0ef4d-113">Name</span></span>|<span data-ttu-id="0ef4d-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ef4d-114">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0ef4d-115">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ef4d-115">Authorization</span></span>|<span data-ttu-id="0ef4d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ef4d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ef4d-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ef4d-118">Request body</span></span>
<span data-ttu-id="0ef4d-119">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0ef4d-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ef4d-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ef4d-120">Response</span></span>

<span data-ttu-id="0ef4d-121">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printService](../resources/printservice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ef4d-121">If successful, this method returns a `200 OK` response code and a [printService](../resources/printservice.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0ef4d-122">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0ef4d-122">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0ef4d-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ef4d-123">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0ef4d-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ef4d-124">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printservice"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/services/{printServiceId}
```
# <a name="c"></a>[<span data-ttu-id="0ef4d-125">C#</span><span class="sxs-lookup"><span data-stu-id="0ef4d-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ef4d-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ef4d-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ef4d-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ef4d-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0ef4d-128">Java</span><span class="sxs-lookup"><span data-stu-id="0ef4d-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="0ef4d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ef4d-129">Response</span></span>
<span data-ttu-id="0ef4d-130">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0ef4d-130">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printService"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/services/$entity",
  "id": "f4cfee8b-4117-4773-a2f0-3807beb282b9",
  "endpoints": [
    {
      "id": "mpsdiscovery",
      "displayName": "Microsoft Universal Print Discovery Service",
      "uri": "https://discovery.print.microsoft.com"
    }
  ]
}
```

