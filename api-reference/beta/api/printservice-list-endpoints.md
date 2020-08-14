---
title: Lista de ServiceEndpoints
description: Recupere uma lista de pontos de extremidade expostos por um serviço de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c5e7f9ccc5348018269db227ccf620406807462f
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674138"
---
# <a name="list-printserviceendpoints"></a><span data-ttu-id="b0eec-103">Lista de ServiceEndpoints</span><span class="sxs-lookup"><span data-stu-id="b0eec-103">List printServiceEndpoints</span></span>

<span data-ttu-id="b0eec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0eec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0eec-105">Recupere uma lista de pontos de extremidade expostos por um serviço de impressão.</span><span class="sxs-lookup"><span data-stu-id="b0eec-105">Retrieve a list of endpoints exposed by a print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0eec-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b0eec-106">Permissions</span></span>
<span data-ttu-id="b0eec-107">Nenhuma permissão é necessária para chamar essa API, mas para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa.</span><span class="sxs-lookup"><span data-stu-id="b0eec-107">No permissions are needed to call this API, but to use the Universal Print service, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="b0eec-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0eec-108">Permission type</span></span> | <span data-ttu-id="b0eec-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0eec-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b0eec-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0eec-110">Delegated (work or school account)</span></span>|<span data-ttu-id="b0eec-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b0eec-111">None.</span></span>|
|<span data-ttu-id="b0eec-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0eec-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0eec-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b0eec-113">None.</span></span>|
|<span data-ttu-id="b0eec-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0eec-114">Application</span></span>|<span data-ttu-id="b0eec-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b0eec-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0eec-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0eec-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services/{id}/endpoints
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0eec-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b0eec-117">Optional query parameters</span></span>
<span data-ttu-id="b0eec-118">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b0eec-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b0eec-119">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b0eec-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0eec-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0eec-120">Request headers</span></span>
| <span data-ttu-id="b0eec-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b0eec-121">Name</span></span>      |<span data-ttu-id="b0eec-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0eec-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b0eec-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0eec-123">Authorization</span></span> | <span data-ttu-id="b0eec-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0eec-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0eec-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0eec-126">Request body</span></span>
<span data-ttu-id="b0eec-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b0eec-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b0eec-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0eec-128">Response</span></span>
<span data-ttu-id="b0eec-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos de [AddServiceEndpoint](../resources/printserviceendpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0eec-129">If successful, this method returns a `200 OK` response code and a collection of [printServiceEndpoint](../resources/printserviceendpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b0eec-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0eec-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0eec-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0eec-131">Request</span></span>
<span data-ttu-id="b0eec-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0eec-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b0eec-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0eec-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services/{id}/endpoints
```
# <a name="c"></a>[<span data-ttu-id="b0eec-134">C#</span><span class="sxs-lookup"><span data-stu-id="b0eec-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0eec-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0eec-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0eec-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0eec-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b0eec-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0eec-137">Response</span></span>
<span data-ttu-id="b0eec-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b0eec-138">The following is an example of the response.</span></span>
><span data-ttu-id="b0eec-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0eec-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printServiceEndpoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printServiceEndpoint)",
  "value": [
    {
      "id": "mpsdiscovery",
      "displayName": "Microsoft Universal Print Discovery Service",
      "uri": "https://discovery.print.microsoft.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List endpoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
