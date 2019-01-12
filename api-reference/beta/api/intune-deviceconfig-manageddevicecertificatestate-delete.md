---
title: Excluir managedDeviceCertificateState
description: Exclui um managedDeviceCertificateState.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: da38b1feaeae9911d887dfdda8ca5845be0dae80
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982530"
---
# <a name="delete-manageddevicecertificatestate"></a><span data-ttu-id="7df73-103">Excluir managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="7df73-103">Delete managedDeviceCertificateState</span></span>

> <span data-ttu-id="7df73-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7df73-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7df73-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7df73-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7df73-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7df73-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7df73-107">Exclui um [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="7df73-107">Deletes a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7df73-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7df73-108">Prerequisites</span></span>
<span data-ttu-id="7df73-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7df73-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7df73-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7df73-111">Permission type</span></span>|<span data-ttu-id="7df73-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7df73-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7df73-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7df73-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7df73-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7df73-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7df73-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7df73-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7df73-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7df73-116">Not supported.</span></span>|
|<span data-ttu-id="7df73-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7df73-117">Application</span></span>|<span data-ttu-id="7df73-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7df73-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7df73-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7df73-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="7df73-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7df73-120">Request headers</span></span>
|<span data-ttu-id="7df73-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7df73-121">Header</span></span>|<span data-ttu-id="7df73-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7df73-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7df73-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7df73-123">Authorization</span></span>|<span data-ttu-id="7df73-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7df73-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7df73-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7df73-125">Accept</span></span>|<span data-ttu-id="7df73-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7df73-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7df73-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7df73-127">Request body</span></span>
<span data-ttu-id="7df73-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7df73-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7df73-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7df73-129">Response</span></span>
<span data-ttu-id="7df73-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7df73-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7df73-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7df73-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="7df73-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7df73-132">Request</span></span>
<span data-ttu-id="7df73-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7df73-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="7df73-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7df73-134">Response</span></span>
<span data-ttu-id="7df73-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7df73-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





