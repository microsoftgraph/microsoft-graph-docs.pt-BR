---
title: Acessar deviceConfigurationAssignment
description: Leia as propriedades e as relações do objeto deviceConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9fbff0cd39189477cbef988ff526ff28fc7395b4
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38084535"
---
# <a name="get-deviceconfigurationassignment"></a><span data-ttu-id="47c19-103">Acessar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="47c19-103">Get deviceConfigurationAssignment</span></span>

> <span data-ttu-id="47c19-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="47c19-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47c19-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="47c19-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47c19-106">Leia as propriedades e as relações do objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="47c19-106">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47c19-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="47c19-107">Prerequisites</span></span>
<span data-ttu-id="47c19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47c19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47c19-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47c19-110">Permission type</span></span>|<span data-ttu-id="47c19-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="47c19-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47c19-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47c19-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47c19-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="47c19-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="47c19-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47c19-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47c19-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47c19-115">Not supported.</span></span>|
|<span data-ttu-id="47c19-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47c19-116">Application</span></span>|<span data-ttu-id="47c19-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="47c19-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47c19-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47c19-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="47c19-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="47c19-119">Optional query parameters</span></span>
<span data-ttu-id="47c19-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="47c19-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="47c19-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47c19-121">Request headers</span></span>
|<span data-ttu-id="47c19-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="47c19-122">Header</span></span>|<span data-ttu-id="47c19-123">Valor</span><span class="sxs-lookup"><span data-stu-id="47c19-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47c19-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="47c19-124">Authorization</span></span>|<span data-ttu-id="47c19-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47c19-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47c19-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="47c19-126">Accept</span></span>|<span data-ttu-id="47c19-127">application/json</span><span class="sxs-lookup"><span data-stu-id="47c19-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47c19-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47c19-128">Request body</span></span>
<span data-ttu-id="47c19-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47c19-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47c19-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="47c19-130">Response</span></span>
<span data-ttu-id="47c19-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47c19-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47c19-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47c19-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="47c19-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47c19-133">Request</span></span>
<span data-ttu-id="47c19-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47c19-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="47c19-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="47c19-135">Response</span></span>
<span data-ttu-id="47c19-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47c19-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 312

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
    "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    },
    "source": "policySets",
    "sourceId": "Source Id value"
  }
}
```






