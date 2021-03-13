---
title: Listar printConnectors
description: Recupere uma lista de conectores.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 688ef963a4680351a5ba38f369eef4c88cd45792
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776995"
---
# <a name="list-printconnectors"></a><span data-ttu-id="a607c-103">Listar printConnectors</span><span class="sxs-lookup"><span data-stu-id="a607c-103">List printConnectors</span></span>
<span data-ttu-id="a607c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a607c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="a607c-105">Recupere uma lista de conectores de impressão.</span><span class="sxs-lookup"><span data-stu-id="a607c-105">Retrieve a list of print connectors.</span></span>

## <a name="permissions"></a><span data-ttu-id="a607c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a607c-106">Permissions</span></span>
<span data-ttu-id="a607c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a607c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a607c-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="a607c-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="a607c-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="a607c-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="a607c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a607c-111">Permission type</span></span> | <span data-ttu-id="a607c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a607c-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a607c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a607c-113">Delegated (work or school account)</span></span>| <span data-ttu-id="a607c-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a607c-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="a607c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a607c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a607c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a607c-116">Not Supported.</span></span>|
|<span data-ttu-id="a607c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a607c-117">Application</span></span>| <span data-ttu-id="a607c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a607c-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a607c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a607c-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a607c-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a607c-120">Optional query parameters</span></span>
<span data-ttu-id="a607c-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a607c-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a607c-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a607c-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="a607c-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="a607c-123">Exceptions</span></span>
<span data-ttu-id="a607c-124">Alguns operadores não têm suporte: `$count` , `$search` , `$filter` .</span><span class="sxs-lookup"><span data-stu-id="a607c-124">Some operators are not supported: `$count`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a607c-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a607c-125">Request headers</span></span>
| <span data-ttu-id="a607c-126">Nome</span><span class="sxs-lookup"><span data-stu-id="a607c-126">Name</span></span>      |<span data-ttu-id="a607c-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a607c-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a607c-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="a607c-128">Authorization</span></span> | <span data-ttu-id="a607c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a607c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a607c-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a607c-131">Request body</span></span>
<span data-ttu-id="a607c-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a607c-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a607c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a607c-133">Response</span></span>

<span data-ttu-id="a607c-134">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos printConnector](../resources/printconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a607c-134">If successful, this method returns a `200 OK` response code and a collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a607c-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a607c-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a607c-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a607c-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a607c-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="a607c-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printconnector"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/connectors
```
# <a name="c"></a>[<span data-ttu-id="a607c-138">C#</span><span class="sxs-lookup"><span data-stu-id="a607c-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a607c-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a607c-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a607c-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a607c-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a607c-141">Java</span><span class="sxs-lookup"><span data-stu-id="a607c-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a607c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a607c-142">Response</span></span>
<span data-ttu-id="a607c-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a607c-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/connectors",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "Connector1",
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

