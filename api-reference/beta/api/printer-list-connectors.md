---
title: Conectores de lista
description: Recupere uma lista de conectores associados à impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: eaf7b1a13b48a145a770cc94214846f69119b083
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062089"
---
# <a name="list-connectors"></a><span data-ttu-id="707f4-103">Conectores de lista</span><span class="sxs-lookup"><span data-stu-id="707f4-103">List connectors</span></span>

<span data-ttu-id="707f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="707f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="707f4-105">Recupere uma lista de **conectores** associados à [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="707f4-105">Retrieve a list of **connectors** associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="707f4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="707f4-106">Permissions</span></span>
<span data-ttu-id="707f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="707f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="707f4-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="707f4-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="707f4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="707f4-110">Permission type</span></span> | <span data-ttu-id="707f4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="707f4-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="707f4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="707f4-112">Delegated (work or school account)</span></span>| <span data-ttu-id="707f4-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="707f4-113">Users.Read.All</span></span> |
|<span data-ttu-id="707f4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="707f4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="707f4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="707f4-115">Not Supported.</span></span>|
|<span data-ttu-id="707f4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="707f4-116">Application</span></span>|<span data-ttu-id="707f4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="707f4-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="707f4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="707f4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/connectors
```

## <a name="request-headers"></a><span data-ttu-id="707f4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="707f4-119">Request headers</span></span>
| <span data-ttu-id="707f4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="707f4-120">Name</span></span>      |<span data-ttu-id="707f4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="707f4-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="707f4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="707f4-122">Authorization</span></span> | <span data-ttu-id="707f4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="707f4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="707f4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="707f4-125">Request body</span></span>
<span data-ttu-id="707f4-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="707f4-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="707f4-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="707f4-127">Response</span></span>
<span data-ttu-id="707f4-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de objetos de [multiconnector](../resources/printconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="707f4-128">If successful, this method returns a `200 OK` response code and collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="707f4-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="707f4-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="707f4-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="707f4-130">Request</span></span>
<span data-ttu-id="707f4-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="707f4-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="707f4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="707f4-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/connectors
```
# <a name="c"></a>[<span data-ttu-id="707f4-133">C#</span><span class="sxs-lookup"><span data-stu-id="707f4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="707f4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="707f4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="707f4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="707f4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="707f4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="707f4-136">Response</span></span>
<span data-ttu-id="707f4-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="707f4-137">The following is an example of the response.</span></span>
><span data-ttu-id="707f4-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="707f4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1373

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printConnector)",
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
