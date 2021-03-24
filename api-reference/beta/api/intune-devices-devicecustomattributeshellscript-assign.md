---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7d1297d9e40112fc6a05d3df7d3a08d4ae891266
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130753"
---
# <a name="assign-action"></a><span data-ttu-id="ce553-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="ce553-103">assign action</span></span>

<span data-ttu-id="ce553-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce553-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce553-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ce553-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce553-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ce553-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce553-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ce553-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce553-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ce553-108">Prerequisites</span></span>
<span data-ttu-id="ce553-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce553-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce553-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce553-111">Permission type</span></span>|<span data-ttu-id="ce553-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce553-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce553-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce553-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce553-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce553-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ce553-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce553-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce553-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce553-116">Not supported.</span></span>|
|<span data-ttu-id="ce553-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce553-117">Application</span></span>|<span data-ttu-id="ce553-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce553-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce553-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce553-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="ce553-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce553-120">Request headers</span></span>
|<span data-ttu-id="ce553-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ce553-121">Header</span></span>|<span data-ttu-id="ce553-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ce553-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce553-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce553-123">Authorization</span></span>|<span data-ttu-id="ce553-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce553-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce553-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ce553-125">Accept</span></span>|<span data-ttu-id="ce553-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce553-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce553-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce553-127">Request body</span></span>
<span data-ttu-id="ce553-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ce553-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ce553-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ce553-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ce553-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce553-130">Property</span></span>|<span data-ttu-id="ce553-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce553-131">Type</span></span>|<span data-ttu-id="ce553-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce553-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce553-133">deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="ce553-133">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="ce553-134">[Coleção deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ce553-134">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="ce553-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ce553-135">Not yet documented</span></span>|
|<span data-ttu-id="ce553-136">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="ce553-136">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="ce553-137">[Coleção deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ce553-137">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="ce553-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ce553-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ce553-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce553-139">Response</span></span>
<span data-ttu-id="ce553-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ce553-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ce553-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce553-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce553-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce553-142">Request</span></span>
<span data-ttu-id="ce553-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce553-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/assign

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

### <a name="response"></a><span data-ttu-id="ce553-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce553-144">Response</span></span>
<span data-ttu-id="ce553-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce553-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




