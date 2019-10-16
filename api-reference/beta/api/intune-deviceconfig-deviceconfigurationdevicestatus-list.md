---
title: Listar deviceConfigurationDeviceStatuses
description: Listar propriedades e relações dos objetos deviceConfigurationDeviceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7b1974fc8278fd7f94508e85e722e152233003c4
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534089"
---
# <a name="list-deviceconfigurationdevicestatuses"></a><span data-ttu-id="4f26a-103">Listar deviceConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="4f26a-103">List deviceConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="4f26a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4f26a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f26a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f26a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f26a-106">Listar propriedades e relações dos objetos [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="4f26a-106">List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f26a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4f26a-107">Prerequisites</span></span>
<span data-ttu-id="4f26a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f26a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f26a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f26a-110">Permission type</span></span>|<span data-ttu-id="4f26a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4f26a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f26a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f26a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f26a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f26a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4f26a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f26a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f26a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f26a-115">Not supported.</span></span>|
|<span data-ttu-id="4f26a-116">Application</span><span class="sxs-lookup"><span data-stu-id="4f26a-116">Application</span></span>|<span data-ttu-id="4f26a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f26a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f26a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f26a-118">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="4f26a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f26a-119">Request headers</span></span>
|<span data-ttu-id="4f26a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f26a-120">Header</span></span>|<span data-ttu-id="4f26a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4f26a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f26a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f26a-122">Authorization</span></span>|<span data-ttu-id="4f26a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f26a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f26a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4f26a-124">Accept</span></span>|<span data-ttu-id="4f26a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4f26a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f26a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f26a-126">Request body</span></span>
<span data-ttu-id="4f26a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f26a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f26a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f26a-128">Response</span></span>
<span data-ttu-id="4f26a-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f26a-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f26a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f26a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f26a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f26a-131">Request</span></span>
<span data-ttu-id="4f26a-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f26a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="4f26a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f26a-133">Response</span></span>
<span data-ttu-id="4f26a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f26a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






