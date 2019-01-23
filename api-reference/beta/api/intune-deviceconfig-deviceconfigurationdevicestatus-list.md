---
title: Listar deviceConfigurationDeviceStatuses
description: Listar propriedades e relações dos objetos deviceConfigurationDeviceStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b470403c3e7581e353326a0557ea78f4feb63e25
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393862"
---
# <a name="list-deviceconfigurationdevicestatuses"></a><span data-ttu-id="b7197-103">Listar deviceConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="b7197-103">List deviceConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="b7197-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="b7197-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b7197-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b7197-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b7197-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="b7197-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7197-107">Listar propriedades e relações dos objetos [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b7197-107">List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7197-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b7197-108">Prerequisites</span></span>
<span data-ttu-id="b7197-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b7197-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b7197-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7197-111">Permission type</span></span>|<span data-ttu-id="b7197-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b7197-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7197-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7197-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b7197-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7197-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b7197-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7197-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7197-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7197-116">Not supported.</span></span>|
|<span data-ttu-id="b7197-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7197-117">Application</span></span>|<span data-ttu-id="b7197-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7197-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7197-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7197-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b7197-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7197-120">Request headers</span></span>
|<span data-ttu-id="b7197-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b7197-121">Header</span></span>|<span data-ttu-id="b7197-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b7197-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7197-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7197-123">Authorization</span></span>|<span data-ttu-id="b7197-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7197-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7197-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b7197-125">Accept</span></span>|<span data-ttu-id="b7197-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b7197-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7197-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7197-127">Request body</span></span>
<span data-ttu-id="b7197-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b7197-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7197-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7197-129">Response</span></span>
<span data-ttu-id="b7197-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7197-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7197-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7197-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7197-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7197-132">Request</span></span>
<span data-ttu-id="b7197-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7197-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="b7197-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7197-134">Response</span></span>
<span data-ttu-id="b7197-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7197-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




