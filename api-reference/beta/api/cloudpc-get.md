---
title: Obter cloudPC
description: Exibir as propriedades e as relações de um objeto cloudPC.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: ad63ff3f4d152005624872f94482b44cb862ef9f
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082206"
---
# <a name="get-cloudpc"></a><span data-ttu-id="9047e-103">Obter cloudPC</span><span class="sxs-lookup"><span data-stu-id="9047e-103">Get cloudPC</span></span>

<span data-ttu-id="9047e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9047e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9047e-105">Leia as propriedades e as relações de um objeto [cloudPC](../resources/cloudpc.md) específico.</span><span class="sxs-lookup"><span data-stu-id="9047e-105">Read the properties and relationships of a specific [cloudPC](../resources/cloudpc.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="9047e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9047e-106">Permissions</span></span>

<span data-ttu-id="9047e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9047e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9047e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9047e-109">Permission type</span></span>|<span data-ttu-id="9047e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9047e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9047e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9047e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9047e-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9047e-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="9047e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9047e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9047e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9047e-114">Not supported.</span></span>|
|<span data-ttu-id="9047e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9047e-115">Application</span></span>|<span data-ttu-id="9047e-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9047e-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9047e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9047e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/cloudPCs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9047e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9047e-118">Optional query parameters</span></span>

<span data-ttu-id="9047e-119">Este método dá suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9047e-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="9047e-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9047e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9047e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9047e-121">Request headers</span></span>

| <span data-ttu-id="9047e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9047e-122">Name</span></span>          | <span data-ttu-id="9047e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9047e-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9047e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9047e-124">Authorization</span></span> | <span data-ttu-id="9047e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9047e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9047e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9047e-127">Request body</span></span>

<span data-ttu-id="9047e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9047e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9047e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9047e-129">Response</span></span>

<span data-ttu-id="9047e-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [cloudPC](../resources/cloudpc.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9047e-130">If successful, this method returns a `200 OK` response code and a [cloudPC](../resources/cloudpc.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9047e-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9047e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9047e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9047e-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9047e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9047e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpc"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs/{id}
```
# <a name="c"></a>[<span data-ttu-id="9047e-134">C#</span><span class="sxs-lookup"><span data-stu-id="9047e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9047e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9047e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9047e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9047e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9047e-137">Java</span><span class="sxs-lookup"><span data-stu-id="9047e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9047e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9047e-138">Response</span></span>

<span data-ttu-id="9047e-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9047e-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_cloudpc",
  "@odata.type": "microsoft.graph.cloudPC"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPC",
    "id": "ac74ae8b-85f7-4272-88cc-54192674ffff",
    "displayName": "Demo-0",
    "imageDisplayName": "Windows-10 19h1-evd",
    "managedDeviceId": "e87f50c7-fa7f-4687-aade-dd45f3d6ffff",  
    "managedDeviceName": "A00002GI001",
    "provisioningPolicyId": "13fa0778-ba00-438a-96d3-488c8602ffff",
    "provisioningPolicyName": "Marketing provisioning policy",
    "onPremisesConnectionName": "on-Premises connection for Marketing",
    "servicePlanId": "da5615b4-a484-4742-a019-2d52c91cffff",
    "servicePlanName": "standard",
    "status": "failed",
    "statusDetails": {
    "@odata.type": "microsoft.graph.cloudPcStatusDetails",
    "code": "internalServerError",
    "message": "There was an internal server error. Please contact support xxx.",
    "additionalInformation": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "correlationId",
          "value": "52367774-cfb7-4e9c-ab51-1b864c31f2d1"
        }
      ]
    },
    "userPrincipalName": "pmitchell@cpccustomer001.onmicrosoft.com",
    "lastModifiedDateTime": "2020-11-03T18:14:34Z",
    "gracePeriodEndDateTime": "2020-11-010T20:00:34Z"
  }
}
```
