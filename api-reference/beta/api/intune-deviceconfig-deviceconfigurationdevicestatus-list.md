---
title: Listar deviceConfigurationDeviceStatuses
description: Listar propriedades e relações dos objetos deviceConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ae6a052ce4bd296353ecfc6713958a7e1747409e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943841"
---
# <a name="list-deviceconfigurationdevicestatuses"></a><span data-ttu-id="493a4-103">Listar deviceConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="493a4-103">List deviceConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="493a4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="493a4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="493a4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="493a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="493a4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="493a4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="493a4-107">Listar propriedades e relações dos objetos [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="493a4-107">List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="493a4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="493a4-108">Prerequisites</span></span>
<span data-ttu-id="493a4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="493a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="493a4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="493a4-111">Permission type</span></span>|<span data-ttu-id="493a4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="493a4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="493a4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="493a4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="493a4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="493a4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="493a4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="493a4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="493a4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="493a4-116">Not supported.</span></span>|
|<span data-ttu-id="493a4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="493a4-117">Application</span></span>|<span data-ttu-id="493a4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="493a4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="493a4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="493a4-119">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="493a4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="493a4-120">Request headers</span></span>
|<span data-ttu-id="493a4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="493a4-121">Header</span></span>|<span data-ttu-id="493a4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="493a4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="493a4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="493a4-123">Authorization</span></span>|<span data-ttu-id="493a4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="493a4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="493a4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="493a4-125">Accept</span></span>|<span data-ttu-id="493a4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="493a4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="493a4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="493a4-127">Request body</span></span>
<span data-ttu-id="493a4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="493a4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="493a4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="493a4-129">Response</span></span>
<span data-ttu-id="493a4-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="493a4-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="493a4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="493a4-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="493a4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="493a4-132">Request</span></span>
<span data-ttu-id="493a4-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="493a4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="493a4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="493a4-134">Response</span></span>
<span data-ttu-id="493a4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="493a4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





