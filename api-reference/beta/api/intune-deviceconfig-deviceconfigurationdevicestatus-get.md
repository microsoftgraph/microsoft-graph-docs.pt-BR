---
title: Acessar deviceConfigurationDeviceStatus
description: Leia as propriedades e as relações do objeto deviceConfigurationDeviceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4fa88b07cbc5e21dc2107242cffdc1353349d74c
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38084479"
---
# <a name="get-deviceconfigurationdevicestatus"></a><span data-ttu-id="17b1d-103">Acessar deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="17b1d-103">Get deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="17b1d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="17b1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17b1d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="17b1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17b1d-106">Leia as propriedades e as relações do objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="17b1d-106">Read properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17b1d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="17b1d-107">Prerequisites</span></span>
<span data-ttu-id="17b1d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17b1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17b1d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17b1d-110">Permission type</span></span>|<span data-ttu-id="17b1d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="17b1d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17b1d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17b1d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17b1d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="17b1d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="17b1d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17b1d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17b1d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17b1d-115">Not supported.</span></span>|
|<span data-ttu-id="17b1d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17b1d-116">Application</span></span>|<span data-ttu-id="17b1d-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="17b1d-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17b1d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17b1d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="17b1d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="17b1d-119">Optional query parameters</span></span>
<span data-ttu-id="17b1d-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="17b1d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="17b1d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17b1d-121">Request headers</span></span>
|<span data-ttu-id="17b1d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17b1d-122">Header</span></span>|<span data-ttu-id="17b1d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="17b1d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17b1d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="17b1d-124">Authorization</span></span>|<span data-ttu-id="17b1d-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17b1d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17b1d-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="17b1d-126">Accept</span></span>|<span data-ttu-id="17b1d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="17b1d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17b1d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17b1d-128">Request body</span></span>
<span data-ttu-id="17b1d-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="17b1d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17b1d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="17b1d-130">Response</span></span>
<span data-ttu-id="17b1d-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17b1d-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17b1d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17b1d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="17b1d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17b1d-133">Request</span></span>
<span data-ttu-id="17b1d-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17b1d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="17b1d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="17b1d-135">Response</span></span>
<span data-ttu-id="17b1d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17b1d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 535

{
  "value": {
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
}
```






