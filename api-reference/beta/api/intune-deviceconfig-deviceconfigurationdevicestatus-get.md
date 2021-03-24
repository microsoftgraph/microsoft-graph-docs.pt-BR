---
title: Acessar deviceConfigurationDeviceStatus
description: Leia as propriedades e as relações do objeto deviceConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1bd9683c708e99d7a58d1f59a9184809bccecdfa
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131628"
---
# <a name="get-deviceconfigurationdevicestatus"></a><span data-ttu-id="823a1-103">Acessar deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="823a1-103">Get deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="823a1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="823a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="823a1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="823a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="823a1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="823a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="823a1-107">Leia as propriedades e as relações do objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="823a1-107">Read properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="823a1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="823a1-108">Prerequisites</span></span>
<span data-ttu-id="823a1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="823a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="823a1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="823a1-111">Permission type</span></span>|<span data-ttu-id="823a1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="823a1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="823a1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="823a1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="823a1-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="823a1-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="823a1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="823a1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="823a1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="823a1-116">Not supported.</span></span>|
|<span data-ttu-id="823a1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="823a1-117">Application</span></span>|<span data-ttu-id="823a1-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="823a1-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="823a1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="823a1-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="823a1-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="823a1-120">Optional query parameters</span></span>
<span data-ttu-id="823a1-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="823a1-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="823a1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="823a1-122">Request headers</span></span>
|<span data-ttu-id="823a1-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="823a1-123">Header</span></span>|<span data-ttu-id="823a1-124">Valor</span><span class="sxs-lookup"><span data-stu-id="823a1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="823a1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="823a1-125">Authorization</span></span>|<span data-ttu-id="823a1-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="823a1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="823a1-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="823a1-127">Accept</span></span>|<span data-ttu-id="823a1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="823a1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="823a1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="823a1-129">Request body</span></span>
<span data-ttu-id="823a1-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="823a1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="823a1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="823a1-131">Response</span></span>
<span data-ttu-id="823a1-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="823a1-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="823a1-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="823a1-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="823a1-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="823a1-134">Request</span></span>
<span data-ttu-id="823a1-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="823a1-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="823a1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="823a1-136">Response</span></span>
<span data-ttu-id="823a1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="823a1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




