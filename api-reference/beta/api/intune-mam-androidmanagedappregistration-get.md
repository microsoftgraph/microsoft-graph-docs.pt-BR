---
title: Get androidManagedAppRegistration
description: Ler propriedades e relações do objeto androidManagedAppRegistration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1bf714c1aa80719ab1320d06ceae9965d6c4b301
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803684"
---
# <a name="get-androidmanagedappregistration"></a><span data-ttu-id="58700-103">Get androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="58700-103">Get androidManagedAppRegistration</span></span>

> <span data-ttu-id="58700-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="58700-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58700-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58700-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58700-106">Ler propriedades e relações do objeto [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="58700-106">Read properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58700-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="58700-107">Prerequisites</span></span>
<span data-ttu-id="58700-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58700-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58700-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58700-110">Permission type</span></span>|<span data-ttu-id="58700-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="58700-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58700-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58700-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58700-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="58700-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="58700-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58700-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58700-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58700-115">Not supported.</span></span>|
|<span data-ttu-id="58700-116">Application</span><span class="sxs-lookup"><span data-stu-id="58700-116">Application</span></span>|<span data-ttu-id="58700-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="58700-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58700-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58700-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="58700-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="58700-119">Optional query parameters</span></span>
<span data-ttu-id="58700-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="58700-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58700-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58700-121">Request headers</span></span>
|<span data-ttu-id="58700-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58700-122">Header</span></span>|<span data-ttu-id="58700-123">Valor</span><span class="sxs-lookup"><span data-stu-id="58700-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58700-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="58700-124">Authorization</span></span>|<span data-ttu-id="58700-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58700-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58700-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="58700-126">Accept</span></span>|<span data-ttu-id="58700-127">application/json</span><span class="sxs-lookup"><span data-stu-id="58700-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58700-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58700-128">Request body</span></span>
<span data-ttu-id="58700-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="58700-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58700-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="58700-130">Response</span></span>
<span data-ttu-id="58700-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58700-131">If successful, this method returns a `200 OK` response code and [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58700-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58700-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="58700-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58700-133">Request</span></span>
<span data-ttu-id="58700-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58700-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="58700-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="58700-135">Response</span></span>
<span data-ttu-id="58700-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58700-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1054

{
  "value": {
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
}
```




