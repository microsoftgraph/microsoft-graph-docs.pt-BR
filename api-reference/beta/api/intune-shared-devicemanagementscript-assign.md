---
title: atribuir ação
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 084f1533cb2e4e2305b13341abc2f213b3940d7c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800988"
---
# <a name="assign-action"></a><span data-ttu-id="be806-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="be806-103">assign action</span></span>

> <span data-ttu-id="be806-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="be806-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be806-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="be806-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be806-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="be806-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be806-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="be806-107">Prerequisites</span></span>
<span data-ttu-id="be806-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be806-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be806-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be806-110">Permission type</span></span>|<span data-ttu-id="be806-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="be806-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be806-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be806-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="be806-113">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="be806-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="be806-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be806-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="be806-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be806-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be806-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be806-116">Not supported.</span></span>|
|<span data-ttu-id="be806-117">Application</span><span class="sxs-lookup"><span data-stu-id="be806-117">Application</span></span>||
| <span data-ttu-id="be806-118">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="be806-118">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="be806-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be806-119">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="be806-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be806-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="be806-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be806-121">Request headers</span></span>
|<span data-ttu-id="be806-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="be806-122">Header</span></span>|<span data-ttu-id="be806-123">Valor</span><span class="sxs-lookup"><span data-stu-id="be806-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be806-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="be806-124">Authorization</span></span>|<span data-ttu-id="be806-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be806-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be806-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="be806-126">Accept</span></span>|<span data-ttu-id="be806-127">application/json</span><span class="sxs-lookup"><span data-stu-id="be806-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be806-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be806-128">Request body</span></span>
<span data-ttu-id="be806-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="be806-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="be806-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="be806-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="be806-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be806-131">Property</span></span>|<span data-ttu-id="be806-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="be806-132">Type</span></span>|<span data-ttu-id="be806-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="be806-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be806-134">deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="be806-134">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="be806-135">coleção [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="be806-135">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="be806-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="be806-136">Not yet documented</span></span>|
|<span data-ttu-id="be806-137">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="be806-137">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="be806-138">coleção [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="be806-138">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="be806-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="be806-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="be806-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="be806-140">Response</span></span>
<span data-ttu-id="be806-141">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="be806-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="be806-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be806-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="be806-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be806-143">Request</span></span>
<span data-ttu-id="be806-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be806-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign

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

### <a name="response"></a><span data-ttu-id="be806-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="be806-145">Response</span></span>
<span data-ttu-id="be806-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be806-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







