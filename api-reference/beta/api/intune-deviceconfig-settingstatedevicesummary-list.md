---
title: Listar settingStateDeviceSummaries
description: Listar propriedades e relações dos objetos settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 665bbb36b475e5542d8d8e7a2cece7b932bb9d02
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518573"
---
# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="e7043-103">Listar settingStateDeviceSummaries</span><span class="sxs-lookup"><span data-stu-id="e7043-103">List settingStateDeviceSummaries</span></span>

> <span data-ttu-id="e7043-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e7043-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7043-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e7043-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7043-106">Listar propriedades e relações dos objetos [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e7043-106">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7043-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7043-107">Prerequisites</span></span>
<span data-ttu-id="e7043-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7043-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7043-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7043-110">Permission type</span></span>|<span data-ttu-id="e7043-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e7043-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7043-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7043-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7043-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7043-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e7043-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7043-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7043-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7043-115">Not supported.</span></span>|
|<span data-ttu-id="e7043-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7043-116">Application</span></span>|<span data-ttu-id="e7043-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7043-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7043-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7043-118">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="e7043-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7043-119">Request headers</span></span>
|<span data-ttu-id="e7043-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7043-120">Header</span></span>|<span data-ttu-id="e7043-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e7043-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7043-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7043-122">Authorization</span></span>|<span data-ttu-id="e7043-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7043-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7043-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e7043-124">Accept</span></span>|<span data-ttu-id="e7043-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7043-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7043-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7043-126">Request body</span></span>
<span data-ttu-id="e7043-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7043-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7043-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7043-128">Response</span></span>
<span data-ttu-id="e7043-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7043-129">If successful, this method returns a `200 OK` response code and a collection of [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7043-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7043-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7043-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7043-131">Request</span></span>
<span data-ttu-id="e7043-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7043-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="e7043-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7043-133">Response</span></span>
<span data-ttu-id="e7043-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7043-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





