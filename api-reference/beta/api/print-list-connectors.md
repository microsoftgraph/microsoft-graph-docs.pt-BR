---
title: Obter conectores
description: Recupere uma lista de conectores.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 0b6e9474def623d6b5492464ad5190828a8135cd
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062165"
---
# <a name="list-connectors"></a><span data-ttu-id="3e97a-103">Conectores de lista</span><span class="sxs-lookup"><span data-stu-id="3e97a-103">List connectors</span></span>

<span data-ttu-id="3e97a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e97a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e97a-105">Recupere uma lista de conectores.</span><span class="sxs-lookup"><span data-stu-id="3e97a-105">Retrieve a list of connectors.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e97a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e97a-106">Permissions</span></span>
<span data-ttu-id="3e97a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e97a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e97a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e97a-109">Permission type</span></span> | <span data-ttu-id="3e97a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e97a-110">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="3e97a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e97a-111">Delegated (work or school account)</span></span>| <span data-ttu-id="3e97a-112">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="3e97a-112">Users.Read.All</span></span> |
|<span data-ttu-id="3e97a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e97a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e97a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e97a-114">Not Supported.</span></span>|
|<span data-ttu-id="3e97a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e97a-115">Application</span></span>|<span data-ttu-id="3e97a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e97a-116">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e97a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e97a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3e97a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3e97a-118">Optional query parameters</span></span>
<span data-ttu-id="3e97a-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3e97a-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3e97a-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3e97a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="3e97a-121">Exceções</span><span class="sxs-lookup"><span data-stu-id="3e97a-121">Exceptions</span></span>
* <span data-ttu-id="3e97a-122">Não `$count` há `$filter` suporte para os operadores e.</span><span class="sxs-lookup"><span data-stu-id="3e97a-122">The `$count` and `$filter` operators are not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e97a-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e97a-123">Request headers</span></span>
| <span data-ttu-id="3e97a-124">Nome</span><span class="sxs-lookup"><span data-stu-id="3e97a-124">Name</span></span>      |<span data-ttu-id="3e97a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e97a-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3e97a-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e97a-126">Authorization</span></span> | <span data-ttu-id="3e97a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e97a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e97a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e97a-129">Request body</span></span>
<span data-ttu-id="3e97a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3e97a-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3e97a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e97a-131">Response</span></span>
<span data-ttu-id="3e97a-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [Connector](../resources/printconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e97a-132">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/printconnector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e97a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e97a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e97a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e97a-134">Request</span></span>
<span data-ttu-id="3e97a-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e97a-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3e97a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e97a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/connectors
```
# <a name="c"></a>[<span data-ttu-id="3e97a-137">C#</span><span class="sxs-lookup"><span data-stu-id="3e97a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e97a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e97a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e97a-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e97a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3e97a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e97a-140">Response</span></span>
<span data-ttu-id="3e97a-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3e97a-141">The following is an example of the response.</span></span>
><span data-ttu-id="3e97a-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e97a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printConnector",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1289

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/connectors",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "name": "Connector1",
      "fullyQualifiedDomainName": "connector1@redmond.corp.microsoft.com",
      "operatingSystem": "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
      "appVersion": "0.19.7338.23496",
      "deviceHealth": {
        "lastConnectionTime": "2020-02-04T07:00:00.0000000"
      },
      "registeredDateTime": "2020-02-04T07:00:00.0000000",
      "location": {
        "latitude": 1.1,
        "longitude": 2.2,
        "altitudeInMeters": 3,
        "streetAddress": "One Microsoft Way",
        "subUnit": [
            "Main Plaza",
            "Unit 400"
        ],
        "city": "Redmond",
        "postalCode": "98052",
        "countryOrRegion": "USA",
        "site": "Puget Sound",
        "building": "Studio E",
        "floorNumber": 1,
        "floorDescription": "First Floor",
        "roomNumber": 1234,
        "roomDescription": "First floor copy room",
        "organization": [
            "C+AI",
            "Microsoft Graph"
        ],
        "subdivision": [
            "King County",
            "Red West"
        ],
        "stateOrProvince": "Washington"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List connectors",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
