---
title: Excluir managedDeviceCertificateState
description: Exclui managedDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 172009471776d21be59f67a79b625010b60c3424
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132552"
---
# <a name="delete-manageddevicecertificatestate"></a><span data-ttu-id="a512b-103">Excluir managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="a512b-103">Delete managedDeviceCertificateState</span></span>

<span data-ttu-id="a512b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a512b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a512b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a512b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a512b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a512b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a512b-107">Exclui [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="a512b-107">Deletes a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a512b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a512b-108">Prerequisites</span></span>
<span data-ttu-id="a512b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a512b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a512b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a512b-111">Permission type</span></span>|<span data-ttu-id="a512b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a512b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a512b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a512b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a512b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a512b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a512b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a512b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a512b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a512b-116">Not supported.</span></span>|
|<span data-ttu-id="a512b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a512b-117">Application</span></span>|<span data-ttu-id="a512b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a512b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a512b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a512b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfilePkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="a512b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a512b-120">Request headers</span></span>
|<span data-ttu-id="a512b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a512b-121">Header</span></span>|<span data-ttu-id="a512b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a512b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a512b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a512b-123">Authorization</span></span>|<span data-ttu-id="a512b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a512b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a512b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a512b-125">Accept</span></span>|<span data-ttu-id="a512b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a512b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a512b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a512b-127">Request body</span></span>
<span data-ttu-id="a512b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a512b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a512b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a512b-129">Response</span></span>
<span data-ttu-id="a512b-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a512b-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a512b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a512b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a512b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a512b-132">Request</span></span>
<span data-ttu-id="a512b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a512b-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="a512b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a512b-134">Response</span></span>
<span data-ttu-id="a512b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a512b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




