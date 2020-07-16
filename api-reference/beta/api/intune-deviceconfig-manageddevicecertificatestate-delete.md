---
title: Excluir managedDeviceCertificateState
description: Exclui managedDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c66af6b517cd68ff475ab04fbc6bf244b7988a53
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122886"
---
# <a name="delete-manageddevicecertificatestate"></a><span data-ttu-id="e058a-103">Excluir managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="e058a-103">Delete managedDeviceCertificateState</span></span>

<span data-ttu-id="e058a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e058a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e058a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e058a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e058a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e058a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e058a-107">Exclui [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="e058a-107">Deletes a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e058a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e058a-108">Prerequisites</span></span>
<span data-ttu-id="e058a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e058a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e058a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e058a-111">Permission type</span></span>|<span data-ttu-id="e058a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e058a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e058a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e058a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e058a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e058a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e058a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e058a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e058a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e058a-116">Not supported.</span></span>|
|<span data-ttu-id="e058a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e058a-117">Application</span></span>|<span data-ttu-id="e058a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e058a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e058a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e058a-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e058a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e058a-120">Request headers</span></span>
|<span data-ttu-id="e058a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e058a-121">Header</span></span>|<span data-ttu-id="e058a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e058a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e058a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e058a-123">Authorization</span></span>|<span data-ttu-id="e058a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e058a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e058a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e058a-125">Accept</span></span>|<span data-ttu-id="e058a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e058a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e058a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e058a-127">Request body</span></span>
<span data-ttu-id="e058a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e058a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e058a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e058a-129">Response</span></span>
<span data-ttu-id="e058a-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e058a-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e058a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e058a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e058a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e058a-132">Request</span></span>
<span data-ttu-id="e058a-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e058a-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="e058a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e058a-134">Response</span></span>
<span data-ttu-id="e058a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e058a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



