---
title: Excluir windowsUpdateState
description: Exclui windowsUpdateState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5cb29c5212d44c9affa895dc9dbe15b56e74e146
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199520"
---
# <a name="delete-windowsupdatestate"></a><span data-ttu-id="622d2-103">Excluir windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="622d2-103">Delete windowsUpdateState</span></span>

> <span data-ttu-id="622d2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="622d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="622d2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="622d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="622d2-106">Exclui [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="622d2-106">Deletes a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="622d2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="622d2-107">Prerequisites</span></span>
<span data-ttu-id="622d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="622d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="622d2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="622d2-110">Permission type</span></span>|<span data-ttu-id="622d2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="622d2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="622d2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="622d2-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="622d2-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="622d2-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="622d2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="622d2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="622d2-115">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="622d2-115">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="622d2-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="622d2-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="622d2-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="622d2-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="622d2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="622d2-118">Not supported.</span></span>|
|<span data-ttu-id="622d2-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="622d2-119">Application</span></span>||
| <span data-ttu-id="622d2-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="622d2-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="622d2-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="622d2-121">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="622d2-122">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="622d2-122">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="622d2-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="622d2-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="622d2-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="622d2-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="622d2-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="622d2-125">Request headers</span></span>
|<span data-ttu-id="622d2-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="622d2-126">Header</span></span>|<span data-ttu-id="622d2-127">Valor</span><span class="sxs-lookup"><span data-stu-id="622d2-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="622d2-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="622d2-128">Authorization</span></span>|<span data-ttu-id="622d2-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="622d2-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="622d2-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="622d2-130">Accept</span></span>|<span data-ttu-id="622d2-131">application/json</span><span class="sxs-lookup"><span data-stu-id="622d2-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="622d2-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="622d2-132">Request body</span></span>
<span data-ttu-id="622d2-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="622d2-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="622d2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="622d2-134">Response</span></span>
<span data-ttu-id="622d2-135">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="622d2-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="622d2-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="622d2-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="622d2-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="622d2-137">Request</span></span>
<span data-ttu-id="622d2-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="622d2-138">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

### <a name="response"></a><span data-ttu-id="622d2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="622d2-139">Response</span></span>
<span data-ttu-id="622d2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="622d2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




