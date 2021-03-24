---
title: Obter deviceConfigurationGroupAssignment
description: Leia propriedades e relações do objeto deviceConfigurationGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5e7ce74a4dc2f4757888d4b6624083752e6d3a41
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131579"
---
# <a name="get-deviceconfigurationgroupassignment"></a><span data-ttu-id="b9655-103">Obter deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="b9655-103">Get deviceConfigurationGroupAssignment</span></span>

<span data-ttu-id="b9655-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9655-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9655-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b9655-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9655-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9655-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9655-107">Leia propriedades e relações do [objeto deviceConfigurationGroupAssignment.](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b9655-107">Read properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9655-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b9655-108">Prerequisites</span></span>
<span data-ttu-id="b9655-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9655-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9655-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9655-111">Permission type</span></span>|<span data-ttu-id="b9655-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9655-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9655-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9655-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9655-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9655-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b9655-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9655-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9655-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9655-116">Not supported.</span></span>|
|<span data-ttu-id="b9655-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9655-117">Application</span></span>|<span data-ttu-id="b9655-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9655-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9655-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9655-119">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9655-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b9655-120">Optional query parameters</span></span>
<span data-ttu-id="b9655-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b9655-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9655-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9655-122">Request headers</span></span>
|<span data-ttu-id="b9655-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9655-123">Header</span></span>|<span data-ttu-id="b9655-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b9655-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9655-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9655-125">Authorization</span></span>|<span data-ttu-id="b9655-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9655-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9655-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b9655-127">Accept</span></span>|<span data-ttu-id="b9655-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b9655-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9655-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9655-129">Request body</span></span>
<span data-ttu-id="b9655-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9655-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9655-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9655-131">Response</span></span>
<span data-ttu-id="b9655-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9655-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9655-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9655-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9655-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9655-134">Request</span></span>
<span data-ttu-id="b9655-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9655-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="b9655-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9655-136">Response</span></span>
<span data-ttu-id="b9655-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9655-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




