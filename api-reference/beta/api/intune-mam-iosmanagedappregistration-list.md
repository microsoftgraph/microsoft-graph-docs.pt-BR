---
title: Listar iosManagedAppRegistrations
description: Listar propriedades e relações dos objetos iosManagedAppRegistration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8b929a2a01126b1ec1803f005be1bf4e14f63938
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37193323"
---
# <a name="list-iosmanagedappregistrations"></a><span data-ttu-id="ca878-103">Listar iosManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="ca878-103">List iosManagedAppRegistrations</span></span>

> <span data-ttu-id="ca878-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ca878-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca878-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca878-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca878-106">Listar propriedades e relações dos objetos [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ca878-106">List properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca878-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ca878-107">Prerequisites</span></span>
<span data-ttu-id="ca878-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca878-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca878-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca878-110">Permission type</span></span>|<span data-ttu-id="ca878-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ca878-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca878-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca878-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca878-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca878-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ca878-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca878-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca878-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca878-115">Not supported.</span></span>|
|<span data-ttu-id="ca878-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca878-116">Application</span></span>|<span data-ttu-id="ca878-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca878-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca878-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca878-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="ca878-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca878-119">Request headers</span></span>
|<span data-ttu-id="ca878-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca878-120">Header</span></span>|<span data-ttu-id="ca878-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ca878-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca878-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca878-122">Authorization</span></span>|<span data-ttu-id="ca878-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca878-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca878-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ca878-124">Accept</span></span>|<span data-ttu-id="ca878-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca878-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca878-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca878-126">Request body</span></span>
<span data-ttu-id="ca878-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ca878-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca878-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca878-128">Response</span></span>
<span data-ttu-id="ca878-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca878-129">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca878-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca878-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca878-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca878-131">Request</span></span>
<span data-ttu-id="ca878-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca878-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="ca878-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca878-133">Response</span></span>
<span data-ttu-id="ca878-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca878-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1060

{
  "value": [
    {
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
  ]
}
```




