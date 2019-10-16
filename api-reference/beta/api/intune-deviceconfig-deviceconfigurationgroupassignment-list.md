---
title: Listar deviceConfigurationGroupAssignments
description: Listar Propriedades e relações dos objetos deviceConfigurationGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b15c5a96e754e30df634df69905d4d8a1c53be95
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534054"
---
# <a name="list-deviceconfigurationgroupassignments"></a><span data-ttu-id="43766-103">Listar deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="43766-103">List deviceConfigurationGroupAssignments</span></span>

> <span data-ttu-id="43766-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="43766-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43766-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="43766-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43766-106">Listar Propriedades e relações dos objetos [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="43766-106">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43766-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="43766-107">Prerequisites</span></span>
<span data-ttu-id="43766-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43766-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43766-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43766-110">Permission type</span></span>|<span data-ttu-id="43766-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="43766-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43766-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43766-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43766-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="43766-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="43766-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43766-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43766-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43766-115">Not supported.</span></span>|
|<span data-ttu-id="43766-116">Application</span><span class="sxs-lookup"><span data-stu-id="43766-116">Application</span></span>|<span data-ttu-id="43766-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="43766-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43766-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43766-118">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="43766-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43766-119">Request headers</span></span>
|<span data-ttu-id="43766-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43766-120">Header</span></span>|<span data-ttu-id="43766-121">Valor</span><span class="sxs-lookup"><span data-stu-id="43766-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43766-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="43766-122">Authorization</span></span>|<span data-ttu-id="43766-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43766-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43766-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="43766-124">Accept</span></span>|<span data-ttu-id="43766-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43766-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43766-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43766-126">Request body</span></span>
<span data-ttu-id="43766-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="43766-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43766-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="43766-128">Response</span></span>
<span data-ttu-id="43766-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43766-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43766-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43766-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="43766-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43766-131">Request</span></span>
<span data-ttu-id="43766-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="43766-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="43766-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="43766-133">Response</span></span>
<span data-ttu-id="43766-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43766-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






