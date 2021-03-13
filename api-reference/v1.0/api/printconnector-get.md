---
title: Obter printConnector
description: Recupere as propriedades e as relações de um objeto conector.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: b0c25b435ab90d1cf767c2e8928e9e3d46c087e4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772139"
---
# <a name="get-printconnector"></a><span data-ttu-id="d950e-103">Obter printConnector</span><span class="sxs-lookup"><span data-stu-id="d950e-103">Get printConnector</span></span>
<span data-ttu-id="d950e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d950e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="d950e-105">Recupere as propriedades e as relações de um **objeto printConnector.**</span><span class="sxs-lookup"><span data-stu-id="d950e-105">Retrieve the properties and relationships of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d950e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d950e-106">Permissions</span></span>
<span data-ttu-id="d950e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d950e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d950e-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="d950e-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="d950e-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="d950e-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="d950e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d950e-111">Permission type</span></span> | <span data-ttu-id="d950e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d950e-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d950e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d950e-113">Delegated (work or school account)</span></span>| <span data-ttu-id="d950e-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d950e-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="d950e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d950e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d950e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d950e-116">Not Supported.</span></span>|
|<span data-ttu-id="d950e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d950e-117">Application</span></span>|<span data-ttu-id="d950e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d950e-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d950e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d950e-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/connectors/{printConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d950e-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d950e-120">Optional query parameters</span></span>
<span data-ttu-id="d950e-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d950e-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d950e-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d950e-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d950e-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d950e-123">Request headers</span></span>
|<span data-ttu-id="d950e-124">Nome</span><span class="sxs-lookup"><span data-stu-id="d950e-124">Name</span></span>|<span data-ttu-id="d950e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d950e-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d950e-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d950e-126">Authorization</span></span>|<span data-ttu-id="d950e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d950e-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d950e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d950e-129">Request body</span></span>
<span data-ttu-id="d950e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d950e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d950e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d950e-131">Response</span></span>

<span data-ttu-id="d950e-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto printConnector](../resources/printconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d950e-132">If successful, this method returns a `200 OK` response code and a [printConnector](../resources/printconnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d950e-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d950e-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d950e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d950e-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d950e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d950e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printconnector"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/connectors/{printConnectorId}
```
# <a name="c"></a>[<span data-ttu-id="d950e-136">C#</span><span class="sxs-lookup"><span data-stu-id="d950e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d950e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d950e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d950e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d950e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d950e-139">Java</span><span class="sxs-lookup"><span data-stu-id="d950e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d950e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d950e-140">Response</span></span>
<span data-ttu-id="d950e-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d950e-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printConnector"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/connectors/$entity",
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
```

