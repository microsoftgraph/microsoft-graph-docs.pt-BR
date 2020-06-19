---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd35d0edabdd0f20e5a3c567858159fdf5dd8de6
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792419"
---
# <a name="assign-action"></a><span data-ttu-id="3be9c-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="3be9c-103">assign action</span></span>

<span data-ttu-id="3be9c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3be9c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3be9c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3be9c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3be9c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3be9c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3be9c-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3be9c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3be9c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3be9c-108">Prerequisites</span></span>
<span data-ttu-id="3be9c-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="3be9c-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3be9c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3be9c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3be9c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3be9c-111">Permission type</span></span>|<span data-ttu-id="3be9c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3be9c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3be9c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3be9c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3be9c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3be9c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3be9c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3be9c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3be9c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3be9c-116">Not supported.</span></span>|
|<span data-ttu-id="3be9c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3be9c-117">Application</span></span>|<span data-ttu-id="3be9c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3be9c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3be9c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3be9c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="3be9c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3be9c-120">Request headers</span></span>
|<span data-ttu-id="3be9c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3be9c-121">Header</span></span>|<span data-ttu-id="3be9c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3be9c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3be9c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3be9c-123">Authorization</span></span>|<span data-ttu-id="3be9c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3be9c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3be9c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3be9c-125">Accept</span></span>|<span data-ttu-id="3be9c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3be9c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3be9c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3be9c-127">Request body</span></span>
<span data-ttu-id="3be9c-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3be9c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3be9c-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="3be9c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3be9c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3be9c-130">Property</span></span>|<span data-ttu-id="3be9c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3be9c-131">Type</span></span>|<span data-ttu-id="3be9c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3be9c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3be9c-133">deviceHealthScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="3be9c-133">deviceHealthScriptAssignments</span></span>|<span data-ttu-id="3be9c-134">coleção [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3be9c-134">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="3be9c-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3be9c-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3be9c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3be9c-136">Response</span></span>
<span data-ttu-id="3be9c-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3be9c-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3be9c-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3be9c-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="3be9c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3be9c-139">Request</span></span>
<span data-ttu-id="3be9c-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3be9c-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assign

Content-type: application/json
Content-length: 688

{
  "deviceHealthScriptAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
      "id": "c08c4eb1-4eb1-c08c-b14e-8cc0b14e8cc0",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
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

### <a name="response"></a><span data-ttu-id="3be9c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3be9c-141">Response</span></span>
<span data-ttu-id="3be9c-142">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="3be9c-142">Here is an example of the response.</span></span> <span data-ttu-id="3be9c-143">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="3be9c-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3be9c-144">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="3be9c-144">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



