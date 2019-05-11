---
title: Acessar deviceConfigurationAssignment
description: Leia as propriedades e as relações do objeto deviceConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 61d206b2f9158261333ddd2dd58cf140340085c0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927437"
---
# <a name="get-deviceconfigurationassignment"></a><span data-ttu-id="dad8c-103">Acessar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="dad8c-103">Get deviceConfigurationAssignment</span></span>

> <span data-ttu-id="dad8c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dad8c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dad8c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dad8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dad8c-106">Leia as propriedades e as relações do objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dad8c-106">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dad8c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dad8c-107">Prerequisites</span></span>
<span data-ttu-id="dad8c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dad8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dad8c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dad8c-110">Permission type</span></span>|<span data-ttu-id="dad8c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dad8c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dad8c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dad8c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dad8c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dad8c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dad8c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dad8c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dad8c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dad8c-115">Not supported.</span></span>|
|<span data-ttu-id="dad8c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dad8c-116">Application</span></span>|<span data-ttu-id="dad8c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dad8c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dad8c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dad8c-118">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dad8c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dad8c-119">Optional query parameters</span></span>
<span data-ttu-id="dad8c-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dad8c-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dad8c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dad8c-121">Request headers</span></span>
|<span data-ttu-id="dad8c-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dad8c-122">Header</span></span>|<span data-ttu-id="dad8c-123">Valor</span><span class="sxs-lookup"><span data-stu-id="dad8c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dad8c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="dad8c-124">Authorization</span></span>|<span data-ttu-id="dad8c-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dad8c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dad8c-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dad8c-126">Accept</span></span>|<span data-ttu-id="dad8c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="dad8c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dad8c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dad8c-128">Request body</span></span>
<span data-ttu-id="dad8c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dad8c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dad8c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="dad8c-130">Response</span></span>
<span data-ttu-id="dad8c-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dad8c-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dad8c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dad8c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="dad8c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dad8c-133">Request</span></span>
<span data-ttu-id="dad8c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dad8c-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="dad8c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="dad8c-135">Response</span></span>
<span data-ttu-id="dad8c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dad8c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
    "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




