---
title: Listar settingStateDeviceSummaries
description: Listar propriedades e relações dos objetos settingStateDeviceSummary.
ms.openlocfilehash: 67439546e66b863ea4a0fbc91dbbab76ef2d66c7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033801"
---
# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="e1860-103">Listar settingStateDeviceSummaries</span><span class="sxs-lookup"><span data-stu-id="e1860-103">List settingStateDeviceSummaries</span></span>

> <span data-ttu-id="e1860-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e1860-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1860-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e1860-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1860-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e1860-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1860-107">Listar propriedades e relações dos objetos [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e1860-107">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1860-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1860-108">Prerequisites</span></span>
<span data-ttu-id="e1860-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1860-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1860-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1860-111">Permission type</span></span>|<span data-ttu-id="e1860-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1860-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1860-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1860-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1860-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1860-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e1860-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1860-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1860-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1860-116">Not supported.</span></span>|
|<span data-ttu-id="e1860-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1860-117">Application</span></span>|<span data-ttu-id="e1860-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1860-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1860-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1860-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e1860-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1860-120">Request headers</span></span>
|<span data-ttu-id="e1860-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1860-121">Header</span></span>|<span data-ttu-id="e1860-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e1860-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1860-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1860-123">Authorization</span></span>|<span data-ttu-id="e1860-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1860-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1860-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e1860-125">Accept</span></span>|<span data-ttu-id="e1860-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1860-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1860-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1860-127">Request body</span></span>
<span data-ttu-id="e1860-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1860-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1860-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1860-129">Response</span></span>
<span data-ttu-id="e1860-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1860-130">If successful, this method returns a `200 OK` response code and a collection of [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1860-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1860-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1860-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1860-132">Request</span></span>
<span data-ttu-id="e1860-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1860-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="e1860-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1860-134">Response</span></span>
<span data-ttu-id="e1860-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1860-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





