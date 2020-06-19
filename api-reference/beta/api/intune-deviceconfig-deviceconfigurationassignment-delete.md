---
title: Excluir deviceConfigurationAssignment
description: Exclui deviceConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 09199ef90d4d484d48d8d35c0b60ec875a1783e0
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792993"
---
# <a name="delete-deviceconfigurationassignment"></a><span data-ttu-id="e4bb8-103">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e4bb8-103">Delete deviceConfigurationAssignment</span></span>

<span data-ttu-id="e4bb8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4bb8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4bb8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e4bb8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4bb8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4bb8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4bb8-107">Exclui [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e4bb8-107">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4bb8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e4bb8-108">Prerequisites</span></span>
<span data-ttu-id="e4bb8-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e4bb8-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e4bb8-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4bb8-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4bb8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4bb8-111">Permission type</span></span>|<span data-ttu-id="e4bb8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e4bb8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4bb8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4bb8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4bb8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4bb8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e4bb8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4bb8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4bb8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4bb8-116">Not supported.</span></span>|
|<span data-ttu-id="e4bb8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4bb8-117">Application</span></span>|<span data-ttu-id="e4bb8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4bb8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4bb8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4bb8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e4bb8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4bb8-120">Request headers</span></span>
|<span data-ttu-id="e4bb8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4bb8-121">Header</span></span>|<span data-ttu-id="e4bb8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e4bb8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4bb8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4bb8-123">Authorization</span></span>|<span data-ttu-id="e4bb8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4bb8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4bb8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e4bb8-125">Accept</span></span>|<span data-ttu-id="e4bb8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4bb8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4bb8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4bb8-127">Request body</span></span>
<span data-ttu-id="e4bb8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e4bb8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4bb8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4bb8-129">Response</span></span>
<span data-ttu-id="e4bb8-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e4bb8-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e4bb8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4bb8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4bb8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4bb8-132">Request</span></span>
<span data-ttu-id="e4bb8-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4bb8-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="e4bb8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4bb8-134">Response</span></span>
<span data-ttu-id="e4bb8-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="e4bb8-135">Here is an example of the response.</span></span> <span data-ttu-id="e4bb8-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="e4bb8-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e4bb8-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="e4bb8-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



