---
title: Excluir windowsUpdateState
description: Exclui windowsUpdateState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9b318e286da7fbfe5903382b5f9d368d565cd56b
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085434"
---
# <a name="delete-windowsupdatestate"></a><span data-ttu-id="de61e-103">Excluir windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="de61e-103">Delete windowsUpdateState</span></span>

> <span data-ttu-id="de61e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="de61e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de61e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="de61e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de61e-106">Exclui [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="de61e-106">Deletes a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de61e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="de61e-107">Prerequisites</span></span>
<span data-ttu-id="de61e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de61e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de61e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de61e-110">Permission type</span></span>|<span data-ttu-id="de61e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="de61e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de61e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de61e-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="de61e-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="de61e-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="de61e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de61e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="de61e-115">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="de61e-115">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="de61e-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de61e-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de61e-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de61e-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de61e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de61e-118">Not supported.</span></span>|
|<span data-ttu-id="de61e-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de61e-119">Application</span></span>||
| <span data-ttu-id="de61e-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="de61e-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="de61e-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de61e-121">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="de61e-122">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="de61e-122">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="de61e-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de61e-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de61e-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de61e-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="de61e-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de61e-125">Request headers</span></span>
|<span data-ttu-id="de61e-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="de61e-126">Header</span></span>|<span data-ttu-id="de61e-127">Valor</span><span class="sxs-lookup"><span data-stu-id="de61e-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de61e-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="de61e-128">Authorization</span></span>|<span data-ttu-id="de61e-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de61e-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de61e-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="de61e-130">Accept</span></span>|<span data-ttu-id="de61e-131">application/json</span><span class="sxs-lookup"><span data-stu-id="de61e-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de61e-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de61e-132">Request body</span></span>
<span data-ttu-id="de61e-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="de61e-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de61e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="de61e-134">Response</span></span>
<span data-ttu-id="de61e-135">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="de61e-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="de61e-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de61e-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="de61e-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de61e-137">Request</span></span>
<span data-ttu-id="de61e-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de61e-138">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

### <a name="response"></a><span data-ttu-id="de61e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="de61e-139">Response</span></span>
<span data-ttu-id="de61e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de61e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









