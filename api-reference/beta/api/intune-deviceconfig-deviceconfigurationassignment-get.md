---
title: Acessar deviceConfigurationAssignment
description: Leia as propriedades e as relações do objeto deviceConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 843921627051961058b6c5788633e5a05fd71da8
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123173"
---
# <a name="get-deviceconfigurationassignment"></a><span data-ttu-id="22a54-103">Acessar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="22a54-103">Get deviceConfigurationAssignment</span></span>

<span data-ttu-id="22a54-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22a54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22a54-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="22a54-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22a54-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22a54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22a54-107">Leia as propriedades e as relações do objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="22a54-107">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22a54-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22a54-108">Prerequisites</span></span>
<span data-ttu-id="22a54-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="22a54-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="22a54-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22a54-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22a54-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22a54-111">Permission type</span></span>|<span data-ttu-id="22a54-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22a54-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22a54-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22a54-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22a54-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22a54-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="22a54-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22a54-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22a54-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22a54-116">Not supported.</span></span>|
|<span data-ttu-id="22a54-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22a54-117">Application</span></span>|<span data-ttu-id="22a54-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22a54-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22a54-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22a54-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22a54-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="22a54-120">Optional query parameters</span></span>
<span data-ttu-id="22a54-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="22a54-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22a54-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22a54-122">Request headers</span></span>
|<span data-ttu-id="22a54-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22a54-123">Header</span></span>|<span data-ttu-id="22a54-124">Valor</span><span class="sxs-lookup"><span data-stu-id="22a54-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22a54-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="22a54-125">Authorization</span></span>|<span data-ttu-id="22a54-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22a54-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22a54-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22a54-127">Accept</span></span>|<span data-ttu-id="22a54-128">application/json</span><span class="sxs-lookup"><span data-stu-id="22a54-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22a54-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22a54-129">Request body</span></span>
<span data-ttu-id="22a54-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22a54-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22a54-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="22a54-131">Response</span></span>
<span data-ttu-id="22a54-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22a54-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22a54-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22a54-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="22a54-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22a54-134">Request</span></span>
<span data-ttu-id="22a54-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22a54-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="22a54-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="22a54-136">Response</span></span>
<span data-ttu-id="22a54-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="22a54-137">Here is an example of the response.</span></span> <span data-ttu-id="22a54-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="22a54-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="22a54-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="22a54-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
    "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
    "target": {
      "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include"
    },
    "source": "policySets",
    "sourceId": "Source Id value"
  }
}
```



