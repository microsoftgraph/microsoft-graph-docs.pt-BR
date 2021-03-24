---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e77be56361eb85568fb0c959c696bd6c2351b068
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146444"
---
# <a name="assign-action"></a><span data-ttu-id="92012-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="92012-103">assign action</span></span>

<span data-ttu-id="92012-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92012-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92012-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="92012-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92012-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92012-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92012-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="92012-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92012-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92012-108">Prerequisites</span></span>
<span data-ttu-id="92012-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92012-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92012-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92012-111">Permission type</span></span>|<span data-ttu-id="92012-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92012-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92012-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92012-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92012-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92012-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="92012-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92012-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92012-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92012-116">Not supported.</span></span>|
|<span data-ttu-id="92012-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92012-117">Application</span></span>|<span data-ttu-id="92012-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92012-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92012-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92012-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="92012-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92012-120">Request headers</span></span>
|<span data-ttu-id="92012-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92012-121">Header</span></span>|<span data-ttu-id="92012-122">Valor</span><span class="sxs-lookup"><span data-stu-id="92012-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92012-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="92012-123">Authorization</span></span>|<span data-ttu-id="92012-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92012-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92012-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92012-125">Accept</span></span>|<span data-ttu-id="92012-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92012-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92012-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92012-127">Request body</span></span>
<span data-ttu-id="92012-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="92012-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="92012-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="92012-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="92012-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92012-130">Property</span></span>|<span data-ttu-id="92012-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="92012-131">Type</span></span>|<span data-ttu-id="92012-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="92012-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92012-133">deviceHealthScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="92012-133">deviceHealthScriptAssignments</span></span>|<span data-ttu-id="92012-134">[Coleção deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="92012-134">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="92012-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="92012-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="92012-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="92012-136">Response</span></span>
<span data-ttu-id="92012-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="92012-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="92012-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92012-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="92012-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92012-139">Request</span></span>
<span data-ttu-id="92012-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92012-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assign

Content-type: application/json
Content-length: 756

{
  "deviceHealthScriptAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
      "id": "c08c4eb1-4eb1-c08c-b14e-8cc0b14e8cc0",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      },
      "runRemediationScript": true,
      "runSchedule": {
        "@odata.type": "microsoft.graph.deviceHealthScriptDailySchedule",
        "interval": 8,
        "useUtc": true,
        "time": "11:58:36.2550000"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="92012-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="92012-141">Response</span></span>
<span data-ttu-id="92012-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92012-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




