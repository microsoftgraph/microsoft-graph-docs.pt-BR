---
title: Acessar deviceConfigurationDeviceOverview
description: Leia as propriedades e relações de objetos de deviceConfigurationDeviceOverview.
author: tfitzmac
ms.openlocfilehash: 2087a92100e69992b3028b7ede45e1c5a64cef82
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312604"
---
# <a name="get-deviceconfigurationdeviceoverview"></a><span data-ttu-id="195e8-103">Acessar deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="195e8-103">Get deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="195e8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="195e8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="195e8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="195e8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="195e8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="195e8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="195e8-107">Leia as propriedades e relações de objetos de [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="195e8-107">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="195e8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="195e8-108">Prerequisites</span></span>
<span data-ttu-id="195e8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="195e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="195e8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="195e8-111">Permission type</span></span>|<span data-ttu-id="195e8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="195e8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="195e8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="195e8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="195e8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="195e8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="195e8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="195e8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="195e8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="195e8-116">Not supported.</span></span>|
|<span data-ttu-id="195e8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="195e8-117">Application</span></span>|<span data-ttu-id="195e8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="195e8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="195e8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="195e8-119">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="195e8-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="195e8-120">Optional query parameters</span></span>
<span data-ttu-id="195e8-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="195e8-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="195e8-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="195e8-122">Request headers</span></span>
|<span data-ttu-id="195e8-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="195e8-123">Header</span></span>|<span data-ttu-id="195e8-124">Valor</span><span class="sxs-lookup"><span data-stu-id="195e8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="195e8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="195e8-125">Authorization</span></span>|<span data-ttu-id="195e8-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="195e8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="195e8-127">Accept</span><span class="sxs-lookup"><span data-stu-id="195e8-127">Accept</span></span>|<span data-ttu-id="195e8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="195e8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="195e8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="195e8-129">Request body</span></span>
<span data-ttu-id="195e8-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="195e8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="195e8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="195e8-131">Response</span></span>
<span data-ttu-id="195e8-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="195e8-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="195e8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="195e8-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="195e8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="195e8-134">Request</span></span>
<span data-ttu-id="195e8-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="195e8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

### <a name="response"></a><span data-ttu-id="195e8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="195e8-136">Response</span></span>
<span data-ttu-id="195e8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="195e8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





