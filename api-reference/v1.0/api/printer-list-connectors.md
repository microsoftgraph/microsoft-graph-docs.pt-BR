---
title: Listar printConnectors para impressora
description: Recupere uma lista de conectores associados à impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 5176819d4d91e696a08c288e086fb237622c777b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771985"
---
# <a name="list-printconnectors-for-a-printer"></a><span data-ttu-id="1b89c-103">Listar printConnectors para uma impressora</span><span class="sxs-lookup"><span data-stu-id="1b89c-103">List printConnectors for a printer</span></span>
<span data-ttu-id="1b89c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b89c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="1b89c-105">Recupere uma lista de [printConnectors associados](../resources/printconnector.md) à [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="1b89c-105">Retrieve a list of [printConnectors](../resources/printconnector.md) associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1b89c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="1b89c-106">Permissions</span></span>
<span data-ttu-id="1b89c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b89c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1b89c-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve [](printer-get.md) ter uma assinatura de Impressão Universal ativa, uma permissão que concede acesso a Obter impressora e uma das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="1b89c-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="1b89c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b89c-110">Permission type</span></span> | <span data-ttu-id="1b89c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b89c-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="1b89c-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b89c-112">Delegated (work or school account)</span></span>| <span data-ttu-id="1b89c-113">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b89c-113">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="1b89c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b89c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b89c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b89c-115">Not Supported.</span></span>|
|<span data-ttu-id="1b89c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b89c-116">Application</span></span>| <span data-ttu-id="1b89c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b89c-117">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b89c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b89c-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers/{printerId}/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1b89c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1b89c-119">Optional query parameters</span></span>
<span data-ttu-id="1b89c-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1b89c-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1b89c-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1b89c-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b89c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b89c-122">Request headers</span></span>
|<span data-ttu-id="1b89c-123">Nome</span><span class="sxs-lookup"><span data-stu-id="1b89c-123">Name</span></span>|<span data-ttu-id="1b89c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b89c-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1b89c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b89c-125">Authorization</span></span>|<span data-ttu-id="1b89c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b89c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b89c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b89c-128">Request body</span></span>
<span data-ttu-id="1b89c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1b89c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b89c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b89c-130">Response</span></span>

<span data-ttu-id="1b89c-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos printConnector](../resources/printconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b89c-131">If successful, this method returns a `200 OK` response code and a collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b89c-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1b89c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1b89c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b89c-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1b89c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b89c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printconnector"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/connectors
```
# <a name="c"></a>[<span data-ttu-id="1b89c-135">C#</span><span class="sxs-lookup"><span data-stu-id="1b89c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b89c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b89c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b89c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b89c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b89c-138">Java</span><span class="sxs-lookup"><span data-stu-id="1b89c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="1b89c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b89c-139">Response</span></span>
<span data-ttu-id="1b89c-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1b89c-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printConnector)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('2f3453b7-4686-4b5b-9575-4f1e5b909ba7')/connectors",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "name": "Connector1",
      "fullyQualifiedDomainName": "connector1@redmond.corp.microsoft.com",
      "operatingSystem": "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
      "appVersion": "0.19.7338.23496",
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
        "floor": "1",
        "floorDescription": "First Floor",
        "roomName": "1234",
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

