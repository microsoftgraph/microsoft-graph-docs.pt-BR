---
title: Get managedDeviceOverview
description: Ler propriedades e relações do objeto managedDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2659de7bceaf6c1daa4286faf07eb549287a42ec
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441554"
---
# <a name="get-manageddeviceoverview"></a><span data-ttu-id="71fdb-103">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="71fdb-103">Get managedDeviceOverview</span></span>

<span data-ttu-id="71fdb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71fdb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71fdb-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="71fdb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71fdb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71fdb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71fdb-107">Ler propriedades e relações do objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="71fdb-107">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71fdb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="71fdb-108">Prerequisites</span></span>
<span data-ttu-id="71fdb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71fdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71fdb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71fdb-111">Permission type</span></span>|<span data-ttu-id="71fdb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="71fdb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71fdb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71fdb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71fdb-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="71fdb-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="71fdb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71fdb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71fdb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71fdb-116">Not supported.</span></span>|
|<span data-ttu-id="71fdb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71fdb-117">Application</span></span>|<span data-ttu-id="71fdb-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="71fdb-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71fdb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71fdb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71fdb-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="71fdb-120">Optional query parameters</span></span>
<span data-ttu-id="71fdb-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="71fdb-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71fdb-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71fdb-122">Request headers</span></span>
|<span data-ttu-id="71fdb-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="71fdb-123">Header</span></span>|<span data-ttu-id="71fdb-124">Valor</span><span class="sxs-lookup"><span data-stu-id="71fdb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71fdb-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="71fdb-125">Authorization</span></span>|<span data-ttu-id="71fdb-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71fdb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71fdb-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="71fdb-127">Accept</span></span>|<span data-ttu-id="71fdb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="71fdb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71fdb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71fdb-129">Request body</span></span>
<span data-ttu-id="71fdb-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="71fdb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71fdb-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="71fdb-131">Response</span></span>
<span data-ttu-id="71fdb-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71fdb-132">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71fdb-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71fdb-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="71fdb-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71fdb-134">Request</span></span>
<span data-ttu-id="71fdb-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71fdb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="71fdb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="71fdb-136">Response</span></span>
<span data-ttu-id="71fdb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71fdb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1459

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceOverview",
    "id": "42a91653-1653-42a9-5316-a9425316a942",
    "enrolledDeviceCount": 3,
    "mdmEnrolledCount": 0,
    "dualEnrolledDeviceCount": 7,
    "deviceOperatingSystemSummary": {
      "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
      "androidCount": 12,
      "iosCount": 8,
      "macOSCount": 10,
      "windowsMobileCount": 2,
      "windowsCount": 12,
      "unknownCount": 12,
      "androidDedicatedCount": 5,
      "androidDeviceAdminCount": 7,
      "androidFullyManagedCount": 8,
      "androidWorkProfileCount": 7,
      "androidCorporateWorkProfileCount": 0,
      "configMgrDeviceCount": 4,
      "aospUserlessCount": 1,
      "aospUserAssociatedCount": 7,
      "linuxCount": 10
    },
    "deviceExchangeAccessStateSummary": {
      "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
      "allowedDeviceCount": 2,
      "blockedDeviceCount": 2,
      "quarantinedDeviceCount": 6,
      "unknownDeviceCount": 2,
      "unavailableDeviceCount": 6
    },
    "managedDeviceModelsAndManufacturers": {
      "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
      "deviceModels": [
        "Device Models value"
      ],
      "deviceManufacturers": [
        "Device Manufacturers value"
      ]
    },
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```




