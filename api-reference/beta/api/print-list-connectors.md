---
title: Listar reconectadores
description: Recupere uma lista de conectores.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 396570be7fd8d7a70b764076b52de57fe03ee53d
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314941"
---
# <a name="list-printconnectors"></a><span data-ttu-id="2f1cb-103">Listar reconectadores</span><span class="sxs-lookup"><span data-stu-id="2f1cb-103">List printConnectors</span></span>

<span data-ttu-id="2f1cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f1cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f1cb-105">Recupere uma lista de conectores de impressão.</span><span class="sxs-lookup"><span data-stu-id="2f1cb-105">Retrieve a list of print connectors.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f1cb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f1cb-106">Permissions</span></span>
<span data-ttu-id="2f1cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f1cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2f1cb-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="2f1cb-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="2f1cb-110">O usuário conectado deve ser um [administrador da impressora](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="2f1cb-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="2f1cb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f1cb-111">Permission type</span></span> | <span data-ttu-id="2f1cb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f1cb-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="2f1cb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f1cb-113">Delegated (work or school account)</span></span>| <span data-ttu-id="2f1cb-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="2f1cb-114">User.Read</span></span> |
|<span data-ttu-id="2f1cb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f1cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f1cb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f1cb-116">Not Supported.</span></span>|
|<span data-ttu-id="2f1cb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f1cb-117">Application</span></span>| <span data-ttu-id="2f1cb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f1cb-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f1cb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f1cb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f1cb-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2f1cb-120">Optional query parameters</span></span>
<span data-ttu-id="2f1cb-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2f1cb-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2f1cb-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2f1cb-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="2f1cb-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="2f1cb-123">Exceptions</span></span>
<span data-ttu-id="2f1cb-124">Não há suporte para alguns operadores: `$count` , `$orderby` , `$search` , `$filter` .</span><span class="sxs-lookup"><span data-stu-id="2f1cb-124">Some operators are not supported: `$count`, `$orderby`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f1cb-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f1cb-125">Request headers</span></span>
| <span data-ttu-id="2f1cb-126">Nome</span><span class="sxs-lookup"><span data-stu-id="2f1cb-126">Name</span></span>      |<span data-ttu-id="2f1cb-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f1cb-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2f1cb-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f1cb-128">Authorization</span></span> | <span data-ttu-id="2f1cb-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f1cb-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f1cb-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f1cb-131">Request body</span></span>
<span data-ttu-id="2f1cb-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2f1cb-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2f1cb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f1cb-133">Response</span></span>
<span data-ttu-id="2f1cb-134">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de objetos de [multiconnector](../resources/printconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f1cb-134">If successful, this method returns a `200 OK` response code and collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2f1cb-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f1cb-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f1cb-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f1cb-136">Request</span></span>
<span data-ttu-id="2f1cb-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f1cb-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2f1cb-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f1cb-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/connectors
```
# <a name="c"></a>[<span data-ttu-id="2f1cb-139">C#</span><span class="sxs-lookup"><span data-stu-id="2f1cb-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f1cb-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f1cb-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f1cb-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f1cb-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2f1cb-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f1cb-142">Response</span></span>
<span data-ttu-id="2f1cb-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2f1cb-143">The following is an example of the response.</span></span>
><span data-ttu-id="2f1cb-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f1cb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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