---
title: Excluir windowsAutopilotDeviceIdentity
description: Exclui windowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 544e2d6aeea6deed991ddb3bcbbcf4f411a61773
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49309422"
---
# <a name="delete-windowsautopilotdeviceidentity"></a><span data-ttu-id="b8464-103">Excluir windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="b8464-103">Delete windowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="b8464-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8464-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8464-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b8464-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8464-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8464-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8464-107">Exclui [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="b8464-107">Deletes a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8464-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b8464-108">Prerequisites</span></span>
<span data-ttu-id="b8464-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8464-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8464-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8464-111">Permission type</span></span>|<span data-ttu-id="b8464-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b8464-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8464-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8464-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8464-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8464-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b8464-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8464-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8464-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8464-116">Not supported.</span></span>|
|<span data-ttu-id="b8464-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8464-117">Application</span></span>|<span data-ttu-id="b8464-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8464-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8464-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8464-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
DELETE /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="b8464-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8464-120">Request headers</span></span>
|<span data-ttu-id="b8464-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8464-121">Header</span></span>|<span data-ttu-id="b8464-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b8464-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8464-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8464-123">Authorization</span></span>|<span data-ttu-id="b8464-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8464-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8464-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b8464-125">Accept</span></span>|<span data-ttu-id="b8464-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8464-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8464-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8464-127">Request body</span></span>
<span data-ttu-id="b8464-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8464-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8464-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8464-129">Response</span></span>
<span data-ttu-id="b8464-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b8464-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b8464-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8464-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8464-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8464-132">Request</span></span>
<span data-ttu-id="b8464-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8464-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="b8464-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8464-134">Response</span></span>
<span data-ttu-id="b8464-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8464-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




