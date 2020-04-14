---
title: Excluir deviceManagementScriptUserState
description: Exclui deviceManagementScriptUserState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9bfe8da15f608dccf8f01ebbb31e4e425cb85006
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43425782"
---
# <a name="delete-devicemanagementscriptuserstate"></a><span data-ttu-id="b8140-103">Excluir deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="b8140-103">Delete deviceManagementScriptUserState</span></span>

<span data-ttu-id="b8140-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8140-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8140-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b8140-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8140-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8140-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8140-107">Exclui [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span><span class="sxs-lookup"><span data-stu-id="b8140-107">Deletes a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8140-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b8140-108">Prerequisites</span></span>
<span data-ttu-id="b8140-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8140-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8140-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8140-111">Permission type</span></span>|<span data-ttu-id="b8140-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b8140-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8140-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8140-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8140-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8140-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b8140-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8140-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8140-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8140-116">Not supported.</span></span>|
|<span data-ttu-id="b8140-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8140-117">Application</span></span>|<span data-ttu-id="b8140-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8140-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8140-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8140-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="b8140-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8140-120">Request headers</span></span>
|<span data-ttu-id="b8140-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8140-121">Header</span></span>|<span data-ttu-id="b8140-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b8140-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8140-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8140-123">Authorization</span></span>|<span data-ttu-id="b8140-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8140-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8140-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b8140-125">Accept</span></span>|<span data-ttu-id="b8140-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8140-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8140-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8140-127">Request body</span></span>
<span data-ttu-id="b8140-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8140-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8140-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8140-129">Response</span></span>
<span data-ttu-id="b8140-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b8140-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b8140-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8140-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8140-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8140-132">Request</span></span>
<span data-ttu-id="b8140-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8140-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

### <a name="response"></a><span data-ttu-id="b8140-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8140-134">Response</span></span>
<span data-ttu-id="b8140-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8140-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



