---
title: Listar windowsAutopilotDeviceIdentities
description: Listar Propriedades e relações dos objetos windowsAutopilotDeviceIdentity.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b715e99fcbe430c864a9534941887e827def577f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42805007"
---
# <a name="list-windowsautopilotdeviceidentities"></a><span data-ttu-id="69687-103">Listar windowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="69687-103">List windowsAutopilotDeviceIdentities</span></span>

> <span data-ttu-id="69687-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="69687-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69687-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="69687-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69687-106">Listar Propriedades e relações dos objetos [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="69687-106">List properties and relationships of the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69687-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="69687-107">Prerequisites</span></span>
<span data-ttu-id="69687-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69687-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69687-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69687-110">Permission type</span></span>|<span data-ttu-id="69687-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="69687-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69687-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69687-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69687-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="69687-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="69687-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69687-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69687-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69687-115">Not supported.</span></span>|
|<span data-ttu-id="69687-116">Application</span><span class="sxs-lookup"><span data-stu-id="69687-116">Application</span></span>|<span data-ttu-id="69687-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="69687-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69687-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69687-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="69687-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69687-119">Request headers</span></span>
|<span data-ttu-id="69687-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="69687-120">Header</span></span>|<span data-ttu-id="69687-121">Valor</span><span class="sxs-lookup"><span data-stu-id="69687-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69687-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="69687-122">Authorization</span></span>|<span data-ttu-id="69687-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69687-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69687-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="69687-124">Accept</span></span>|<span data-ttu-id="69687-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69687-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69687-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69687-126">Request body</span></span>
<span data-ttu-id="69687-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="69687-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69687-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="69687-128">Response</span></span>
<span data-ttu-id="69687-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69687-129">If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69687-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69687-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="69687-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69687-131">Request</span></span>
<span data-ttu-id="69687-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="69687-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="69687-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="69687-133">Response</span></span>
<span data-ttu-id="69687-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69687-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1245

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
      "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
      "deploymentProfileAssignmentStatus": "assignedInSync",
      "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
      "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
      "orderIdentifier": "Order Identifier value",
      "groupTag": "Group Tag value",
      "purchaseOrderIdentifier": "Purchase Order Identifier value",
      "serialNumber": "Serial Number value",
      "productKey": "Product Key value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "enrollmentState": "enrolled",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "addressableUserName": "Addressable User Name value",
      "userPrincipalName": "User Principal Name value",
      "resourceName": "Resource Name value",
      "skuNumber": "Sku Number value",
      "systemFamily": "System Family value",
      "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
      "managedDeviceId": "Managed Device Id value",
      "displayName": "Display Name value"
    }
  ]
}
```




