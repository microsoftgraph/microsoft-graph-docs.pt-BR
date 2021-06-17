---
title: Obter cloudPC
description: Exibir as propriedades e as relações de um objeto cloudPC.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 0470f6000ed7699b10288407a9d92ca74cc8177e
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52990844"
---
# <a name="get-cloudpc"></a><span data-ttu-id="f9cd3-103">Obter cloudPC</span><span class="sxs-lookup"><span data-stu-id="f9cd3-103">Get cloudPC</span></span>

<span data-ttu-id="f9cd3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9cd3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9cd3-105">Leia as propriedades e as relações de um objeto [cloudPC](../resources/cloudpc.md) específico.</span><span class="sxs-lookup"><span data-stu-id="f9cd3-105">Read the properties and relationships of a specific [cloudPC](../resources/cloudpc.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="f9cd3-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f9cd3-106">Permissions</span></span>

<span data-ttu-id="f9cd3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9cd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9cd3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9cd3-109">Permission type</span></span>|<span data-ttu-id="f9cd3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9cd3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9cd3-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9cd3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f9cd3-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9cd3-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="f9cd3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9cd3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9cd3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9cd3-114">Not supported.</span></span>|
|<span data-ttu-id="f9cd3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9cd3-115">Application</span></span>|<span data-ttu-id="f9cd3-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9cd3-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9cd3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9cd3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/cloudPCs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f9cd3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f9cd3-118">Optional query parameters</span></span>

<span data-ttu-id="f9cd3-119">Este método dá suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f9cd3-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="f9cd3-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f9cd3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9cd3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9cd3-121">Request headers</span></span>

| <span data-ttu-id="f9cd3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f9cd3-122">Name</span></span>          | <span data-ttu-id="f9cd3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9cd3-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f9cd3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9cd3-124">Authorization</span></span> | <span data-ttu-id="f9cd3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9cd3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9cd3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9cd3-127">Request body</span></span>

<span data-ttu-id="f9cd3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f9cd3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9cd3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9cd3-129">Response</span></span>

<span data-ttu-id="f9cd3-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [cloudPC](../resources/cloudpc.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9cd3-130">If successful, this method returns a `200 OK` response code and a [cloudPC](../resources/cloudpc.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f9cd3-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f9cd3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f9cd3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9cd3-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f9cd3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9cd3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpc"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs/{id}
```
# <a name="c"></a>[<span data-ttu-id="f9cd3-134">C#</span><span class="sxs-lookup"><span data-stu-id="f9cd3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9cd3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9cd3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9cd3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9cd3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f9cd3-137">Java</span><span class="sxs-lookup"><span data-stu-id="f9cd3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f9cd3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9cd3-138">Response</span></span>

<span data-ttu-id="f9cd3-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f9cd3-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "displayName": "Display Name value",
    "imageDisplayName": "Image Display Name value",
    "managedDeviceId": "e87f50c7-fa7f-4687-aade-dd45f3d6ffff",  
    "managedDeviceName": "Device Name value",
    "provisioningPolicyId": "13fa0778-ba00-438a-96d3-488c8602ffff",
    "provisioningPolicyName": "Provisioning Policy Name value",
    "onPremisesConnectionName": "On-premises connection Name value",
    "servicePlanId": "da5615b4-a484-4742-a019-2d52c91cffff",
    "servicePlanName": "standard",
    "status": "failed",
    "statusDetails": {
    "@odata.type": "microsoft.graph.cloudPcStatusDetails",
    "code": "Sample code",
    "message": "Sample message",
    "additionalInformation": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Sample value"
        }
      ]
    },
    "userPrincipalName": "User Principal Name value",
    "lastModifiedDateTime": "2020-11-03T18:14:34Z",
    "gracePeriodEndDateTime": "Grace Period End Date Time value "
  }
}
```
