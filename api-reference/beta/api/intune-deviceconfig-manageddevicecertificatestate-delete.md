---
title: Excluir managedDeviceCertificateState
description: Exclui managedDeviceCertificateState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bed52c4168ae16ca1b86c712f7db500b9e338fb8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966989"
---
# <a name="delete-manageddevicecertificatestate"></a><span data-ttu-id="40cec-103">Excluir managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="40cec-103">Delete managedDeviceCertificateState</span></span>

> <span data-ttu-id="40cec-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="40cec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40cec-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="40cec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40cec-106">Exclui [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="40cec-106">Deletes a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40cec-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="40cec-107">Prerequisites</span></span>
<span data-ttu-id="40cec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40cec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40cec-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40cec-110">Permission type</span></span>|<span data-ttu-id="40cec-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="40cec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40cec-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40cec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="40cec-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40cec-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="40cec-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40cec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40cec-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40cec-115">Not supported.</span></span>|
|<span data-ttu-id="40cec-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40cec-116">Application</span></span>|<span data-ttu-id="40cec-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40cec-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40cec-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40cec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="40cec-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40cec-119">Request headers</span></span>
|<span data-ttu-id="40cec-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40cec-120">Header</span></span>|<span data-ttu-id="40cec-121">Valor</span><span class="sxs-lookup"><span data-stu-id="40cec-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40cec-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="40cec-122">Authorization</span></span>|<span data-ttu-id="40cec-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40cec-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40cec-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="40cec-124">Accept</span></span>|<span data-ttu-id="40cec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="40cec-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40cec-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40cec-126">Request body</span></span>
<span data-ttu-id="40cec-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="40cec-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40cec-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="40cec-128">Response</span></span>
<span data-ttu-id="40cec-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="40cec-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="40cec-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40cec-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="40cec-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40cec-131">Request</span></span>
<span data-ttu-id="40cec-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40cec-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="40cec-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="40cec-133">Response</span></span>
<span data-ttu-id="40cec-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40cec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




