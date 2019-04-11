---
title: Excluir securityBaselineSettingState
description: Exclui securityBaselineSettingState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 84c12d56e33d2e8a1a4c44d2a77faad470eed8b7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805562"
---
# <a name="delete-securitybaselinesettingstate"></a><span data-ttu-id="023af-103">Excluir securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="023af-103">Delete securityBaselineSettingState</span></span>

> <span data-ttu-id="023af-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="023af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="023af-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="023af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="023af-106">Exclui [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="023af-106">Deletes a [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="023af-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="023af-107">Prerequisites</span></span>
<span data-ttu-id="023af-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="023af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="023af-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="023af-110">Permission type</span></span>|<span data-ttu-id="023af-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="023af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="023af-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="023af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="023af-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="023af-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="023af-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="023af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="023af-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="023af-115">Not supported.</span></span>|
|<span data-ttu-id="023af-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="023af-116">Application</span></span>|<span data-ttu-id="023af-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="023af-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="023af-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="023af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates/{securityBaselineSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="023af-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="023af-119">Request headers</span></span>
|<span data-ttu-id="023af-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="023af-120">Header</span></span>|<span data-ttu-id="023af-121">Valor</span><span class="sxs-lookup"><span data-stu-id="023af-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="023af-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="023af-122">Authorization</span></span>|<span data-ttu-id="023af-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="023af-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="023af-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="023af-124">Accept</span></span>|<span data-ttu-id="023af-125">application/json</span><span class="sxs-lookup"><span data-stu-id="023af-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="023af-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="023af-126">Request body</span></span>
<span data-ttu-id="023af-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="023af-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="023af-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="023af-128">Response</span></span>
<span data-ttu-id="023af-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="023af-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="023af-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="023af-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="023af-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="023af-131">Request</span></span>
<span data-ttu-id="023af-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="023af-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates/{securityBaselineSettingStateId}
```

### <a name="response"></a><span data-ttu-id="023af-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="023af-133">Response</span></span>
<span data-ttu-id="023af-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="023af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



