---
title: Excluir windowsUpdateState
description: Exclui windowsUpdateState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f86c4114ccd0cf06313c4a50bdb83d83ae033caf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457920"
---
# <a name="delete-windowsupdatestate"></a><span data-ttu-id="7bf61-103">Excluir windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="7bf61-103">Delete windowsUpdateState</span></span>

<span data-ttu-id="7bf61-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7bf61-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7bf61-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7bf61-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bf61-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7bf61-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bf61-107">Exclui [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="7bf61-107">Deletes a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7bf61-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7bf61-108">Prerequisites</span></span>
<span data-ttu-id="7bf61-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bf61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bf61-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7bf61-111">Permission type</span></span>|<span data-ttu-id="7bf61-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7bf61-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bf61-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7bf61-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7bf61-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="7bf61-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="7bf61-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bf61-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="7bf61-116">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="7bf61-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="7bf61-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bf61-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7bf61-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7bf61-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bf61-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bf61-119">Not supported.</span></span>|
|<span data-ttu-id="7bf61-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bf61-120">Application</span></span>||
| <span data-ttu-id="7bf61-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="7bf61-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="7bf61-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bf61-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="7bf61-123">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="7bf61-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="7bf61-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bf61-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bf61-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7bf61-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="7bf61-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7bf61-126">Request headers</span></span>
|<span data-ttu-id="7bf61-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7bf61-127">Header</span></span>|<span data-ttu-id="7bf61-128">Valor</span><span class="sxs-lookup"><span data-stu-id="7bf61-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7bf61-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="7bf61-129">Authorization</span></span>|<span data-ttu-id="7bf61-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bf61-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7bf61-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7bf61-131">Accept</span></span>|<span data-ttu-id="7bf61-132">application/json</span><span class="sxs-lookup"><span data-stu-id="7bf61-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bf61-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7bf61-133">Request body</span></span>
<span data-ttu-id="7bf61-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7bf61-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bf61-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bf61-135">Response</span></span>
<span data-ttu-id="7bf61-136">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7bf61-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7bf61-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7bf61-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="7bf61-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bf61-138">Request</span></span>
<span data-ttu-id="7bf61-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7bf61-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

### <a name="response"></a><span data-ttu-id="7bf61-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bf61-140">Response</span></span>
<span data-ttu-id="7bf61-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7bf61-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








