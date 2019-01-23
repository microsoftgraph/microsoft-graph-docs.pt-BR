---
title: Get settingStateDeviceSummary
description: Ler propriedades e relações do objeto settingStateDeviceSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ab2d1b1d23b740290105d67fc591d20ceaa6b322
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423010"
---
# <a name="get-settingstatedevicesummary"></a><span data-ttu-id="a196d-103">Get settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="a196d-103">Get settingStateDeviceSummary</span></span>

> <span data-ttu-id="a196d-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="a196d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a196d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a196d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a196d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="a196d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a196d-107">Ler propriedades e relações do objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a196d-107">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a196d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a196d-108">Prerequisites</span></span>
<span data-ttu-id="a196d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a196d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a196d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a196d-111">Permission type</span></span>|<span data-ttu-id="a196d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a196d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a196d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a196d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a196d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a196d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a196d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a196d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a196d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a196d-116">Not supported.</span></span>|
|<span data-ttu-id="a196d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a196d-117">Application</span></span>|<span data-ttu-id="a196d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a196d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a196d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a196d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a196d-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a196d-120">Optional query parameters</span></span>
<span data-ttu-id="a196d-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a196d-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a196d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a196d-122">Request headers</span></span>
|<span data-ttu-id="a196d-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a196d-123">Header</span></span>|<span data-ttu-id="a196d-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a196d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a196d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a196d-125">Authorization</span></span>|<span data-ttu-id="a196d-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a196d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a196d-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a196d-127">Accept</span></span>|<span data-ttu-id="a196d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a196d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a196d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a196d-129">Request body</span></span>
<span data-ttu-id="a196d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a196d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a196d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a196d-131">Response</span></span>
<span data-ttu-id="a196d-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a196d-132">If successful, this method returns a `200 OK` response code and [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a196d-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a196d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a196d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a196d-134">Request</span></span>
<span data-ttu-id="a196d-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a196d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

### <a name="response"></a><span data-ttu-id="a196d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a196d-136">Response</span></span>
<span data-ttu-id="a196d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a196d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": {
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
}
```




