---
title: Listar printServices
description: Recupere uma lista de objetos printService que representam os serviços disponíveis para seu locatário.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 72bc0f46df6eccd5462a776f0d38aa70175ab6f0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777212"
---
# <a name="list-printservices"></a><span data-ttu-id="0c837-103">Listar printServices</span><span class="sxs-lookup"><span data-stu-id="0c837-103">List printServices</span></span>
<span data-ttu-id="0c837-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c837-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="0c837-105">Recupere uma lista de **objetos printService** que representam os serviços disponíveis para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="0c837-105">Retrieve a list of **printService** objects that represent the services available to your tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c837-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="0c837-106">Permissions</span></span>
<span data-ttu-id="0c837-107">Uma das permissões **de** Impressão Universal delegada [é](/graph/permissions-reference#universal-print-permissions) necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="0c837-107">One of the **delegated** Universal Print [permissions](/graph/permissions-reference#universal-print-permissions) is required to call this API.</span></span>

## <a name="http-request"></a><span data-ttu-id="0c837-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c837-108">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/services
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0c837-109">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0c837-109">Optional query parameters</span></span>
<span data-ttu-id="0c837-110">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0c837-110">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0c837-111">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0c837-111">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c837-112">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c837-112">Request headers</span></span>
|<span data-ttu-id="0c837-113">Nome</span><span class="sxs-lookup"><span data-stu-id="0c837-113">Name</span></span>|<span data-ttu-id="0c837-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c837-114">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0c837-115">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c837-115">Authorization</span></span>|<span data-ttu-id="0c837-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c837-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c837-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c837-118">Request body</span></span>
<span data-ttu-id="0c837-119">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0c837-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c837-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c837-120">Response</span></span>

<span data-ttu-id="0c837-121">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos printService](../resources/printservice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c837-121">If successful, this method returns a `200 OK` response code and a collection of [printService](../resources/printservice.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0c837-122">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0c837-122">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0c837-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c837-123">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0c837-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c837-124">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printservice"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/services
```
# <a name="c"></a>[<span data-ttu-id="0c837-125">C#</span><span class="sxs-lookup"><span data-stu-id="0c837-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0c837-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c837-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0c837-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c837-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0c837-128">Java</span><span class="sxs-lookup"><span data-stu-id="0c837-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="0c837-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c837-129">Response</span></span>
<span data-ttu-id="0c837-130">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0c837-130">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printService)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/services",
  "value": [
    {
      "id": "f4cfee8b-4117-4773-a2f0-3807beb282b9",
      "endpoints": [
        {
          "id": "mpsdiscovery",
          "displayName": "Microsoft Universal Print Discovery Service",
          "uri": "https://discovery.print.microsoft.com"
        }
      ]
    }
  ]
}
```

