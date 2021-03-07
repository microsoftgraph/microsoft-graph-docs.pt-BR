---
title: Listar printConnectors
description: Recupere uma lista de conectores.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 3c6c7f8507599cb22eb0e37bc95860d10a5e3c9f
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516848"
---
# <a name="list-printconnectors"></a><span data-ttu-id="a691a-103">Listar printConnectors</span><span class="sxs-lookup"><span data-stu-id="a691a-103">List printConnectors</span></span>
<span data-ttu-id="a691a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a691a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="a691a-105">Recupere uma lista de conectores de impressão.</span><span class="sxs-lookup"><span data-stu-id="a691a-105">Retrieve a list of print connectors.</span></span>

## <a name="permissions"></a><span data-ttu-id="a691a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a691a-106">Permissions</span></span>
<span data-ttu-id="a691a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a691a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a691a-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="a691a-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="a691a-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="a691a-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="a691a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a691a-111">Permission type</span></span> | <span data-ttu-id="a691a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a691a-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a691a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a691a-113">Delegated (work or school account)</span></span>| <span data-ttu-id="a691a-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a691a-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="a691a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a691a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a691a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a691a-116">Not Supported.</span></span>|
|<span data-ttu-id="a691a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a691a-117">Application</span></span>| <span data-ttu-id="a691a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a691a-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a691a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a691a-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a691a-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a691a-120">Optional query parameters</span></span>
<span data-ttu-id="a691a-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a691a-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a691a-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a691a-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="a691a-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="a691a-123">Exceptions</span></span>
<span data-ttu-id="a691a-124">Alguns operadores não têm suporte: `$count` , `$search` , `$filter` .</span><span class="sxs-lookup"><span data-stu-id="a691a-124">Some operators are not supported: `$count`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a691a-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a691a-125">Request headers</span></span>
| <span data-ttu-id="a691a-126">Nome</span><span class="sxs-lookup"><span data-stu-id="a691a-126">Name</span></span>      |<span data-ttu-id="a691a-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a691a-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a691a-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="a691a-128">Authorization</span></span> | <span data-ttu-id="a691a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a691a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a691a-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a691a-131">Request body</span></span>
<span data-ttu-id="a691a-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a691a-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a691a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a691a-133">Response</span></span>

<span data-ttu-id="a691a-134">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos printConnector](../resources/printconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a691a-134">If successful, this method returns a `200 OK` response code and a collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a691a-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a691a-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a691a-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a691a-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printconnector"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/connectors
```

### <a name="response"></a><span data-ttu-id="a691a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a691a-137">Response</span></span>
<span data-ttu-id="a691a-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a691a-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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

