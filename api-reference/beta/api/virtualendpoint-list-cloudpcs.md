---
title: Listar cloudPCs
description: Listar Propriedades e relações dos objetos cloudPC.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: cb7b5e79d3fd490fc574fbfbb8c08988321bc86d
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378252"
---
# <a name="list-cloudpcs"></a><span data-ttu-id="8263c-103">Listar cloudPCs</span><span class="sxs-lookup"><span data-stu-id="8263c-103">List cloudPCs</span></span>

<span data-ttu-id="8263c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8263c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8263c-105">Listar Propriedades e relações dos objetos [cloudPC](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="8263c-105">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8263c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="8263c-106">Permissions</span></span>

<span data-ttu-id="8263c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8263c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8263c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8263c-109">Permission type</span></span>|<span data-ttu-id="8263c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8263c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8263c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8263c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8263c-112">CloudPC. ReadWrite. All, CloudPC. Read. All</span><span class="sxs-lookup"><span data-stu-id="8263c-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="8263c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8263c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8263c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8263c-114">Not supported.</span></span>|
|<span data-ttu-id="8263c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8263c-115">Application</span></span>|<span data-ttu-id="8263c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8263c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8263c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8263c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/cloudPCs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8263c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8263c-118">Optional query parameters</span></span>

<span data-ttu-id="8263c-119">Este método oferece `$select` suporte `$filter` e `$count` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8263c-119">This method supports `$select`, `$filter` and `$count` OData query parameters to help customize the response.</span></span> <span data-ttu-id="8263c-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8263c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8263c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8263c-121">Request headers</span></span>

| <span data-ttu-id="8263c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8263c-122">Name</span></span>          | <span data-ttu-id="8263c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8263c-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8263c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8263c-124">Authorization</span></span> | <span data-ttu-id="8263c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8263c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8263c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8263c-127">Request body</span></span>

<span data-ttu-id="8263c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8263c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8263c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8263c-129">Response</span></span>

<span data-ttu-id="8263c-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [cloudPC](../resources/cloudpc.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8263c-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPC](../resources/cloudpc.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8263c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8263c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8263c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8263c-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_cloudpcs"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs
```

### <a name="response"></a><span data-ttu-id="8263c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8263c-133">Response</span></span>

<span data-ttu-id="8263c-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8263c-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPC)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPC",
      "id": "662009bc-7732-4f6f-8726-25883518ffff",
      "displayName": "Display Name value",
      "imageDisplayName": "Image Display Name value",
      "managedDeviceId": "bdc8e6dd-0455-4412-83d9-c818664fffff",
      "managedDeviceName": "Managed Device Name value",
      "provisioningPolicyId": "7ed725ad-0a00-4117-b557-d965c373ffff",
      "servicePlanId": "dbb9148c-ff83-4a4c-8d7f-28752e93ffff",
      "servicePlanName": "lite",
      "status": "provisioned",
      "userPrincipalName": "User Principal Name value",
      "lastModifiedDateTime": "2020-11-03T10:29:57Z",
      "statusDetails": null
    }
  ]
}
```
