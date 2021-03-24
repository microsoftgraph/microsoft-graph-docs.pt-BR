---
title: Listar androidManagedAppRegistrations
description: Listar propriedades e relações dos objetos androidManagedAppRegistration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 578f5a735d32fb89af37a8b1396d2344ff1ca28c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145471"
---
# <a name="list-androidmanagedappregistrations"></a><span data-ttu-id="e5286-103">Listar androidManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="e5286-103">List androidManagedAppRegistrations</span></span>

<span data-ttu-id="e5286-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5286-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5286-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e5286-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5286-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e5286-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5286-107">Listar propriedades e relações dos objetos [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e5286-107">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5286-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e5286-108">Prerequisites</span></span>
<span data-ttu-id="e5286-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5286-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5286-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5286-111">Permission type</span></span>|<span data-ttu-id="e5286-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5286-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5286-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5286-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5286-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5286-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e5286-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5286-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5286-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5286-116">Not supported.</span></span>|
|<span data-ttu-id="e5286-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5286-117">Application</span></span>|<span data-ttu-id="e5286-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5286-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5286-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5286-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="e5286-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5286-120">Request headers</span></span>
|<span data-ttu-id="e5286-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e5286-121">Header</span></span>|<span data-ttu-id="e5286-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e5286-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5286-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5286-123">Authorization</span></span>|<span data-ttu-id="e5286-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5286-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5286-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e5286-125">Accept</span></span>|<span data-ttu-id="e5286-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5286-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5286-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5286-127">Request body</span></span>
<span data-ttu-id="e5286-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5286-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5286-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5286-129">Response</span></span>
<span data-ttu-id="e5286-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5286-130">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5286-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5286-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5286-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5286-132">Request</span></span>
<span data-ttu-id="e5286-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5286-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="e5286-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5286-134">Response</span></span>
<span data-ttu-id="e5286-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5286-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




