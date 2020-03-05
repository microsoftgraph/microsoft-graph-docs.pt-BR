---
title: atribuir ação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5cb968e0663a508a589456ce42567168cb73ba78
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469164"
---
# <a name="assign-action"></a><span data-ttu-id="45258-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="45258-103">assign action</span></span>

<span data-ttu-id="45258-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="45258-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45258-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45258-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45258-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45258-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45258-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="45258-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45258-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45258-108">Prerequisites</span></span>
<span data-ttu-id="45258-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45258-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45258-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45258-111">Permission type</span></span>|<span data-ttu-id="45258-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="45258-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45258-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45258-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45258-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45258-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="45258-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45258-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45258-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45258-116">Not supported.</span></span>|
|<span data-ttu-id="45258-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45258-117">Application</span></span>|<span data-ttu-id="45258-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45258-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45258-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45258-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="45258-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45258-120">Request headers</span></span>
|<span data-ttu-id="45258-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45258-121">Header</span></span>|<span data-ttu-id="45258-122">Valor</span><span class="sxs-lookup"><span data-stu-id="45258-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45258-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="45258-123">Authorization</span></span>|<span data-ttu-id="45258-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45258-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45258-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="45258-125">Accept</span></span>|<span data-ttu-id="45258-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45258-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45258-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45258-127">Request body</span></span>
<span data-ttu-id="45258-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="45258-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="45258-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="45258-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="45258-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45258-130">Property</span></span>|<span data-ttu-id="45258-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="45258-131">Type</span></span>|<span data-ttu-id="45258-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="45258-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45258-133">deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="45258-133">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="45258-134">coleção [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="45258-134">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="45258-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="45258-135">Not yet documented</span></span>|
|<span data-ttu-id="45258-136">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="45258-136">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="45258-137">coleção [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="45258-137">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="45258-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="45258-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="45258-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="45258-139">Response</span></span>
<span data-ttu-id="45258-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="45258-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="45258-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45258-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="45258-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45258-142">Request</span></span>
<span data-ttu-id="45258-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45258-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="45258-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="45258-144">Response</span></span>
<span data-ttu-id="45258-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45258-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





