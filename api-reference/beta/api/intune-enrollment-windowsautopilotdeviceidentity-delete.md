---
title: Excluir windowsAutopilotDeviceIdentity
description: Exclui windowsAutopilotDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 915b528fd66a45a44f35d435df1e59cc1ea87e37
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943695"
---
# <a name="delete-windowsautopilotdeviceidentity"></a><span data-ttu-id="e1b78-103">Excluir windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="e1b78-103">Delete windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="e1b78-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e1b78-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1b78-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1b78-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1b78-106">Exclui [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="e1b78-106">Deletes a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1b78-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1b78-107">Prerequisites</span></span>
<span data-ttu-id="e1b78-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1b78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1b78-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1b78-110">Permission type</span></span>|<span data-ttu-id="e1b78-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1b78-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1b78-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1b78-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e1b78-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1b78-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e1b78-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1b78-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1b78-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1b78-115">Not supported.</span></span>|
|<span data-ttu-id="e1b78-116">Application</span><span class="sxs-lookup"><span data-stu-id="e1b78-116">Application</span></span>|<span data-ttu-id="e1b78-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1b78-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1b78-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1b78-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
DELETE /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="e1b78-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1b78-119">Request headers</span></span>
|<span data-ttu-id="e1b78-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1b78-120">Header</span></span>|<span data-ttu-id="e1b78-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e1b78-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1b78-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1b78-122">Authorization</span></span>|<span data-ttu-id="e1b78-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1b78-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1b78-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1b78-124">Accept</span></span>|<span data-ttu-id="e1b78-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e1b78-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1b78-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1b78-126">Request body</span></span>
<span data-ttu-id="e1b78-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1b78-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1b78-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1b78-128">Response</span></span>
<span data-ttu-id="e1b78-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e1b78-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e1b78-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1b78-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1b78-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1b78-131">Request</span></span>
<span data-ttu-id="e1b78-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1b78-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="e1b78-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1b78-133">Response</span></span>
<span data-ttu-id="e1b78-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1b78-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





