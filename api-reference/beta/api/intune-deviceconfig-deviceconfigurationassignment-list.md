---
title: Listar deviceConfigurationAssignments
description: Listar propriedades e relações dos objetos deviceConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3d3bd3f098e7e0c6d99ab7b1475aa0145c2ae023
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534138"
---
# <a name="list-deviceconfigurationassignments"></a><span data-ttu-id="845ba-103">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="845ba-103">List deviceConfigurationAssignments</span></span>

> <span data-ttu-id="845ba-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="845ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="845ba-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="845ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="845ba-106">Listar propriedades e relações dos objetos [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="845ba-106">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="845ba-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="845ba-107">Prerequisites</span></span>
<span data-ttu-id="845ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="845ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="845ba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="845ba-110">Permission type</span></span>|<span data-ttu-id="845ba-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="845ba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="845ba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="845ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="845ba-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="845ba-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="845ba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="845ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="845ba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="845ba-115">Not supported.</span></span>|
|<span data-ttu-id="845ba-116">Application</span><span class="sxs-lookup"><span data-stu-id="845ba-116">Application</span></span>|<span data-ttu-id="845ba-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="845ba-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="845ba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="845ba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="845ba-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="845ba-119">Request headers</span></span>
|<span data-ttu-id="845ba-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="845ba-120">Header</span></span>|<span data-ttu-id="845ba-121">Valor</span><span class="sxs-lookup"><span data-stu-id="845ba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="845ba-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="845ba-122">Authorization</span></span>|<span data-ttu-id="845ba-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="845ba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="845ba-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="845ba-124">Accept</span></span>|<span data-ttu-id="845ba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="845ba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="845ba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="845ba-126">Request body</span></span>
<span data-ttu-id="845ba-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="845ba-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="845ba-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="845ba-128">Response</span></span>
<span data-ttu-id="845ba-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="845ba-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="845ba-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="845ba-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="845ba-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="845ba-131">Request</span></span>
<span data-ttu-id="845ba-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="845ba-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="845ba-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="845ba-133">Response</span></span>
<span data-ttu-id="845ba-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="845ba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 340

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```






