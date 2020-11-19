---
title: Excluir deviceManagementScriptDeviceState
description: Exclui deviceManagementScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dda5dc75770dbd5285afa30272531c26521e18bf
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49212913"
---
# <a name="delete-devicemanagementscriptdevicestate"></a><span data-ttu-id="760dd-103">Excluir deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="760dd-103">Delete deviceManagementScriptDeviceState</span></span>

<span data-ttu-id="760dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="760dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="760dd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="760dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="760dd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="760dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="760dd-107">Exclui [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="760dd-107">Deletes a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="760dd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="760dd-108">Prerequisites</span></span>
<span data-ttu-id="760dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="760dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="760dd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="760dd-111">Permission type</span></span>|<span data-ttu-id="760dd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="760dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="760dd-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="760dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="760dd-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="760dd-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="760dd-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="760dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="760dd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="760dd-116">Not supported.</span></span>|
|<span data-ttu-id="760dd-117">Application</span><span class="sxs-lookup"><span data-stu-id="760dd-117">Application</span></span>|<span data-ttu-id="760dd-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="760dd-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="760dd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="760dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
DELETE /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="760dd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="760dd-120">Request headers</span></span>
|<span data-ttu-id="760dd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="760dd-121">Header</span></span>|<span data-ttu-id="760dd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="760dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="760dd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="760dd-123">Authorization</span></span>|<span data-ttu-id="760dd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="760dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="760dd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="760dd-125">Accept</span></span>|<span data-ttu-id="760dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="760dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="760dd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="760dd-127">Request body</span></span>
<span data-ttu-id="760dd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="760dd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="760dd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="760dd-129">Response</span></span>
<span data-ttu-id="760dd-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="760dd-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="760dd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="760dd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="760dd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="760dd-132">Request</span></span>
<span data-ttu-id="760dd-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="760dd-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="760dd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="760dd-134">Response</span></span>
<span data-ttu-id="760dd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="760dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




