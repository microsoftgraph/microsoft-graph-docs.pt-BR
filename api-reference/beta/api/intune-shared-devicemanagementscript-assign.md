---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 385c2230dd6911388f3e357cae508ec5521cd481
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49223903"
---
# <a name="assign-action"></a><span data-ttu-id="3830e-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="3830e-103">assign action</span></span>

<span data-ttu-id="3830e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3830e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3830e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3830e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3830e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3830e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3830e-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3830e-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3830e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3830e-108">Prerequisites</span></span>
<span data-ttu-id="3830e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3830e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3830e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3830e-111">Permission type</span></span>|<span data-ttu-id="3830e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3830e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3830e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3830e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3830e-114">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="3830e-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="3830e-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3830e-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3830e-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3830e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3830e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3830e-117">Not supported.</span></span>|
|<span data-ttu-id="3830e-118">Application</span><span class="sxs-lookup"><span data-stu-id="3830e-118">Application</span></span>||
| <span data-ttu-id="3830e-119">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="3830e-119">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="3830e-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3830e-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3830e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3830e-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="3830e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3830e-122">Request headers</span></span>
|<span data-ttu-id="3830e-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3830e-123">Header</span></span>|<span data-ttu-id="3830e-124">Valor</span><span class="sxs-lookup"><span data-stu-id="3830e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3830e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3830e-125">Authorization</span></span>|<span data-ttu-id="3830e-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3830e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3830e-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3830e-127">Accept</span></span>|<span data-ttu-id="3830e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3830e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3830e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3830e-129">Request body</span></span>
<span data-ttu-id="3830e-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3830e-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3830e-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="3830e-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3830e-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3830e-132">Property</span></span>|<span data-ttu-id="3830e-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="3830e-133">Type</span></span>|<span data-ttu-id="3830e-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="3830e-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3830e-135">deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="3830e-135">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="3830e-136">coleção [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3830e-136">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="3830e-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3830e-137">Not yet documented</span></span>|
|<span data-ttu-id="3830e-138">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="3830e-138">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="3830e-139">coleção [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3830e-139">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="3830e-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3830e-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3830e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3830e-141">Response</span></span>
<span data-ttu-id="3830e-142">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3830e-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3830e-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3830e-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="3830e-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3830e-144">Request</span></span>
<span data-ttu-id="3830e-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3830e-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3830e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="3830e-146">Response</span></span>
<span data-ttu-id="3830e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3830e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







