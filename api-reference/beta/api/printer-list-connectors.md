---
title: Listar printConnectors para impressora
description: Recupere uma lista de conectores associados à impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 97640840c7054037254073f9145e801e0faf0a24
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961458"
---
# <a name="list-printconnectors-for-printer"></a><span data-ttu-id="8d437-103">Listar printConnectors para impressora</span><span class="sxs-lookup"><span data-stu-id="8d437-103">List printConnectors for printer</span></span>

<span data-ttu-id="8d437-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d437-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d437-105">Recupere uma lista **de conectores associados** à [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="8d437-105">Retrieve a list of **connectors** associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8d437-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d437-106">Permissions</span></span>
<span data-ttu-id="8d437-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d437-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8d437-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="8d437-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="8d437-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="8d437-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="8d437-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d437-111">Permission type</span></span> | <span data-ttu-id="8d437-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d437-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8d437-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d437-113">Delegated (work or school account)</span></span>| <span data-ttu-id="8d437-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="8d437-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="8d437-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d437-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d437-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d437-116">Not Supported.</span></span>|
|<span data-ttu-id="8d437-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d437-117">Application</span></span>| <span data-ttu-id="8d437-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d437-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d437-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d437-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8d437-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8d437-120">Optional query parameters</span></span>
<span data-ttu-id="8d437-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8d437-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8d437-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8d437-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d437-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d437-123">Request headers</span></span>
| <span data-ttu-id="8d437-124">Nome</span><span class="sxs-lookup"><span data-stu-id="8d437-124">Name</span></span>      |<span data-ttu-id="8d437-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d437-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8d437-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d437-126">Authorization</span></span> | <span data-ttu-id="8d437-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d437-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d437-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d437-129">Request body</span></span>
<span data-ttu-id="8d437-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8d437-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8d437-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d437-131">Response</span></span>
<span data-ttu-id="8d437-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [printConnector](../resources/printconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d437-132">If successful, this method returns a `200 OK` response code and collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8d437-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d437-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d437-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d437-134">Request</span></span>
<span data-ttu-id="8d437-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d437-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8d437-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d437-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectors_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/connectors
```
# <a name="c"></a>[<span data-ttu-id="8d437-137">C#</span><span class="sxs-lookup"><span data-stu-id="8d437-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectors-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d437-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d437-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectors-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d437-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d437-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectors-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d437-140">Java</span><span class="sxs-lookup"><span data-stu-id="8d437-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectors-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8d437-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d437-141">Response</span></span>
<span data-ttu-id="8d437-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8d437-142">The following is an example of the response.</span></span>
><span data-ttu-id="8d437-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d437-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
