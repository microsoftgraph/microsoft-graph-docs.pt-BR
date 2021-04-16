---
title: atribuir ação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 75b41fa478201b1064b20807e786d65c3348e0e9
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867823"
---
# <a name="assign-action"></a><span data-ttu-id="8edf2-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="8edf2-103">assign action</span></span>

<span data-ttu-id="8edf2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8edf2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8edf2-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8edf2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8edf2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8edf2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8edf2-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8edf2-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8edf2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8edf2-108">Prerequisites</span></span>
<span data-ttu-id="8edf2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8edf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8edf2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8edf2-111">Permission type</span></span>|<span data-ttu-id="8edf2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8edf2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8edf2-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8edf2-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8edf2-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="8edf2-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8edf2-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8edf2-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8edf2-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8edf2-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8edf2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8edf2-117">Not supported.</span></span>|
|<span data-ttu-id="8edf2-118">Application</span><span class="sxs-lookup"><span data-stu-id="8edf2-118">Application</span></span>||
| <span data-ttu-id="8edf2-119">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="8edf2-119">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8edf2-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8edf2-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8edf2-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8edf2-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="8edf2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8edf2-122">Request headers</span></span>
|<span data-ttu-id="8edf2-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8edf2-123">Header</span></span>|<span data-ttu-id="8edf2-124">Valor</span><span class="sxs-lookup"><span data-stu-id="8edf2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8edf2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="8edf2-125">Authorization</span></span>|<span data-ttu-id="8edf2-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8edf2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8edf2-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8edf2-127">Accept</span></span>|<span data-ttu-id="8edf2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8edf2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8edf2-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8edf2-129">Request body</span></span>
<span data-ttu-id="8edf2-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="8edf2-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8edf2-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="8edf2-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8edf2-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8edf2-132">Property</span></span>|<span data-ttu-id="8edf2-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="8edf2-133">Type</span></span>|<span data-ttu-id="8edf2-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="8edf2-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8edf2-135">deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="8edf2-135">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="8edf2-136">[Coleção deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8edf2-136">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="8edf2-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8edf2-137">Not yet documented</span></span>|
|<span data-ttu-id="8edf2-138">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="8edf2-138">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="8edf2-139">[Coleção deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8edf2-139">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="8edf2-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8edf2-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8edf2-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8edf2-141">Response</span></span>
<span data-ttu-id="8edf2-142">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8edf2-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8edf2-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8edf2-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="8edf2-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8edf2-144">Request</span></span>
<span data-ttu-id="8edf2-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8edf2-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8edf2-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="8edf2-146">Response</span></span>
<span data-ttu-id="8edf2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8edf2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







