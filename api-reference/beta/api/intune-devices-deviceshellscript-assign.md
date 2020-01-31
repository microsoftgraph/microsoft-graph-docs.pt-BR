---
title: atribuir ação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c1a888271cfdd03d13101b7adaeff9295b61b44e
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636466"
---
# <a name="assign-action"></a><span data-ttu-id="610bb-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="610bb-103">assign action</span></span>

> <span data-ttu-id="610bb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="610bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="610bb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="610bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="610bb-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="610bb-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="610bb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="610bb-107">Prerequisites</span></span>
<span data-ttu-id="610bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="610bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="610bb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="610bb-110">Permission type</span></span>|<span data-ttu-id="610bb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="610bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="610bb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="610bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="610bb-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="610bb-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="610bb-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="610bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="610bb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="610bb-115">Not supported.</span></span>|
|<span data-ttu-id="610bb-116">Application</span><span class="sxs-lookup"><span data-stu-id="610bb-116">Application</span></span>|<span data-ttu-id="610bb-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="610bb-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="610bb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="610bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="610bb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="610bb-119">Request headers</span></span>
|<span data-ttu-id="610bb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="610bb-120">Header</span></span>|<span data-ttu-id="610bb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="610bb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="610bb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="610bb-122">Authorization</span></span>|<span data-ttu-id="610bb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="610bb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="610bb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="610bb-124">Accept</span></span>|<span data-ttu-id="610bb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="610bb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="610bb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="610bb-126">Request body</span></span>
<span data-ttu-id="610bb-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="610bb-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="610bb-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="610bb-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="610bb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="610bb-129">Property</span></span>|<span data-ttu-id="610bb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="610bb-130">Type</span></span>|<span data-ttu-id="610bb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="610bb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="610bb-132">deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="610bb-132">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="610bb-133">coleção [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="610bb-133">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="610bb-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="610bb-134">Not yet documented</span></span>|
|<span data-ttu-id="610bb-135">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="610bb-135">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="610bb-136">coleção [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="610bb-136">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="610bb-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="610bb-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="610bb-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="610bb-138">Response</span></span>
<span data-ttu-id="610bb-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="610bb-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="610bb-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="610bb-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="610bb-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="610bb-141">Request</span></span>
<span data-ttu-id="610bb-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="610bb-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assign

Content-type: application/json
Content-length: 550

{
  "deviceManagementScriptGroupAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
      "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
      "targetGroupId": "Target Group Id value"
    }
  ],
  "deviceManagementScriptAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
      "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="610bb-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="610bb-143">Response</span></span>
<span data-ttu-id="610bb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="610bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





