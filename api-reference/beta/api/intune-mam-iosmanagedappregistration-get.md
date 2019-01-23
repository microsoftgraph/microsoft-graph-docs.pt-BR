---
title: Get iosManagedAppRegistration
description: Ler propriedades e relações do objeto iosManagedAppRegistration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0b104724698416e03af02f483065eb010e905538
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414869"
---
# <a name="get-iosmanagedappregistration"></a><span data-ttu-id="43142-103">Get iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="43142-103">Get iosManagedAppRegistration</span></span>

> <span data-ttu-id="43142-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="43142-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="43142-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="43142-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43142-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="43142-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43142-107">Ler propriedades e relações do objeto [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="43142-107">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43142-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="43142-108">Prerequisites</span></span>
<span data-ttu-id="43142-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="43142-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="43142-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43142-111">Permission type</span></span>|<span data-ttu-id="43142-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="43142-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43142-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43142-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43142-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="43142-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="43142-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43142-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43142-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43142-116">Not supported.</span></span>|
|<span data-ttu-id="43142-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43142-117">Application</span></span>|<span data-ttu-id="43142-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43142-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43142-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43142-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43142-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="43142-120">Optional query parameters</span></span>
<span data-ttu-id="43142-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="43142-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43142-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43142-122">Request headers</span></span>
|<span data-ttu-id="43142-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43142-123">Header</span></span>|<span data-ttu-id="43142-124">Valor</span><span class="sxs-lookup"><span data-stu-id="43142-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43142-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="43142-125">Authorization</span></span>|<span data-ttu-id="43142-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43142-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43142-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="43142-127">Accept</span></span>|<span data-ttu-id="43142-128">application/json</span><span class="sxs-lookup"><span data-stu-id="43142-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43142-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43142-129">Request body</span></span>
<span data-ttu-id="43142-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="43142-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43142-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="43142-131">Response</span></span>
<span data-ttu-id="43142-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43142-132">If successful, this method returns a `200 OK` response code and [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43142-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43142-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="43142-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43142-134">Request</span></span>
<span data-ttu-id="43142-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="43142-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="43142-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="43142-136">Response</span></span>
<span data-ttu-id="43142-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43142-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




