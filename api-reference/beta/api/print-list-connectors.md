---
title: Obter conectores
description: Recupere uma lista de conectores.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: b71230de9c0b4c64eff35bf699a0168d355594ac
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895595"
---
# <a name="list-connectors"></a><span data-ttu-id="21f0f-103">Conectores de lista</span><span class="sxs-lookup"><span data-stu-id="21f0f-103">List connectors</span></span>

<span data-ttu-id="21f0f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21f0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21f0f-105">Recupere uma lista de conectores.</span><span class="sxs-lookup"><span data-stu-id="21f0f-105">Retrieve a list of connectors.</span></span>

## <a name="permissions"></a><span data-ttu-id="21f0f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="21f0f-106">Permissions</span></span>
<span data-ttu-id="21f0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21f0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21f0f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21f0f-109">Permission type</span></span> | <span data-ttu-id="21f0f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21f0f-110">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="21f0f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21f0f-111">Delegated (work or school account)</span></span>| <span data-ttu-id="21f0f-112">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="21f0f-112">Users.Read.All</span></span> |
|<span data-ttu-id="21f0f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21f0f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21f0f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21f0f-114">Not Supported.</span></span>|
|<span data-ttu-id="21f0f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21f0f-115">Application</span></span>|<span data-ttu-id="21f0f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21f0f-116">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21f0f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21f0f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="21f0f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="21f0f-118">Optional query parameters</span></span>
<span data-ttu-id="21f0f-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="21f0f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="21f0f-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="21f0f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="21f0f-121">Exceções</span><span class="sxs-lookup"><span data-stu-id="21f0f-121">Exceptions</span></span>
* <span data-ttu-id="21f0f-122">Não `$count` há `$filter` suporte para os operadores e.</span><span class="sxs-lookup"><span data-stu-id="21f0f-122">The `$count` and `$filter` operators are not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="21f0f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21f0f-123">Request headers</span></span>
| <span data-ttu-id="21f0f-124">Nome</span><span class="sxs-lookup"><span data-stu-id="21f0f-124">Name</span></span>      |<span data-ttu-id="21f0f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="21f0f-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="21f0f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="21f0f-126">Authorization</span></span> | <span data-ttu-id="21f0f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21f0f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21f0f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21f0f-129">Request body</span></span>
<span data-ttu-id="21f0f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="21f0f-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="21f0f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="21f0f-131">Response</span></span>
<span data-ttu-id="21f0f-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [Connector](../resources/printconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21f0f-132">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/printconnector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="21f0f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21f0f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21f0f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21f0f-134">Request</span></span>
<span data-ttu-id="21f0f-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="21f0f-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```http
GET https://graph.microsoft.com/beta/print/connectors
```
##### <a name="response"></a><span data-ttu-id="21f0f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="21f0f-136">Response</span></span>
<span data-ttu-id="21f0f-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="21f0f-137">The following is an example of the response.</span></span>
><span data-ttu-id="21f0f-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21f0f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
      "registeredBy": {},
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