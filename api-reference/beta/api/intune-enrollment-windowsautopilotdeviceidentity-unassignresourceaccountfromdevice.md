---
title: Ação unassignResourceAccountFromDevice
description: Retira a atribuição da conta de recurso de um dispositivo de piloto automático.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe71d4112a7b4a764ee466f50ca6598245a5b66c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908155"
---
# <a name="unassignresourceaccountfromdevice-action"></a><span data-ttu-id="7fb59-103">Ação unassignResourceAccountFromDevice</span><span class="sxs-lookup"><span data-stu-id="7fb59-103">unassignResourceAccountFromDevice action</span></span>

> <span data-ttu-id="7fb59-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7fb59-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7fb59-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7fb59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fb59-106">Retira a atribuição da conta de recurso de um dispositivo de piloto automático.</span><span class="sxs-lookup"><span data-stu-id="7fb59-106">Unassigns the resource account from an Autopilot device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7fb59-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7fb59-107">Prerequisites</span></span>
<span data-ttu-id="7fb59-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fb59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fb59-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fb59-110">Permission type</span></span>|<span data-ttu-id="7fb59-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7fb59-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fb59-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fb59-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7fb59-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fb59-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7fb59-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fb59-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fb59-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fb59-115">Not supported.</span></span>|
|<span data-ttu-id="7fb59-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fb59-116">Application</span></span>|<span data-ttu-id="7fb59-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fb59-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fb59-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fb59-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/unassignResourceAccountFromDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/unassignResourceAccountFromDevice
```

## <a name="request-headers"></a><span data-ttu-id="7fb59-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fb59-119">Request headers</span></span>
|<span data-ttu-id="7fb59-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7fb59-120">Header</span></span>|<span data-ttu-id="7fb59-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7fb59-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fb59-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7fb59-122">Authorization</span></span>|<span data-ttu-id="7fb59-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7fb59-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fb59-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7fb59-124">Accept</span></span>|<span data-ttu-id="7fb59-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7fb59-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fb59-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fb59-126">Request body</span></span>
<span data-ttu-id="7fb59-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7fb59-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fb59-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fb59-128">Response</span></span>
<span data-ttu-id="7fb59-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7fb59-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7fb59-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7fb59-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fb59-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fb59-131">Request</span></span>
<span data-ttu-id="7fb59-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fb59-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/unassignResourceAccountFromDevice
```

### <a name="response"></a><span data-ttu-id="7fb59-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fb59-133">Response</span></span>
<span data-ttu-id="7fb59-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7fb59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




