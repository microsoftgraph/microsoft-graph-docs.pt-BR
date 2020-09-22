---
title: Listar deviceConfigurationGroupAssignments
description: Listar Propriedades e relações dos objetos deviceConfigurationGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a537ba6d75afae54e1e5fe9de4a04711013cda6a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032380"
---
# <a name="list-deviceconfigurationgroupassignments"></a><span data-ttu-id="d9206-103">Listar deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="d9206-103">List deviceConfigurationGroupAssignments</span></span>

<span data-ttu-id="d9206-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9206-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9206-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9206-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9206-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9206-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9206-107">Listar Propriedades e relações dos objetos [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="d9206-107">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9206-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d9206-108">Prerequisites</span></span>
<span data-ttu-id="d9206-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9206-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9206-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9206-111">Permission type</span></span>|<span data-ttu-id="d9206-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d9206-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9206-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9206-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9206-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9206-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d9206-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9206-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9206-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9206-116">Not supported.</span></span>|
|<span data-ttu-id="d9206-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9206-117">Application</span></span>|<span data-ttu-id="d9206-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9206-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9206-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9206-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="d9206-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9206-120">Request headers</span></span>
|<span data-ttu-id="d9206-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9206-121">Header</span></span>|<span data-ttu-id="d9206-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d9206-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9206-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9206-123">Authorization</span></span>|<span data-ttu-id="d9206-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9206-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9206-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d9206-125">Accept</span></span>|<span data-ttu-id="d9206-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9206-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9206-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9206-127">Request body</span></span>
<span data-ttu-id="d9206-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9206-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9206-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9206-129">Response</span></span>
<span data-ttu-id="d9206-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9206-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9206-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9206-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9206-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9206-132">Request</span></span>
<span data-ttu-id="d9206-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9206-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="d9206-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9206-134">Response</span></span>
<span data-ttu-id="d9206-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9206-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 244

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
      "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
      "targetGroupId": "Target Group Id value",
      "excludeGroup": true
    }
  ]
}
```






