---
title: Obter deviceConfigurationGroupAssignment
description: Leia as propriedades e as relações do objeto deviceConfigurationGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d4e70662ec60bd200e3a74c12e140a2fc6521144
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792902"
---
# <a name="get-deviceconfigurationgroupassignment"></a><span data-ttu-id="87d1f-103">Obter deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="87d1f-103">Get deviceConfigurationGroupAssignment</span></span>

<span data-ttu-id="87d1f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87d1f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87d1f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="87d1f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87d1f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="87d1f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87d1f-107">Leia as propriedades e as relações do objeto [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="87d1f-107">Read properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87d1f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="87d1f-108">Prerequisites</span></span>
<span data-ttu-id="87d1f-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="87d1f-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="87d1f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87d1f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87d1f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87d1f-111">Permission type</span></span>|<span data-ttu-id="87d1f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="87d1f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87d1f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87d1f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87d1f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="87d1f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="87d1f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87d1f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87d1f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87d1f-116">Not supported.</span></span>|
|<span data-ttu-id="87d1f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87d1f-117">Application</span></span>|<span data-ttu-id="87d1f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="87d1f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87d1f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87d1f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87d1f-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="87d1f-120">Optional query parameters</span></span>
<span data-ttu-id="87d1f-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="87d1f-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87d1f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87d1f-122">Request headers</span></span>
|<span data-ttu-id="87d1f-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87d1f-123">Header</span></span>|<span data-ttu-id="87d1f-124">Valor</span><span class="sxs-lookup"><span data-stu-id="87d1f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87d1f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="87d1f-125">Authorization</span></span>|<span data-ttu-id="87d1f-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87d1f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87d1f-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="87d1f-127">Accept</span></span>|<span data-ttu-id="87d1f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="87d1f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87d1f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87d1f-129">Request body</span></span>
<span data-ttu-id="87d1f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87d1f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87d1f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="87d1f-131">Response</span></span>
<span data-ttu-id="87d1f-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87d1f-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87d1f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87d1f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="87d1f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87d1f-134">Request</span></span>
<span data-ttu-id="87d1f-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87d1f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="87d1f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="87d1f-136">Response</span></span>
<span data-ttu-id="87d1f-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="87d1f-137">Here is an example of the response.</span></span> <span data-ttu-id="87d1f-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="87d1f-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="87d1f-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="87d1f-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 222

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
    "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
    "targetGroupId": "Target Group Id value",
    "excludeGroup": true
  }
}
```



