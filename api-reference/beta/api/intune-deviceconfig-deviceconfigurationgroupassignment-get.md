---
title: Obter deviceConfigurationGroupAssignment
description: Leia as propriedades e os relacionamentos do objeto deviceConfigurationGroupAssignment.
ms.openlocfilehash: ffde36d82bb22cac836bf7e74cc14fbba11e7b4e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039935"
---
# <a name="get-deviceconfigurationgroupassignment"></a><span data-ttu-id="2583f-103">Obter deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="2583f-103">Get deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="2583f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2583f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2583f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2583f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2583f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2583f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2583f-107">Leia as propriedades e os relacionamentos do objeto [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="2583f-107">Read properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2583f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2583f-108">Prerequisites</span></span>
<span data-ttu-id="2583f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2583f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2583f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2583f-111">Permission type</span></span>|<span data-ttu-id="2583f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2583f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2583f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2583f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2583f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2583f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2583f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2583f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2583f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2583f-116">Not supported.</span></span>|
|<span data-ttu-id="2583f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2583f-117">Application</span></span>|<span data-ttu-id="2583f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2583f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2583f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2583f-119">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2583f-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2583f-120">Optional query parameters</span></span>
<span data-ttu-id="2583f-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2583f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2583f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2583f-122">Request headers</span></span>
|<span data-ttu-id="2583f-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2583f-123">Header</span></span>|<span data-ttu-id="2583f-124">Valor</span><span class="sxs-lookup"><span data-stu-id="2583f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2583f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2583f-125">Authorization</span></span>|<span data-ttu-id="2583f-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2583f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2583f-127">Accept</span><span class="sxs-lookup"><span data-stu-id="2583f-127">Accept</span></span>|<span data-ttu-id="2583f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2583f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2583f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2583f-129">Request body</span></span>
<span data-ttu-id="2583f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2583f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2583f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2583f-131">Response</span></span>
<span data-ttu-id="2583f-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2583f-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2583f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2583f-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="2583f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2583f-134">Request</span></span>
<span data-ttu-id="2583f-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2583f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="2583f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2583f-136">Response</span></span>
<span data-ttu-id="2583f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2583f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





