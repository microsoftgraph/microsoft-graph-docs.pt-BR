---
title: Listar windowsAutopilotDeviceIdentities
description: Listar Propriedades e relações dos objetos windowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 18d8c681dcd5c9bbc3dc44feeeeb98169dd06119
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696640"
---
# <a name="list-windowsautopilotdeviceidentities"></a><span data-ttu-id="33563-103">Listar windowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="33563-103">List windowsAutopilotDeviceIdentities</span></span>

<span data-ttu-id="33563-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33563-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33563-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="33563-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33563-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="33563-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33563-107">Listar Propriedades e relações dos objetos [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="33563-107">List properties and relationships of the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33563-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="33563-108">Prerequisites</span></span>
<span data-ttu-id="33563-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33563-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33563-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33563-111">Permission type</span></span>|<span data-ttu-id="33563-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="33563-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33563-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33563-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33563-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="33563-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="33563-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33563-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33563-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33563-116">Not supported.</span></span>|
|<span data-ttu-id="33563-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33563-117">Application</span></span>|<span data-ttu-id="33563-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="33563-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33563-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33563-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="33563-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33563-120">Request headers</span></span>
|<span data-ttu-id="33563-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33563-121">Header</span></span>|<span data-ttu-id="33563-122">Valor</span><span class="sxs-lookup"><span data-stu-id="33563-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33563-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="33563-123">Authorization</span></span>|<span data-ttu-id="33563-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33563-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33563-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="33563-125">Accept</span></span>|<span data-ttu-id="33563-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33563-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33563-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33563-127">Request body</span></span>
<span data-ttu-id="33563-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="33563-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33563-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="33563-129">Response</span></span>
<span data-ttu-id="33563-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33563-130">If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33563-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33563-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="33563-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33563-132">Request</span></span>
<span data-ttu-id="33563-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33563-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="33563-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="33563-134">Response</span></span>
<span data-ttu-id="33563-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33563-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





