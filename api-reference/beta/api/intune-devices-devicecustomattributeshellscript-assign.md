---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 322cd097950c82eea59bdefc748ea4686c75203f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704866"
---
# <a name="assign-action"></a><span data-ttu-id="190a3-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="190a3-103">assign action</span></span>

<span data-ttu-id="190a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="190a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="190a3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="190a3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="190a3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="190a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="190a3-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="190a3-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="190a3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="190a3-108">Prerequisites</span></span>
<span data-ttu-id="190a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="190a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="190a3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="190a3-111">Permission type</span></span>|<span data-ttu-id="190a3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="190a3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="190a3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="190a3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="190a3-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="190a3-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="190a3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="190a3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="190a3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="190a3-116">Not supported.</span></span>|
|<span data-ttu-id="190a3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="190a3-117">Application</span></span>|<span data-ttu-id="190a3-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="190a3-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="190a3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="190a3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="190a3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="190a3-120">Request headers</span></span>
|<span data-ttu-id="190a3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="190a3-121">Header</span></span>|<span data-ttu-id="190a3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="190a3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="190a3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="190a3-123">Authorization</span></span>|<span data-ttu-id="190a3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="190a3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="190a3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="190a3-125">Accept</span></span>|<span data-ttu-id="190a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="190a3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="190a3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="190a3-127">Request body</span></span>
<span data-ttu-id="190a3-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="190a3-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="190a3-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="190a3-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="190a3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="190a3-130">Property</span></span>|<span data-ttu-id="190a3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="190a3-131">Type</span></span>|<span data-ttu-id="190a3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="190a3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="190a3-133">deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="190a3-133">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="190a3-134">coleção [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="190a3-134">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="190a3-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="190a3-135">Not yet documented</span></span>|
|<span data-ttu-id="190a3-136">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="190a3-136">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="190a3-137">coleção [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="190a3-137">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="190a3-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="190a3-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="190a3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="190a3-139">Response</span></span>
<span data-ttu-id="190a3-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="190a3-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="190a3-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="190a3-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="190a3-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="190a3-142">Request</span></span>
<span data-ttu-id="190a3-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="190a3-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/assign

Content-type: application/json
Content-length: 713

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
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="190a3-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="190a3-144">Response</span></span>
<span data-ttu-id="190a3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="190a3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





