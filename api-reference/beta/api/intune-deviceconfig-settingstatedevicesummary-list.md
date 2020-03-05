---
title: Listar settingStateDeviceSummaries
description: Listar propriedades e relações dos objetos settingStateDeviceSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2ae6b9d01384d806db1bbeaad6c0ebd3942eb217
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42483431"
---
# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="14e4d-103">Listar settingStateDeviceSummaries</span><span class="sxs-lookup"><span data-stu-id="14e4d-103">List settingStateDeviceSummaries</span></span>

<span data-ttu-id="14e4d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="14e4d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14e4d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="14e4d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14e4d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14e4d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14e4d-107">Listar propriedades e relações dos objetos [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="14e4d-107">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14e4d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="14e4d-108">Prerequisites</span></span>
<span data-ttu-id="14e4d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14e4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14e4d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14e4d-111">Permission type</span></span>|<span data-ttu-id="14e4d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="14e4d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14e4d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14e4d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14e4d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="14e4d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="14e4d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14e4d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14e4d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14e4d-116">Not supported.</span></span>|
|<span data-ttu-id="14e4d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14e4d-117">Application</span></span>|<span data-ttu-id="14e4d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="14e4d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14e4d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14e4d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="14e4d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14e4d-120">Request headers</span></span>
|<span data-ttu-id="14e4d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14e4d-121">Header</span></span>|<span data-ttu-id="14e4d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="14e4d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14e4d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="14e4d-123">Authorization</span></span>|<span data-ttu-id="14e4d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14e4d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14e4d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="14e4d-125">Accept</span></span>|<span data-ttu-id="14e4d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14e4d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14e4d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14e4d-127">Request body</span></span>
<span data-ttu-id="14e4d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="14e4d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14e4d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="14e4d-129">Response</span></span>
<span data-ttu-id="14e4d-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14e4d-130">If successful, this method returns a `200 OK` response code and a collection of [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14e4d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14e4d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="14e4d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14e4d-132">Request</span></span>
<span data-ttu-id="14e4d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14e4d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="14e4d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="14e4d-134">Response</span></span>
<span data-ttu-id="14e4d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14e4d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 486

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
      "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
      "settingName": "Setting Name value",
      "instancePath": "Instance Path value",
      "unknownDeviceCount": 2,
      "notApplicableDeviceCount": 8,
      "compliantDeviceCount": 4,
      "remediatedDeviceCount": 5,
      "nonCompliantDeviceCount": 7,
      "errorDeviceCount": 0,
      "conflictDeviceCount": 3
    }
  ]
}
```





