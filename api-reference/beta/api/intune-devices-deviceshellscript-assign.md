---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d8c2332c0e0f69ef66dec0d945e8c9f3bb33f7f5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156417"
---
# <a name="assign-action"></a><span data-ttu-id="04e89-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="04e89-103">assign action</span></span>

<span data-ttu-id="04e89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04e89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04e89-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="04e89-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04e89-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04e89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04e89-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="04e89-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04e89-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="04e89-108">Prerequisites</span></span>
<span data-ttu-id="04e89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04e89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04e89-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04e89-111">Permission type</span></span>|<span data-ttu-id="04e89-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="04e89-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04e89-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04e89-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04e89-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04e89-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="04e89-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04e89-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04e89-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04e89-116">Not supported.</span></span>|
|<span data-ttu-id="04e89-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04e89-117">Application</span></span>|<span data-ttu-id="04e89-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04e89-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04e89-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04e89-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="04e89-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04e89-120">Request headers</span></span>
|<span data-ttu-id="04e89-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04e89-121">Header</span></span>|<span data-ttu-id="04e89-122">Valor</span><span class="sxs-lookup"><span data-stu-id="04e89-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04e89-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="04e89-123">Authorization</span></span>|<span data-ttu-id="04e89-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04e89-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04e89-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="04e89-125">Accept</span></span>|<span data-ttu-id="04e89-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04e89-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04e89-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04e89-127">Request body</span></span>
<span data-ttu-id="04e89-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="04e89-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="04e89-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="04e89-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="04e89-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04e89-130">Property</span></span>|<span data-ttu-id="04e89-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="04e89-131">Type</span></span>|<span data-ttu-id="04e89-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="04e89-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04e89-133">deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="04e89-133">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="04e89-134">[Coleção deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="04e89-134">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="04e89-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="04e89-135">Not yet documented</span></span>|
|<span data-ttu-id="04e89-136">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="04e89-136">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="04e89-137">[Coleção deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="04e89-137">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="04e89-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="04e89-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="04e89-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="04e89-139">Response</span></span>
<span data-ttu-id="04e89-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="04e89-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="04e89-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04e89-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="04e89-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04e89-142">Request</span></span>
<span data-ttu-id="04e89-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04e89-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assign

Content-type: application/json
Content-length: 781

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
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="04e89-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="04e89-144">Response</span></span>
<span data-ttu-id="04e89-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04e89-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




