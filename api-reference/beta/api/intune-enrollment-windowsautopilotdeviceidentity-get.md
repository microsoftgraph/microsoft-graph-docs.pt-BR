---
title: Obter windowsAutopilotDeviceIdentity
description: Leia as propriedades e as relações do objeto windowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 58f39920d386d50050f8e1c1dd6fa08d5148f3d3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452383"
---
# <a name="get-windowsautopilotdeviceidentity"></a><span data-ttu-id="b9ad5-103">Obter windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="b9ad5-103">Get windowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="b9ad5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9ad5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9ad5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b9ad5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9ad5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9ad5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9ad5-107">Leia as propriedades e as relações do objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="b9ad5-107">Read properties and relationships of the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9ad5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b9ad5-108">Prerequisites</span></span>
<span data-ttu-id="b9ad5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9ad5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9ad5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9ad5-111">Permission type</span></span>|<span data-ttu-id="b9ad5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b9ad5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9ad5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9ad5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9ad5-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9ad5-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b9ad5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9ad5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9ad5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9ad5-116">Not supported.</span></span>|
|<span data-ttu-id="b9ad5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9ad5-117">Application</span></span>|<span data-ttu-id="b9ad5-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9ad5-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9ad5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9ad5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9ad5-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b9ad5-120">Optional query parameters</span></span>
<span data-ttu-id="b9ad5-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b9ad5-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9ad5-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9ad5-122">Request headers</span></span>
|<span data-ttu-id="b9ad5-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9ad5-123">Header</span></span>|<span data-ttu-id="b9ad5-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b9ad5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9ad5-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9ad5-125">Authorization</span></span>|<span data-ttu-id="b9ad5-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9ad5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9ad5-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b9ad5-127">Accept</span></span>|<span data-ttu-id="b9ad5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b9ad5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9ad5-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9ad5-129">Request body</span></span>
<span data-ttu-id="b9ad5-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9ad5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9ad5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9ad5-131">Response</span></span>
<span data-ttu-id="b9ad5-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9ad5-132">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9ad5-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9ad5-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9ad5-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9ad5-134">Request</span></span>
<span data-ttu-id="b9ad5-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9ad5-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="b9ad5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9ad5-136">Response</span></span>
<span data-ttu-id="b9ad5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9ad5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1187

{
  "value": {
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
}
```



