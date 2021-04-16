---
title: Excluir windowsUpdateState
description: Exclui um windowsUpdateState.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 75212db281d3d14b27f69ff3e342f7af33ffb513
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863027"
---
# <a name="delete-windowsupdatestate"></a><span data-ttu-id="6262d-103">Excluir windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="6262d-103">Delete windowsUpdateState</span></span>

<span data-ttu-id="6262d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6262d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6262d-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6262d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6262d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6262d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6262d-107">Exclui um [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="6262d-107">Deletes a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6262d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6262d-108">Prerequisites</span></span>
<span data-ttu-id="6262d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6262d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6262d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6262d-111">Permission type</span></span>|<span data-ttu-id="6262d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6262d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6262d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6262d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6262d-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="6262d-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="6262d-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6262d-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="6262d-116">&nbsp;&nbsp; **Atualização de Software**</span><span class="sxs-lookup"><span data-stu-id="6262d-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="6262d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6262d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6262d-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6262d-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6262d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6262d-119">Not supported.</span></span>|
|<span data-ttu-id="6262d-120">Application</span><span class="sxs-lookup"><span data-stu-id="6262d-120">Application</span></span>||
| <span data-ttu-id="6262d-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="6262d-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="6262d-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6262d-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="6262d-123">&nbsp;&nbsp; **Atualização de Software**</span><span class="sxs-lookup"><span data-stu-id="6262d-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="6262d-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6262d-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6262d-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6262d-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="6262d-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6262d-126">Request headers</span></span>
|<span data-ttu-id="6262d-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6262d-127">Header</span></span>|<span data-ttu-id="6262d-128">Valor</span><span class="sxs-lookup"><span data-stu-id="6262d-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6262d-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="6262d-129">Authorization</span></span>|<span data-ttu-id="6262d-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6262d-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6262d-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6262d-131">Accept</span></span>|<span data-ttu-id="6262d-132">application/json</span><span class="sxs-lookup"><span data-stu-id="6262d-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6262d-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6262d-133">Request body</span></span>
<span data-ttu-id="6262d-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6262d-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6262d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6262d-135">Response</span></span>
<span data-ttu-id="6262d-136">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6262d-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6262d-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6262d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="6262d-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6262d-138">Request</span></span>
<span data-ttu-id="6262d-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6262d-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

### <a name="response"></a><span data-ttu-id="6262d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6262d-140">Response</span></span>
<span data-ttu-id="6262d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6262d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







