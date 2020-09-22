---
title: Listar managedAppRegistrations
description: Listar propriedades e relações dos objetos managedAppRegistration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 514aef9ee523c4d6ed0e8adcb21ebec1dc47ed16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011120"
---
# <a name="list-managedappregistrations"></a><span data-ttu-id="61913-103">Listar managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="61913-103">List managedAppRegistrations</span></span>

<span data-ttu-id="61913-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="61913-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61913-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="61913-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61913-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="61913-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61913-107">Listar propriedades e relações dos objetos [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="61913-107">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61913-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61913-108">Prerequisites</span></span>
<span data-ttu-id="61913-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61913-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61913-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61913-111">Permission type</span></span>|<span data-ttu-id="61913-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="61913-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61913-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61913-113">Delegated (work or school account)</span></span>|<span data-ttu-id="61913-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="61913-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="61913-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61913-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61913-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61913-116">Not supported.</span></span>|
|<span data-ttu-id="61913-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61913-117">Application</span></span>|<span data-ttu-id="61913-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="61913-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="61913-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61913-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="61913-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61913-120">Request headers</span></span>
|<span data-ttu-id="61913-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="61913-121">Header</span></span>|<span data-ttu-id="61913-122">Valor</span><span class="sxs-lookup"><span data-stu-id="61913-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61913-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="61913-123">Authorization</span></span>|<span data-ttu-id="61913-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61913-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61913-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="61913-125">Accept</span></span>|<span data-ttu-id="61913-126">application/json</span><span class="sxs-lookup"><span data-stu-id="61913-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61913-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61913-127">Request body</span></span>
<span data-ttu-id="61913-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="61913-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61913-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="61913-129">Response</span></span>
<span data-ttu-id="61913-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedAppRegistration](../resources/intune-mam-managedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61913-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61913-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61913-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="61913-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61913-132">Request</span></span>
<span data-ttu-id="61913-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61913-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="61913-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="61913-134">Response</span></span>
<span data-ttu-id="61913-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61913-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1063

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppRegistration",
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
      "id": "5496aa60-aa60-5496-60aa-965460aa9654",
      "version": "Version value"
    }
  ]
}
```






