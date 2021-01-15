---
title: Listar printConnectors
description: Recupere uma lista de conectores.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 4fec305bc6239da0bc11a4ccdf61591bd32157c4
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874365"
---
# <a name="list-printconnectors"></a><span data-ttu-id="dd993-103">Listar printConnectors</span><span class="sxs-lookup"><span data-stu-id="dd993-103">List printConnectors</span></span>

<span data-ttu-id="dd993-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd993-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd993-105">Recupere uma lista de conectores de impressão.</span><span class="sxs-lookup"><span data-stu-id="dd993-105">Retrieve a list of print connectors.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd993-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd993-106">Permissions</span></span>
<span data-ttu-id="dd993-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd993-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="dd993-109">Para usar o serviço de Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="dd993-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="dd993-110">O usuário assinado deve ser um Administrador [de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="dd993-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="dd993-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd993-111">Permission type</span></span> | <span data-ttu-id="dd993-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd993-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="dd993-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd993-113">Delegated (work or school account)</span></span>| <span data-ttu-id="dd993-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd993-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="dd993-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd993-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd993-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd993-116">Not Supported.</span></span>|
|<span data-ttu-id="dd993-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd993-117">Application</span></span>| <span data-ttu-id="dd993-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd993-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd993-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd993-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dd993-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dd993-120">Optional query parameters</span></span>
<span data-ttu-id="dd993-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dd993-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="dd993-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="dd993-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="dd993-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="dd993-123">Exceptions</span></span>
<span data-ttu-id="dd993-124">Alguns operadores não são suportados: `$count` , `$search` , `$filter` .</span><span class="sxs-lookup"><span data-stu-id="dd993-124">Some operators are not supported: `$count`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd993-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd993-125">Request headers</span></span>
| <span data-ttu-id="dd993-126">Nome</span><span class="sxs-lookup"><span data-stu-id="dd993-126">Name</span></span>      |<span data-ttu-id="dd993-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd993-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dd993-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd993-128">Authorization</span></span> | <span data-ttu-id="dd993-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd993-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd993-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd993-131">Request body</span></span>
<span data-ttu-id="dd993-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dd993-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="dd993-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd993-133">Response</span></span>
<span data-ttu-id="dd993-134">Se bem-sucedido, este método retorna um código `200 OK` de resposta e uma coleção de objetos [printConnector](../resources/printconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd993-134">If successful, this method returns a `200 OK` response code and collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dd993-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd993-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd993-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd993-136">Request</span></span>
<span data-ttu-id="dd993-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd993-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd993-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd993-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/connectors
```
# <a name="c"></a>[<span data-ttu-id="dd993-139">C#</span><span class="sxs-lookup"><span data-stu-id="dd993-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd993-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd993-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd993-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd993-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd993-142">Java</span><span class="sxs-lookup"><span data-stu-id="dd993-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="dd993-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd993-143">Response</span></span>
<span data-ttu-id="dd993-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dd993-144">The following is an example of the response.</span></span>
><span data-ttu-id="dd993-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd993-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
