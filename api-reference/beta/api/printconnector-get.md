---
title: Obter um multiconectado
description: Recupere as propriedades e os relacionamentos de um objeto Connector.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: d6fef9ad3a7e5166f13fce08ac3bf77b3c8a1336
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848791"
---
# <a name="get-printconnector"></a><span data-ttu-id="f23a9-103">Obter um multiconectado</span><span class="sxs-lookup"><span data-stu-id="f23a9-103">Get printConnector</span></span>

<span data-ttu-id="f23a9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f23a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f23a9-105">Recupere as propriedades e os relacionamentos de **um objeto** Printer.</span><span class="sxs-lookup"><span data-stu-id="f23a9-105">Retrieve the properties and relationships of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f23a9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f23a9-106">Permissions</span></span>
<span data-ttu-id="f23a9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f23a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f23a9-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="f23a9-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="f23a9-110">O usuário conectado deve ser um [administrador da impressora](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="f23a9-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="f23a9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f23a9-111">Permission type</span></span> | <span data-ttu-id="f23a9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f23a9-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f23a9-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f23a9-113">Delegated (work or school account)</span></span>| <span data-ttu-id="f23a9-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="f23a9-114">User.Read</span></span> |
|<span data-ttu-id="f23a9-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f23a9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f23a9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f23a9-116">Not Supported.</span></span>|
|<span data-ttu-id="f23a9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f23a9-117">Application</span></span>|<span data-ttu-id="f23a9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f23a9-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f23a9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f23a9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f23a9-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f23a9-120">Optional query parameters</span></span>
<span data-ttu-id="f23a9-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f23a9-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f23a9-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f23a9-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f23a9-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f23a9-123">Request headers</span></span>
| <span data-ttu-id="f23a9-124">Nome</span><span class="sxs-lookup"><span data-stu-id="f23a9-124">Name</span></span>      |<span data-ttu-id="f23a9-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f23a9-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f23a9-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="f23a9-126">Authorization</span></span> | <span data-ttu-id="f23a9-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f23a9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f23a9-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f23a9-129">Request body</span></span>
<span data-ttu-id="f23a9-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f23a9-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f23a9-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f23a9-131">Response</span></span>
<span data-ttu-id="f23a9-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [multiconnecter](../resources/printconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f23a9-132">If successful, this method returns a `200 OK` response code and [printConnector](../resources/printconnector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f23a9-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f23a9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f23a9-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f23a9-134">Request</span></span>
<span data-ttu-id="f23a9-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f23a9-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f23a9-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f23a9-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connector"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="f23a9-137">C#</span><span class="sxs-lookup"><span data-stu-id="f23a9-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f23a9-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f23a9-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f23a9-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f23a9-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f23a9-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f23a9-140">Response</span></span>
<span data-ttu-id="f23a9-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f23a9-141">The following is an example of the response.</span></span>
><span data-ttu-id="f23a9-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f23a9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
