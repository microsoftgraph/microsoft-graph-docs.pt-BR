---
title: Listar printConnectors
description: Recupere uma lista de conectores.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7483553e73dc078ff544cfe3ce0a192de8155cbc
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052933"
---
# <a name="list-printconnectors"></a><span data-ttu-id="44435-103">Listar printConnectors</span><span class="sxs-lookup"><span data-stu-id="44435-103">List printConnectors</span></span>

<span data-ttu-id="44435-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44435-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44435-105">Recupere uma lista de conectores de impressão.</span><span class="sxs-lookup"><span data-stu-id="44435-105">Retrieve a list of print connectors.</span></span>

## <a name="permissions"></a><span data-ttu-id="44435-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="44435-106">Permissions</span></span>
<span data-ttu-id="44435-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44435-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="44435-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="44435-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="44435-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="44435-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="44435-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44435-111">Permission type</span></span> | <span data-ttu-id="44435-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="44435-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="44435-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44435-113">Delegated (work or school account)</span></span>| <span data-ttu-id="44435-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44435-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="44435-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44435-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44435-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44435-116">Not Supported.</span></span>|
|<span data-ttu-id="44435-117">Application</span><span class="sxs-lookup"><span data-stu-id="44435-117">Application</span></span>| <span data-ttu-id="44435-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44435-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44435-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44435-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="44435-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="44435-120">Optional query parameters</span></span>
<span data-ttu-id="44435-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="44435-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="44435-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="44435-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="44435-123">Exceções</span><span class="sxs-lookup"><span data-stu-id="44435-123">Exceptions</span></span>
<span data-ttu-id="44435-124">Alguns operadores não têm suporte: `$count` , `$search` , `$filter` .</span><span class="sxs-lookup"><span data-stu-id="44435-124">Some operators are not supported: `$count`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="44435-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44435-125">Request headers</span></span>
| <span data-ttu-id="44435-126">Nome</span><span class="sxs-lookup"><span data-stu-id="44435-126">Name</span></span>      |<span data-ttu-id="44435-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="44435-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="44435-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="44435-128">Authorization</span></span> | <span data-ttu-id="44435-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44435-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44435-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44435-131">Request body</span></span>
<span data-ttu-id="44435-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="44435-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="44435-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="44435-133">Response</span></span>
<span data-ttu-id="44435-134">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [printConnector](../resources/printconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44435-134">If successful, this method returns a `200 OK` response code and collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="44435-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44435-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="44435-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44435-136">Request</span></span>
<span data-ttu-id="44435-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="44435-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="44435-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="44435-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectors_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/connectors
```
# <a name="c"></a>[<span data-ttu-id="44435-139">C#</span><span class="sxs-lookup"><span data-stu-id="44435-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectors-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44435-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44435-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectors-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44435-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44435-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectors-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44435-142">Java</span><span class="sxs-lookup"><span data-stu-id="44435-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectors-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="44435-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="44435-143">Response</span></span>
<span data-ttu-id="44435-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="44435-144">The following is an example of the response.</span></span>
><span data-ttu-id="44435-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="44435-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "displayName": "Connector1",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List connectors",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
