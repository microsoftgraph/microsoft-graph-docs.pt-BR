---
title: Listar settingStateDeviceSummaries
description: Listar propriedades e relações dos objetos settingStateDeviceSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 470da5c14bd2648cb9d94bac2a1daed4984d0939
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127876"
---
# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="307bc-103">Listar settingStateDeviceSummaries</span><span class="sxs-lookup"><span data-stu-id="307bc-103">List settingStateDeviceSummaries</span></span>

<span data-ttu-id="307bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="307bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="307bc-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="307bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="307bc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="307bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="307bc-107">Listar propriedades e relações dos objetos [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="307bc-107">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="307bc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="307bc-108">Prerequisites</span></span>
<span data-ttu-id="307bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="307bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="307bc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="307bc-111">Permission type</span></span>|<span data-ttu-id="307bc-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="307bc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="307bc-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="307bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="307bc-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="307bc-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="307bc-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="307bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="307bc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="307bc-116">Not supported.</span></span>|
|<span data-ttu-id="307bc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="307bc-117">Application</span></span>|<span data-ttu-id="307bc-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="307bc-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="307bc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="307bc-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="307bc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="307bc-120">Request headers</span></span>
|<span data-ttu-id="307bc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="307bc-121">Header</span></span>|<span data-ttu-id="307bc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="307bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="307bc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="307bc-123">Authorization</span></span>|<span data-ttu-id="307bc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="307bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="307bc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="307bc-125">Accept</span></span>|<span data-ttu-id="307bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="307bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="307bc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="307bc-127">Request body</span></span>
<span data-ttu-id="307bc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="307bc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="307bc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="307bc-129">Response</span></span>
<span data-ttu-id="307bc-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="307bc-130">If successful, this method returns a `200 OK` response code and a collection of [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="307bc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="307bc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="307bc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="307bc-132">Request</span></span>
<span data-ttu-id="307bc-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="307bc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="307bc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="307bc-134">Response</span></span>
<span data-ttu-id="307bc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="307bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




