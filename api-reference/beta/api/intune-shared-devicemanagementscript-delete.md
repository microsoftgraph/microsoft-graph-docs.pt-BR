---
title: Excluir deviceManagementScript
description: Exclui deviceManagementScript.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3b92f2d8bf06e6ff12d37ed56aa61b5fa3c3315d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800974"
---
# <a name="delete-devicemanagementscript"></a><span data-ttu-id="c4c4c-103">Excluir deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="c4c4c-103">Delete deviceManagementScript</span></span>

> <span data-ttu-id="c4c4c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c4c4c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4c4c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4c4c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4c4c-106">Exclui [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="c4c4c-106">Deletes a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4c4c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4c4c-107">Prerequisites</span></span>
<span data-ttu-id="c4c4c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4c4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4c4c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4c4c-110">Permission type</span></span>|<span data-ttu-id="c4c4c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c4c4c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4c4c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4c4c-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c4c4c-113">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c4c4c-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c4c4c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4c4c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="c4c4c-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="c4c4c-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c4c4c-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4c4c-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c4c4c-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4c4c-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4c4c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4c4c-118">Not supported.</span></span>|
|<span data-ttu-id="c4c4c-119">Application</span><span class="sxs-lookup"><span data-stu-id="c4c4c-119">Application</span></span>||
| <span data-ttu-id="c4c4c-120">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c4c4c-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c4c4c-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4c4c-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="c4c4c-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="c4c4c-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c4c4c-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4c4c-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4c4c-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4c4c-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="c4c4c-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4c4c-125">Request headers</span></span>
|<span data-ttu-id="c4c4c-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4c4c-126">Header</span></span>|<span data-ttu-id="c4c4c-127">Valor</span><span class="sxs-lookup"><span data-stu-id="c4c4c-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4c4c-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4c4c-128">Authorization</span></span>|<span data-ttu-id="c4c4c-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4c4c-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4c4c-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c4c4c-130">Accept</span></span>|<span data-ttu-id="c4c4c-131">application/json</span><span class="sxs-lookup"><span data-stu-id="c4c4c-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4c4c-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4c4c-132">Request body</span></span>
<span data-ttu-id="c4c4c-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4c4c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4c4c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4c4c-134">Response</span></span>
<span data-ttu-id="c4c4c-135">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c4c4c-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c4c4c-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4c4c-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4c4c-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4c4c-137">Request</span></span>
<span data-ttu-id="c4c4c-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4c4c-138">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

### <a name="response"></a><span data-ttu-id="c4c4c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4c4c-139">Response</span></span>
<span data-ttu-id="c4c4c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4c4c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







