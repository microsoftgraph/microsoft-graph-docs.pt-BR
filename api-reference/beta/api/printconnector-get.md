---
title: Obter um multiconectado
description: Recupere as propriedades e os relacionamentos de um objeto Connector.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 8999a4371ea50b2d3438bcca20d2bf3c205f7bcf
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948142"
---
# <a name="get-printconnector"></a><span data-ttu-id="22e60-103">Obter um multiconectado</span><span class="sxs-lookup"><span data-stu-id="22e60-103">Get printConnector</span></span>

<span data-ttu-id="22e60-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22e60-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22e60-105">Recupere as propriedades e os relacionamentos de **um objeto** Printer.</span><span class="sxs-lookup"><span data-stu-id="22e60-105">Retrieve the properties and relationships of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="22e60-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="22e60-106">Permissions</span></span>
<span data-ttu-id="22e60-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22e60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="22e60-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="22e60-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="22e60-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22e60-110">Permission type</span></span> | <span data-ttu-id="22e60-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22e60-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="22e60-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22e60-112">Delegated (work or school account)</span></span>| <span data-ttu-id="22e60-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="22e60-113">Users.Read.All</span></span> |
|<span data-ttu-id="22e60-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22e60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22e60-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22e60-115">Not Supported.</span></span>|
|<span data-ttu-id="22e60-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22e60-116">Application</span></span>|<span data-ttu-id="22e60-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22e60-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22e60-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22e60-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22e60-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="22e60-119">Optional query parameters</span></span>
<span data-ttu-id="22e60-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="22e60-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="22e60-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="22e60-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="22e60-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22e60-122">Request headers</span></span>
| <span data-ttu-id="22e60-123">Nome</span><span class="sxs-lookup"><span data-stu-id="22e60-123">Name</span></span>      |<span data-ttu-id="22e60-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="22e60-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="22e60-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="22e60-125">Authorization</span></span> | <span data-ttu-id="22e60-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22e60-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22e60-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22e60-128">Request body</span></span>
<span data-ttu-id="22e60-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22e60-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="22e60-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="22e60-130">Response</span></span>
<span data-ttu-id="22e60-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [multiconnecter](../resources/printconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22e60-131">If successful, this method returns a `200 OK` response code and [printConnector](../resources/printconnector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="22e60-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22e60-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="22e60-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22e60-133">Request</span></span>
<span data-ttu-id="22e60-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="22e60-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="22e60-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="22e60-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connector"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="22e60-136">C#</span><span class="sxs-lookup"><span data-stu-id="22e60-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22e60-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22e60-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22e60-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22e60-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="22e60-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="22e60-139">Response</span></span>
<span data-ttu-id="22e60-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="22e60-140">The following is an example of the response.</span></span>
><span data-ttu-id="22e60-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22e60-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printConnector"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1097

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/connectors/$entity",
  "id": "9953d245-3f6e-418c-a438-67f50e69a430",
  "name": "ConnectorName",
  "fullyQualifiedDomainName": "CONNECTOR-MACHINE",
  "operatingSystem": "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
  "appVersion": "0.19.7338.23496",
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
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
  },
  "registeredBy": {}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printConnector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
