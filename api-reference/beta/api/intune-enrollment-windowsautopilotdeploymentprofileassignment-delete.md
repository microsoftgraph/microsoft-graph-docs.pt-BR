---
title: Excluir windowsAutopilotDeploymentProfileAssignment
description: Exclui windowsAutopilotDeploymentProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3ba7266879cade8576ad08b6bdf067cecfc0021d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49218479"
---
# <a name="delete-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="cd9bf-103">Excluir windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="cd9bf-103">Delete windowsAutopilotDeploymentProfileAssignment</span></span>

<span data-ttu-id="cd9bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd9bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd9bf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cd9bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd9bf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cd9bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd9bf-107">Exclui [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cd9bf-107">Deletes a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd9bf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cd9bf-108">Prerequisites</span></span>
<span data-ttu-id="cd9bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd9bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd9bf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd9bf-111">Permission type</span></span>|<span data-ttu-id="cd9bf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cd9bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd9bf-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd9bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cd9bf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd9bf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cd9bf-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd9bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd9bf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd9bf-116">Not supported.</span></span>|
|<span data-ttu-id="cd9bf-117">Application</span><span class="sxs-lookup"><span data-stu-id="cd9bf-117">Application</span></span>|<span data-ttu-id="cd9bf-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd9bf-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd9bf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd9bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="cd9bf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd9bf-120">Request headers</span></span>
|<span data-ttu-id="cd9bf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cd9bf-121">Header</span></span>|<span data-ttu-id="cd9bf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cd9bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd9bf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd9bf-123">Authorization</span></span>|<span data-ttu-id="cd9bf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd9bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd9bf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cd9bf-125">Accept</span></span>|<span data-ttu-id="cd9bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cd9bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd9bf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd9bf-127">Request body</span></span>
<span data-ttu-id="cd9bf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cd9bf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd9bf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd9bf-129">Response</span></span>
<span data-ttu-id="cd9bf-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cd9bf-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cd9bf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd9bf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd9bf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd9bf-132">Request</span></span>
<span data-ttu-id="cd9bf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd9bf-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

### <a name="response"></a><span data-ttu-id="cd9bf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd9bf-134">Response</span></span>
<span data-ttu-id="cd9bf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cd9bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




