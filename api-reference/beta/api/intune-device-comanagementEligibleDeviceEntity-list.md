---
title: Listar comanagementEligibleDeviceEntity
description: Listar Propriedades e relações dos objetos comanagementEligibleDeviceEntity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 39d7a92c5914107cdd5ecfebb9b4b7948bc8b8b0
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636032"
---
# <a name="list-comanagementeligibledeviceentity"></a><span data-ttu-id="64959-103">Listar comanagementEligibleDeviceEntity</span><span class="sxs-lookup"><span data-stu-id="64959-103">List comanagementEligibleDeviceEntity</span></span>

> <span data-ttu-id="64959-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="64959-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64959-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64959-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64959-106">Listar Propriedades e relações dos objetos comanagementEligibleDeviceEntity.</span><span class="sxs-lookup"><span data-stu-id="64959-106">List properties and relationships of the comanagementEligibleDeviceEntity objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64959-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="64959-107">Prerequisites</span></span>
<span data-ttu-id="64959-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64959-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64959-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64959-110">Permission type</span></span>|<span data-ttu-id="64959-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="64959-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64959-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64959-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64959-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="64959-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="64959-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64959-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64959-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64959-115">Not supported.</span></span>|
|<span data-ttu-id="64959-116">Application</span><span class="sxs-lookup"><span data-stu-id="64959-116">Application</span></span>|<span data-ttu-id="64959-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="64959-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64959-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64959-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/comanagementEligibleReports
```

## <a name="request-headers"></a><span data-ttu-id="64959-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64959-119">Request headers</span></span>
|<span data-ttu-id="64959-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64959-120">Header</span></span>|<span data-ttu-id="64959-121">Valor</span><span class="sxs-lookup"><span data-stu-id="64959-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64959-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="64959-122">Authorization</span></span>|<span data-ttu-id="64959-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64959-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64959-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="64959-124">Accept</span></span>|<span data-ttu-id="64959-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64959-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64959-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64959-126">Request body</span></span>
<span data-ttu-id="64959-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64959-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64959-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="64959-128">Response</span></span>
<span data-ttu-id="64959-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos comanagementEligibleDeviceEntity no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64959-129">If successful, this method returns a `200 OK` response code and a collection of comanagementEligibleDeviceEntity objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64959-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64959-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="64959-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64959-131">Request</span></span>
<span data-ttu-id="64959-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64959-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/comanagementEligibleReports
```

### <a name="response"></a><span data-ttu-id="64959-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="64959-133">Response</span></span>
<span data-ttu-id="64959-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64959-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1303

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.comanagementEligibleDeviceEntity",
      "id": "659554f2-54f2-6595-f254-9565f2549565",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "deviceType": "Device Type value",
      "clientRegistrationStatus": "Client Registration Status value",
      "ownerType": "Owner Type value",
      "managementAgents": "Management Agent value",
      "managementState": "Management State value",
      "referenceId": "Reference Id value",
      "mdmStatus": "MDM Status value",
      "osVersion": "OS Version value",
      "serialNumber": "Serial Number value",
      "manufacturer": "Manufacture value",
      "model": "Model value",
      "osDescription": "OS Description value",
      "entitySource": 1024,
      "userId": "User Id value",
      "upn": "UPN value",
      "userEmail": "User Email value",
      "userName": "User name value",
      "coManageEligibleStatus": "CO Manage Eligible Status value"
    }
  ]
}
```



