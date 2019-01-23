---
title: Listar iosManagedAppRegistrations
description: Lista propriedades e relações dos objetos iosManagedAppRegistration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 258becf30b23b02d84318523515c5b7c6d07a13d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419125"
---
# <a name="list-iosmanagedappregistrations"></a><span data-ttu-id="d9511-103">Listar iosManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="d9511-103">List iosManagedAppRegistrations</span></span>

> <span data-ttu-id="d9511-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="d9511-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d9511-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d9511-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9511-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="d9511-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9511-107">Listar propriedades e relações dos objetos [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d9511-107">List properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9511-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d9511-108">Prerequisites</span></span>
<span data-ttu-id="d9511-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d9511-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d9511-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9511-111">Permission type</span></span>|<span data-ttu-id="d9511-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d9511-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9511-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9511-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9511-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9511-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d9511-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9511-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9511-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9511-116">Not supported.</span></span>|
|<span data-ttu-id="d9511-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9511-117">Application</span></span>|<span data-ttu-id="d9511-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9511-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9511-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9511-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="d9511-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9511-120">Request headers</span></span>
|<span data-ttu-id="d9511-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9511-121">Header</span></span>|<span data-ttu-id="d9511-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d9511-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9511-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9511-123">Authorization</span></span>|<span data-ttu-id="d9511-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9511-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9511-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d9511-125">Accept</span></span>|<span data-ttu-id="d9511-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9511-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9511-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9511-127">Request body</span></span>
<span data-ttu-id="d9511-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9511-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9511-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9511-129">Response</span></span>
<span data-ttu-id="d9511-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9511-130">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9511-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9511-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9511-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9511-132">Request</span></span>
<span data-ttu-id="d9511-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9511-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="d9511-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9511-134">Response</span></span>
<span data-ttu-id="d9511-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9511-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




