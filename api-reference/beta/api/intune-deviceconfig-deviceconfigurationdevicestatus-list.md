---
title: Listar deviceConfigurationDeviceStatuses
description: Listar propriedades e relações dos objetos deviceConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 67e425d908c49898c9ea2ce6056f0adf9e999fad
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792930"
---
# <a name="list-deviceconfigurationdevicestatuses"></a><span data-ttu-id="99073-103">Listar deviceConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="99073-103">List deviceConfigurationDeviceStatuses</span></span>

<span data-ttu-id="99073-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99073-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99073-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="99073-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99073-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99073-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99073-107">Listar propriedades e relações dos objetos [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="99073-107">List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99073-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="99073-108">Prerequisites</span></span>
<span data-ttu-id="99073-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="99073-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="99073-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99073-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99073-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99073-111">Permission type</span></span>|<span data-ttu-id="99073-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="99073-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99073-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99073-113">Delegated (work or school account)</span></span>|<span data-ttu-id="99073-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="99073-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="99073-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99073-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99073-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99073-116">Not supported.</span></span>|
|<span data-ttu-id="99073-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99073-117">Application</span></span>|<span data-ttu-id="99073-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="99073-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99073-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99073-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="99073-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99073-120">Request headers</span></span>
|<span data-ttu-id="99073-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="99073-121">Header</span></span>|<span data-ttu-id="99073-122">Valor</span><span class="sxs-lookup"><span data-stu-id="99073-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99073-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="99073-123">Authorization</span></span>|<span data-ttu-id="99073-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99073-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99073-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="99073-125">Accept</span></span>|<span data-ttu-id="99073-126">application/json</span><span class="sxs-lookup"><span data-stu-id="99073-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99073-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99073-127">Request body</span></span>
<span data-ttu-id="99073-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="99073-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99073-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="99073-129">Response</span></span>
<span data-ttu-id="99073-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99073-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99073-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99073-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="99073-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99073-132">Request</span></span>
<span data-ttu-id="99073-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99073-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="99073-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="99073-134">Response</span></span>
<span data-ttu-id="99073-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="99073-135">Here is an example of the response.</span></span> <span data-ttu-id="99073-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="99073-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="99073-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="99073-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 569

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
      "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "platform": 8,
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



