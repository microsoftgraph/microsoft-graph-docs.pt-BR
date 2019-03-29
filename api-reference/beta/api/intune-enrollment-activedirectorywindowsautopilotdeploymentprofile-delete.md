---
title: Excluir activeDirectoryWindowsAutopilotDeploymentProfile
description: Exclui activeDirectoryWindowsAutopilotDeploymentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0e14adc6b2b492733363370ba0d13e5720d307a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978161"
---
# <a name="delete-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="ef7a8-103">Excluir activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="ef7a8-103">Delete activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="ef7a8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ef7a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef7a8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ef7a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef7a8-106">Exclui [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="ef7a8-106">Deletes a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef7a8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ef7a8-107">Prerequisites</span></span>
<span data-ttu-id="ef7a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef7a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef7a8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef7a8-110">Permission type</span></span>|<span data-ttu-id="ef7a8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ef7a8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef7a8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef7a8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef7a8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef7a8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ef7a8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef7a8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef7a8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef7a8-115">Not supported.</span></span>|
|<span data-ttu-id="ef7a8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef7a8-116">Application</span></span>|<span data-ttu-id="ef7a8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef7a8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef7a8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef7a8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
DELETE /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
DELETE /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="ef7a8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef7a8-119">Request headers</span></span>
|<span data-ttu-id="ef7a8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef7a8-120">Header</span></span>|<span data-ttu-id="ef7a8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ef7a8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef7a8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef7a8-122">Authorization</span></span>|<span data-ttu-id="ef7a8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef7a8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef7a8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ef7a8-124">Accept</span></span>|<span data-ttu-id="ef7a8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ef7a8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef7a8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef7a8-126">Request body</span></span>
<span data-ttu-id="ef7a8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ef7a8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef7a8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef7a8-128">Response</span></span>
<span data-ttu-id="ef7a8-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ef7a8-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ef7a8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef7a8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef7a8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef7a8-131">Request</span></span>
<span data-ttu-id="ef7a8-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef7a8-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="ef7a8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef7a8-133">Response</span></span>
<span data-ttu-id="ef7a8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef7a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




