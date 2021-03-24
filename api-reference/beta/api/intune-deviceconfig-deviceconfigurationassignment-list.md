---
title: Listar deviceConfigurationAssignments
description: Listar propriedades e relações dos objetos deviceConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 84ef78e1a9d5d122af2dd45af2341149f736e199
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131754"
---
# <a name="list-deviceconfigurationassignments"></a><span data-ttu-id="71a63-103">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="71a63-103">List deviceConfigurationAssignments</span></span>

<span data-ttu-id="71a63-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71a63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71a63-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="71a63-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71a63-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71a63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71a63-107">Listar propriedades e relações dos objetos [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="71a63-107">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71a63-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="71a63-108">Prerequisites</span></span>
<span data-ttu-id="71a63-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71a63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71a63-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71a63-111">Permission type</span></span>|<span data-ttu-id="71a63-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71a63-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71a63-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71a63-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71a63-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71a63-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71a63-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71a63-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71a63-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71a63-116">Not supported.</span></span>|
|<span data-ttu-id="71a63-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71a63-117">Application</span></span>|<span data-ttu-id="71a63-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71a63-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71a63-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71a63-119">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="71a63-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71a63-120">Request headers</span></span>
|<span data-ttu-id="71a63-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="71a63-121">Header</span></span>|<span data-ttu-id="71a63-122">Valor</span><span class="sxs-lookup"><span data-stu-id="71a63-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71a63-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="71a63-123">Authorization</span></span>|<span data-ttu-id="71a63-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71a63-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71a63-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="71a63-125">Accept</span></span>|<span data-ttu-id="71a63-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71a63-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71a63-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71a63-127">Request body</span></span>
<span data-ttu-id="71a63-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="71a63-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71a63-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="71a63-129">Response</span></span>
<span data-ttu-id="71a63-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71a63-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71a63-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71a63-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="71a63-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71a63-132">Request</span></span>
<span data-ttu-id="71a63-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71a63-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="71a63-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="71a63-134">Response</span></span>
<span data-ttu-id="71a63-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71a63-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 571

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```




