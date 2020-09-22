---
title: Excluir deviceManagementScript
description: Exclui deviceManagementScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 97564203738499e1a90b5dc73358f31202a15a61
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074332"
---
# <a name="delete-devicemanagementscript"></a><span data-ttu-id="422dc-103">Excluir deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="422dc-103">Delete deviceManagementScript</span></span>

<span data-ttu-id="422dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="422dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="422dc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="422dc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="422dc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="422dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="422dc-107">Exclui [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="422dc-107">Deletes a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="422dc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="422dc-108">Prerequisites</span></span>
<span data-ttu-id="422dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="422dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="422dc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="422dc-111">Permission type</span></span>|<span data-ttu-id="422dc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="422dc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="422dc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="422dc-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="422dc-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="422dc-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="422dc-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="422dc-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="422dc-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="422dc-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="422dc-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="422dc-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="422dc-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="422dc-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="422dc-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="422dc-119">Not supported.</span></span>|
|<span data-ttu-id="422dc-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="422dc-120">Application</span></span>||
| <span data-ttu-id="422dc-121">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="422dc-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="422dc-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="422dc-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="422dc-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="422dc-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="422dc-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="422dc-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="422dc-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="422dc-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="422dc-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="422dc-126">Request headers</span></span>
|<span data-ttu-id="422dc-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="422dc-127">Header</span></span>|<span data-ttu-id="422dc-128">Valor</span><span class="sxs-lookup"><span data-stu-id="422dc-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="422dc-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="422dc-129">Authorization</span></span>|<span data-ttu-id="422dc-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="422dc-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="422dc-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="422dc-131">Accept</span></span>|<span data-ttu-id="422dc-132">application/json</span><span class="sxs-lookup"><span data-stu-id="422dc-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="422dc-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="422dc-133">Request body</span></span>
<span data-ttu-id="422dc-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="422dc-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="422dc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="422dc-135">Response</span></span>
<span data-ttu-id="422dc-136">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="422dc-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="422dc-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="422dc-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="422dc-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="422dc-138">Request</span></span>
<span data-ttu-id="422dc-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="422dc-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

### <a name="response"></a><span data-ttu-id="422dc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="422dc-140">Response</span></span>
<span data-ttu-id="422dc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="422dc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









