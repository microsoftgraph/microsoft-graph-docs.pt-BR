---
title: Obter o AddServiceEndpoint
description: Recupere as propriedades e os relacionamentos de um ponto de extremidade de serviço de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: fd03c0601d98080af4942df574a1aee2740640a0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968188"
---
# <a name="get-printserviceendpoint"></a><span data-ttu-id="f35c0-103">Obter o AddServiceEndpoint</span><span class="sxs-lookup"><span data-stu-id="f35c0-103">Get printServiceEndpoint</span></span>

<span data-ttu-id="f35c0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f35c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f35c0-105">Recupere as propriedades e os relacionamentos de um ponto de extremidade de serviço de impressão.</span><span class="sxs-lookup"><span data-stu-id="f35c0-105">Retrieve the properties and relationships of a print service endpoint.</span></span>

## <a name="permissions"></a><span data-ttu-id="f35c0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f35c0-106">Permissions</span></span>
<span data-ttu-id="f35c0-107">Nenhuma permissão é necessária para chamar essa API, mas para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa.</span><span class="sxs-lookup"><span data-stu-id="f35c0-107">No permissions are needed to call this API, but to use the Universal Print service, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="f35c0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f35c0-108">Permission type</span></span> | <span data-ttu-id="f35c0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f35c0-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f35c0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f35c0-110">Delegated (work or school account)</span></span>|<span data-ttu-id="f35c0-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f35c0-111">None.</span></span>|
|<span data-ttu-id="f35c0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f35c0-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f35c0-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f35c0-113">None.</span></span>|
|<span data-ttu-id="f35c0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f35c0-114">Application</span></span>|<span data-ttu-id="f35c0-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f35c0-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f35c0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f35c0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services/{id}/endpoints/{name}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f35c0-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f35c0-117">Optional query parameters</span></span>
<span data-ttu-id="f35c0-118">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f35c0-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f35c0-119">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f35c0-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f35c0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f35c0-120">Request headers</span></span>
| <span data-ttu-id="f35c0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f35c0-121">Name</span></span>      |<span data-ttu-id="f35c0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f35c0-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f35c0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f35c0-123">Authorization</span></span> | <span data-ttu-id="f35c0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f35c0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f35c0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f35c0-126">Request body</span></span>
<span data-ttu-id="f35c0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f35c0-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f35c0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f35c0-128">Response</span></span>
<span data-ttu-id="f35c0-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [myserviceendpoint](../resources/printserviceendpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f35c0-129">If successful, this method returns a `200 OK` response code and a [printServiceEndpoint](../resources/printserviceendpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f35c0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f35c0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f35c0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f35c0-131">Request</span></span>
<span data-ttu-id="f35c0-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f35c0-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f35c0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f35c0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printserviceendpoint"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services/{id}/endpoints/{name}
```
# <a name="c"></a>[<span data-ttu-id="f35c0-134">C#</span><span class="sxs-lookup"><span data-stu-id="f35c0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printserviceendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f35c0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f35c0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printserviceendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f35c0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f35c0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printserviceendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f35c0-137">Java</span><span class="sxs-lookup"><span data-stu-id="f35c0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printserviceendpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f35c0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f35c0-138">Response</span></span>
<span data-ttu-id="f35c0-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f35c0-139">The following is an example of the response.</span></span>
><span data-ttu-id="f35c0-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f35c0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printServiceEndpoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 260

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printServiceEndpoint)",
  "id": "mpsdiscovery",
  "displayName": "Microsoft Universal Print Discovery Service",
  "uri": "https://discovery.print.microsoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printServiceEndpoint",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


