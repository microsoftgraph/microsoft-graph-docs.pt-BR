---
title: Listar androidManagedAppRegistrations
description: Listar propriedades e relações dos objetos androidManagedAppRegistration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 714ae4a22a00d5f4dab8fbe07b44b2d928b13876
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35994940"
---
# <a name="list-androidmanagedappregistrations"></a><span data-ttu-id="6d375-103">Listar androidManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="6d375-103">List androidManagedAppRegistrations</span></span>

> <span data-ttu-id="6d375-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6d375-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d375-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d375-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d375-106">Listar propriedades e relações dos objetos [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6d375-106">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d375-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6d375-107">Prerequisites</span></span>
<span data-ttu-id="6d375-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d375-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d375-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d375-110">Permission type</span></span>|<span data-ttu-id="6d375-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6d375-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d375-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d375-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6d375-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d375-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6d375-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d375-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d375-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d375-115">Not supported.</span></span>|
|<span data-ttu-id="6d375-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d375-116">Application</span></span>|<span data-ttu-id="6d375-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d375-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d375-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d375-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="6d375-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d375-119">Request headers</span></span>
|<span data-ttu-id="6d375-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6d375-120">Header</span></span>|<span data-ttu-id="6d375-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6d375-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d375-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d375-122">Authorization</span></span>|<span data-ttu-id="6d375-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d375-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d375-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6d375-124">Accept</span></span>|<span data-ttu-id="6d375-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6d375-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d375-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d375-126">Request body</span></span>
<span data-ttu-id="6d375-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6d375-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d375-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d375-128">Response</span></span>
<span data-ttu-id="6d375-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d375-129">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d375-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d375-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d375-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d375-131">Request</span></span>
<span data-ttu-id="6d375-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d375-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="6d375-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d375-133">Response</span></span>
<span data-ttu-id="6d375-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d375-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1116

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
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
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "id": "0e064997-4997-0e06-9749-060e9749060e",
      "version": "Version value",
      "patchVersion": "Patch Version value"
    }
  ]
}
```





