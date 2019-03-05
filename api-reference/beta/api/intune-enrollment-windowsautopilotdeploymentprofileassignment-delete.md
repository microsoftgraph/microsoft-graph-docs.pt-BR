---
title: Excluir windowsAutopilotDeploymentProfileAssignment
description: Exclui windowsAutopilotDeploymentProfileAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d7b3123d26dff8bbc3ae438e11f92367da84c858
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171355"
---
# <a name="delete-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="3a2be-103">Excluir windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="3a2be-103">Delete windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="3a2be-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3a2be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a2be-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3a2be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a2be-106">Exclui [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3a2be-106">Deletes a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a2be-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3a2be-107">Prerequisites</span></span>
<span data-ttu-id="3a2be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3a2be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3a2be-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a2be-110">Permission type</span></span>|<span data-ttu-id="3a2be-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3a2be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a2be-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a2be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3a2be-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a2be-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3a2be-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a2be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a2be-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a2be-115">Not supported.</span></span>|
|<span data-ttu-id="3a2be-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a2be-116">Application</span></span>|<span data-ttu-id="3a2be-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a2be-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a2be-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a2be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="3a2be-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a2be-119">Request headers</span></span>
|<span data-ttu-id="3a2be-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a2be-120">Header</span></span>|<span data-ttu-id="3a2be-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3a2be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a2be-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a2be-122">Authorization</span></span>|<span data-ttu-id="3a2be-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a2be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a2be-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3a2be-124">Accept</span></span>|<span data-ttu-id="3a2be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3a2be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a2be-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a2be-126">Request body</span></span>
<span data-ttu-id="3a2be-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a2be-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a2be-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a2be-128">Response</span></span>
<span data-ttu-id="3a2be-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3a2be-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3a2be-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a2be-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a2be-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a2be-131">Request</span></span>
<span data-ttu-id="3a2be-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a2be-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

### <a name="response"></a><span data-ttu-id="3a2be-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a2be-133">Response</span></span>
<span data-ttu-id="3a2be-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a2be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




