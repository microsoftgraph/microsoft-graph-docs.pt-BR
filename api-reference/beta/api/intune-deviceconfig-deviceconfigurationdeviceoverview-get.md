---
title: Acessar deviceConfigurationDeviceOverview
description: Leia as propriedades e relações de objetos de deviceConfigurationDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b360794e51892ca58b4a6ad602724aac800404b6
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792965"
---
# <a name="get-deviceconfigurationdeviceoverview"></a><span data-ttu-id="64024-103">Acessar deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="64024-103">Get deviceConfigurationDeviceOverview</span></span>

<span data-ttu-id="64024-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64024-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64024-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="64024-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64024-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64024-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64024-107">Leia as propriedades e relações de objetos de [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="64024-107">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64024-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="64024-108">Prerequisites</span></span>
<span data-ttu-id="64024-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="64024-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="64024-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64024-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64024-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64024-111">Permission type</span></span>|<span data-ttu-id="64024-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="64024-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64024-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64024-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64024-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="64024-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="64024-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64024-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64024-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64024-116">Not supported.</span></span>|
|<span data-ttu-id="64024-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64024-117">Application</span></span>|<span data-ttu-id="64024-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="64024-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64024-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64024-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64024-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="64024-120">Optional query parameters</span></span>
<span data-ttu-id="64024-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="64024-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64024-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64024-122">Request headers</span></span>
|<span data-ttu-id="64024-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64024-123">Header</span></span>|<span data-ttu-id="64024-124">Valor</span><span class="sxs-lookup"><span data-stu-id="64024-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64024-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="64024-125">Authorization</span></span>|<span data-ttu-id="64024-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64024-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64024-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="64024-127">Accept</span></span>|<span data-ttu-id="64024-128">application/json</span><span class="sxs-lookup"><span data-stu-id="64024-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64024-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64024-129">Request body</span></span>
<span data-ttu-id="64024-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64024-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64024-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="64024-131">Response</span></span>
<span data-ttu-id="64024-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64024-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64024-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64024-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="64024-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64024-134">Request</span></span>
<span data-ttu-id="64024-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64024-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

### <a name="response"></a><span data-ttu-id="64024-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="64024-136">Response</span></span>
<span data-ttu-id="64024-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="64024-137">Here is an example of the response.</span></span> <span data-ttu-id="64024-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="64024-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="64024-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="64024-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 435

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
    "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "notApplicablePlatformCount": 10,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```



