---
title: Acessar deviceConfigurationDeviceStatus
description: Leia as propriedades e as relações do objeto deviceConfigurationDeviceStatus.
ms.openlocfilehash: 78862a9b0aff5f256d59fb03e0cf86447459ce1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033886"
---
# <a name="get-deviceconfigurationdevicestatus"></a><span data-ttu-id="77578-103">Acessar deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="77578-103">Get deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="77578-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="77578-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77578-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="77578-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77578-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="77578-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77578-107">Leia as propriedades e as relações do objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="77578-107">Read properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="77578-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="77578-108">Prerequisites</span></span>
<span data-ttu-id="77578-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77578-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77578-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77578-111">Permission type</span></span>|<span data-ttu-id="77578-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="77578-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77578-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77578-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77578-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="77578-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="77578-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77578-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77578-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77578-116">Not supported.</span></span>|
|<span data-ttu-id="77578-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77578-117">Application</span></span>|<span data-ttu-id="77578-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77578-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77578-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77578-119">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77578-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="77578-120">Optional query parameters</span></span>
<span data-ttu-id="77578-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="77578-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="77578-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77578-122">Request headers</span></span>
|<span data-ttu-id="77578-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="77578-123">Header</span></span>|<span data-ttu-id="77578-124">Valor</span><span class="sxs-lookup"><span data-stu-id="77578-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77578-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="77578-125">Authorization</span></span>|<span data-ttu-id="77578-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77578-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77578-127">Accept</span><span class="sxs-lookup"><span data-stu-id="77578-127">Accept</span></span>|<span data-ttu-id="77578-128">application/json</span><span class="sxs-lookup"><span data-stu-id="77578-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77578-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77578-129">Request body</span></span>
<span data-ttu-id="77578-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="77578-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77578-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="77578-131">Response</span></span>
<span data-ttu-id="77578-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77578-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77578-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77578-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="77578-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77578-134">Request</span></span>
<span data-ttu-id="77578-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77578-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="77578-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="77578-136">Response</span></span>
<span data-ttu-id="77578-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77578-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





