---
title: Obter windowsAutopilotDeviceIdentity
description: Leia as propriedades e as relações do objeto windowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: db567c3d79e6df3a4f03603fa7506c3c451d4476
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959807"
---
# <a name="get-windowsautopilotdeviceidentity"></a><span data-ttu-id="9eb24-103">Obter windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="9eb24-103">Get windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="9eb24-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9eb24-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9eb24-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9eb24-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9eb24-106">Leia as propriedades e as relações do objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="9eb24-106">Read properties and relationships of the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9eb24-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9eb24-107">Prerequisites</span></span>
<span data-ttu-id="9eb24-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9eb24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9eb24-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9eb24-110">Permission type</span></span>|<span data-ttu-id="9eb24-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9eb24-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9eb24-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9eb24-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9eb24-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9eb24-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="9eb24-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9eb24-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9eb24-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9eb24-115">Not supported.</span></span>|
|<span data-ttu-id="9eb24-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9eb24-116">Application</span></span>|<span data-ttu-id="9eb24-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9eb24-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9eb24-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9eb24-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9eb24-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9eb24-119">Optional query parameters</span></span>
<span data-ttu-id="9eb24-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9eb24-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9eb24-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9eb24-121">Request headers</span></span>
|<span data-ttu-id="9eb24-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9eb24-122">Header</span></span>|<span data-ttu-id="9eb24-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9eb24-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9eb24-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9eb24-124">Authorization</span></span>|<span data-ttu-id="9eb24-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9eb24-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9eb24-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9eb24-126">Accept</span></span>|<span data-ttu-id="9eb24-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9eb24-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9eb24-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9eb24-128">Request body</span></span>
<span data-ttu-id="9eb24-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9eb24-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9eb24-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9eb24-130">Response</span></span>
<span data-ttu-id="9eb24-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9eb24-131">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9eb24-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9eb24-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9eb24-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9eb24-133">Request</span></span>
<span data-ttu-id="9eb24-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9eb24-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="9eb24-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9eb24-135">Response</span></span>
<span data-ttu-id="9eb24-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9eb24-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1109

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
    "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
    "deploymentProfileAssignmentStatus": "assignedInSync",
    "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
    "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
    "orderIdentifier": "Order Identifier value",
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
    "managedDeviceId": "Managed Device Id value"
  }
}
```




