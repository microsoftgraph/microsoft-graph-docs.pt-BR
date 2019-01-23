---
title: Listar androidManagedAppRegistrations
description: Lista propriedades e relações dos objetos androidManagedAppRegistration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8fb7abfba70411569e8ad0295fcb9b1adc47430b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411250"
---
# <a name="list-androidmanagedappregistrations"></a><span data-ttu-id="7e12e-103">Listar androidManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="7e12e-103">List androidManagedAppRegistrations</span></span>

> <span data-ttu-id="7e12e-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="7e12e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7e12e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7e12e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7e12e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="7e12e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e12e-107">Listar propriedades e relações dos objetos [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="7e12e-107">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e12e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7e12e-108">Prerequisites</span></span>
<span data-ttu-id="7e12e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7e12e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7e12e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e12e-111">Permission type</span></span>|<span data-ttu-id="7e12e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7e12e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e12e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e12e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7e12e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e12e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7e12e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e12e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e12e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e12e-116">Not supported.</span></span>|
|<span data-ttu-id="7e12e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e12e-117">Application</span></span>|<span data-ttu-id="7e12e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e12e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e12e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e12e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="7e12e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e12e-120">Request headers</span></span>
|<span data-ttu-id="7e12e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7e12e-121">Header</span></span>|<span data-ttu-id="7e12e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7e12e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e12e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e12e-123">Authorization</span></span>|<span data-ttu-id="7e12e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e12e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e12e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7e12e-125">Accept</span></span>|<span data-ttu-id="7e12e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7e12e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e12e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e12e-127">Request body</span></span>
<span data-ttu-id="7e12e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7e12e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e12e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e12e-129">Response</span></span>
<span data-ttu-id="7e12e-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e12e-130">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e12e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e12e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e12e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e12e-132">Request</span></span>
<span data-ttu-id="7e12e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e12e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="7e12e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e12e-134">Response</span></span>
<span data-ttu-id="7e12e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e12e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




