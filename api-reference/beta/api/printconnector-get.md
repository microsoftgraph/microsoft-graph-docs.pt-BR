---
title: Obter printConnector
description: Recupere as propriedades e os relacionamentos de um objeto connector.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: cfe27f18f9e1229babdce07c8cf64c0ed6146fe2
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873553"
---
# <a name="get-printconnector"></a><span data-ttu-id="13410-103">Obter printConnector</span><span class="sxs-lookup"><span data-stu-id="13410-103">Get printConnector</span></span>

<span data-ttu-id="13410-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13410-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13410-105">Recupere as propriedades e os relacionamentos de um **objeto printConnector.**</span><span class="sxs-lookup"><span data-stu-id="13410-105">Retrieve the properties and relationships of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="13410-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="13410-106">Permissions</span></span>
<span data-ttu-id="13410-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13410-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="13410-109">Para usar o serviço de Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="13410-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="13410-110">O usuário assinado deve ser um Administrador [de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="13410-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="13410-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13410-111">Permission type</span></span> | <span data-ttu-id="13410-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13410-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="13410-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13410-113">Delegated (work or school account)</span></span>| <span data-ttu-id="13410-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13410-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="13410-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13410-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13410-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13410-116">Not Supported.</span></span>|
|<span data-ttu-id="13410-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13410-117">Application</span></span>|<span data-ttu-id="13410-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13410-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13410-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13410-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13410-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="13410-120">Optional query parameters</span></span>
<span data-ttu-id="13410-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="13410-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="13410-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="13410-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="13410-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13410-123">Request headers</span></span>
| <span data-ttu-id="13410-124">Nome</span><span class="sxs-lookup"><span data-stu-id="13410-124">Name</span></span>      |<span data-ttu-id="13410-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="13410-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="13410-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="13410-126">Authorization</span></span> | <span data-ttu-id="13410-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13410-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13410-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13410-129">Request body</span></span>
<span data-ttu-id="13410-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13410-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="13410-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="13410-131">Response</span></span>
<span data-ttu-id="13410-132">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [printConnector](../resources/printconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13410-132">If successful, this method returns a `200 OK` response code and [printConnector](../resources/printconnector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="13410-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13410-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13410-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13410-134">Request</span></span>
<span data-ttu-id="13410-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="13410-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="13410-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="13410-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connector"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="13410-137">C#</span><span class="sxs-lookup"><span data-stu-id="13410-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13410-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13410-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13410-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13410-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="13410-140">Java</span><span class="sxs-lookup"><span data-stu-id="13410-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="13410-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="13410-141">Response</span></span>
<span data-ttu-id="13410-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="13410-142">The following is an example of the response.</span></span>
><span data-ttu-id="13410-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13410-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "displayName": "ConnectorName",
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
  }
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
