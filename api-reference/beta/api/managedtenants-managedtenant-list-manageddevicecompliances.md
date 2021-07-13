---
title: Listar managedDeviceCompliances
description: Obter uma lista dos objetos managedDeviceCompliance e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 0376c59d5a43f4c5d8b4dc9aa4429fcbfee42d85
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401904"
---
# <a name="list-manageddevicecompliances"></a><span data-ttu-id="41dc7-103">Listar managedDeviceCompliances</span><span class="sxs-lookup"><span data-stu-id="41dc7-103">List managedDeviceCompliances</span></span>
<span data-ttu-id="41dc7-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="41dc7-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41dc7-105">Obter uma lista dos [objetos managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="41dc7-105">Get a list of the [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="41dc7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="41dc7-106">Permissions</span></span>
<span data-ttu-id="41dc7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41dc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41dc7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41dc7-109">Permission type</span></span>|<span data-ttu-id="41dc7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41dc7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41dc7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41dc7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="41dc7-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41dc7-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="41dc7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41dc7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41dc7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41dc7-114">Not supported.</span></span>|
|<span data-ttu-id="41dc7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41dc7-115">Application</span></span>|<span data-ttu-id="41dc7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41dc7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41dc7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41dc7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managedDeviceCompliances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41dc7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="41dc7-118">Optional query parameters</span></span>
<span data-ttu-id="41dc7-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="41dc7-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41dc7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41dc7-120">Request headers</span></span>
|<span data-ttu-id="41dc7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="41dc7-121">Name</span></span>|<span data-ttu-id="41dc7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="41dc7-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="41dc7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="41dc7-123">Authorization</span></span>|<span data-ttu-id="41dc7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41dc7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="41dc7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41dc7-126">Request body</span></span>
<span data-ttu-id="41dc7-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41dc7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41dc7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="41dc7-128">Response</span></span>

<span data-ttu-id="41dc7-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41dc7-129">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="41dc7-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="41dc7-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="41dc7-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41dc7-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_manageddevicecompliance"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managedDeviceCompliances
```


### <a name="response"></a><span data-ttu-id="41dc7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="41dc7-132">Response</span></span>
><span data-ttu-id="41dc7-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="41dc7-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.managedDeviceCompliance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#managedDeviceCompliances",
  "value": [
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320_6dd4fe4b-5ea2-4ab2-8ac4-7dd2995f1649",
      "managedDeviceId": "6dd4fe4b-5ea2-4ab2-8ac4-7dd2995f1649",
      "managedDeviceName": "VM2688",
      "complianceStatus": "Noncompliant",
      "osDescription": "Windows",
      "osVersion": "10.0.19042.1083",
      "lastSyncDateTime": "2021-07-09T14:38:56.379702Z",
      "ownerType": "Company",
      "model": "Virtual Machine",
      "manufacturer": "Microsoft Corporation",
      "inGracePeriodUntilDateTime": "2021-06-14T14:35:24.8225Z",
      "lastRefreshedDateTime": "2021-07-11T07:03:54.0326474Z",
      "deviceType": "WindowsRT",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantDisplayName": "Consolidated Messenger"
    },
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320_49ed91f1-32ac-4881-9c1b-b709ba29e31b",
      "managedDeviceId": "49ed91f1-32ac-4881-9c1b-b709ba29e31b",
      "managedDeviceName": "VM4511",
      "complianceStatus": "Noncompliant",
      "osDescription": "Windows",
      "osVersion": "10.0.19042.1052",
      "lastSyncDateTime": "2021-07-09T14:41:57.8785122Z",
      "ownerType": "Company",
      "model": "Virtual Machine",
      "manufacturer": "Microsoft Corporation",
      "inGracePeriodUntilDateTime": "2021-06-14T14:36:09.1851Z",
      "lastRefreshedDateTime": "2021-07-11T06:53:35.8484421Z",
      "deviceType": "WindowsRT",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantDisplayName": "Consolidated Messenger"
    }
  ]
}
```
