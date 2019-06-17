---
title: Get iosManagedAppRegistration
description: Ler propriedades e relações do objeto iosManagedAppRegistration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2a743f71d6e69ac84ae43e00c3c2dff6bb9ccde
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34985973"
---
# <a name="get-iosmanagedappregistration"></a><span data-ttu-id="27862-103">Get iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="27862-103">Get iosManagedAppRegistration</span></span>

> <span data-ttu-id="27862-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="27862-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27862-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="27862-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27862-106">Ler propriedades e relações do objeto [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="27862-106">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27862-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27862-107">Prerequisites</span></span>
<span data-ttu-id="27862-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27862-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27862-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27862-110">Permission type</span></span>|<span data-ttu-id="27862-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="27862-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27862-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27862-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27862-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="27862-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="27862-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27862-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27862-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27862-115">Not supported.</span></span>|
|<span data-ttu-id="27862-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27862-116">Application</span></span>|<span data-ttu-id="27862-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27862-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27862-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27862-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="27862-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="27862-119">Optional query parameters</span></span>
<span data-ttu-id="27862-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="27862-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="27862-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27862-121">Request headers</span></span>
|<span data-ttu-id="27862-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27862-122">Header</span></span>|<span data-ttu-id="27862-123">Valor</span><span class="sxs-lookup"><span data-stu-id="27862-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27862-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="27862-124">Authorization</span></span>|<span data-ttu-id="27862-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27862-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27862-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="27862-126">Accept</span></span>|<span data-ttu-id="27862-127">application/json</span><span class="sxs-lookup"><span data-stu-id="27862-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27862-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27862-128">Request body</span></span>
<span data-ttu-id="27862-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27862-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27862-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="27862-130">Response</span></span>
<span data-ttu-id="27862-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27862-131">If successful, this method returns a `200 OK` response code and [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27862-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27862-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="27862-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27862-133">Request</span></span>
<span data-ttu-id="27862-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27862-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="27862-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="27862-135">Response</span></span>
<span data-ttu-id="27862-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27862-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1000

{
  "value": {
    "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "applicationVersion": "Application Version value",
    "managementSdkVersion": "Management Sdk Version value",
    "platformVersion": "Platform Version value",
    "deviceType": "Device Type value",
    "deviceTag": "Device Tag value",
    "deviceName": "Device Name value",
    "managedDeviceId": "Managed Device Id value",
    "azureADDeviceId": "Azure ADDevice Id value",
    "deviceModel": "Device Model value",
    "deviceManufacturer": "Device Manufacturer value",
    "flaggedReasons": [
      "rootedDevice"
    ],
    "userId": "User Id value",
    "appIdentifier": {
      "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
      "bundleId": "Bundle Id value"
    },
    "id": "47632c19-2c19-4763-192c-6347192c6347",
    "version": "Version value"
  }
}
```





