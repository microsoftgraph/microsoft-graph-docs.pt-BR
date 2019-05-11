---
title: Excluir detectedApp
description: Exclui detectedApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 70cfc39d871fbbac39c168b865cf8658a4ab214c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909957"
---
# <a name="delete-detectedapp"></a><span data-ttu-id="7bb15-103">Excluir detectedApp</span><span class="sxs-lookup"><span data-stu-id="7bb15-103">Delete detectedApp</span></span>

> <span data-ttu-id="7bb15-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7bb15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bb15-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7bb15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bb15-106">Exclui [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bb15-106">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7bb15-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7bb15-107">Prerequisites</span></span>
<span data-ttu-id="7bb15-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bb15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bb15-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7bb15-110">Permission type</span></span>|<span data-ttu-id="7bb15-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7bb15-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bb15-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7bb15-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7bb15-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bb15-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7bb15-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7bb15-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bb15-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bb15-115">Not supported.</span></span>|
|<span data-ttu-id="7bb15-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bb15-116">Application</span></span>|<span data-ttu-id="7bb15-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bb15-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bb15-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7bb15-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/detectedApps/{detectedAppId}
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="7bb15-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7bb15-119">Request headers</span></span>
|<span data-ttu-id="7bb15-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7bb15-120">Header</span></span>|<span data-ttu-id="7bb15-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7bb15-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7bb15-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7bb15-122">Authorization</span></span>|<span data-ttu-id="7bb15-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bb15-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7bb15-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7bb15-124">Accept</span></span>|<span data-ttu-id="7bb15-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7bb15-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bb15-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7bb15-126">Request body</span></span>
<span data-ttu-id="7bb15-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7bb15-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bb15-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bb15-128">Response</span></span>
<span data-ttu-id="7bb15-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7bb15-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7bb15-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7bb15-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7bb15-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bb15-131">Request</span></span>
<span data-ttu-id="7bb15-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7bb15-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/detectedApps/{detectedAppId}
```

### <a name="response"></a><span data-ttu-id="7bb15-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bb15-133">Response</span></span>
<span data-ttu-id="7bb15-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7bb15-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




