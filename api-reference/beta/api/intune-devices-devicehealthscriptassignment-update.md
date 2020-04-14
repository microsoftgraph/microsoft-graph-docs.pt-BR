---
title: Atualizar deviceHealthScriptAssignment
description: Atualiza as propriedades de um objeto deviceHealthScriptAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 89075571f51cad503041a82af99900caeb5a801f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43380649"
---
# <a name="update-devicehealthscriptassignment"></a><span data-ttu-id="33dcc-103">Atualizar deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="33dcc-103">Update deviceHealthScriptAssignment</span></span>

<span data-ttu-id="33dcc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33dcc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33dcc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="33dcc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33dcc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="33dcc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33dcc-107">Atualiza as propriedades de um objeto [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="33dcc-107">Update the properties of a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33dcc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="33dcc-108">Prerequisites</span></span>
<span data-ttu-id="33dcc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33dcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33dcc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33dcc-111">Permission type</span></span>|<span data-ttu-id="33dcc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="33dcc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33dcc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33dcc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33dcc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="33dcc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="33dcc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33dcc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33dcc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33dcc-116">Not supported.</span></span>|
|<span data-ttu-id="33dcc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33dcc-117">Application</span></span>|<span data-ttu-id="33dcc-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="33dcc-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33dcc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33dcc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="33dcc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33dcc-120">Request headers</span></span>
|<span data-ttu-id="33dcc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33dcc-121">Header</span></span>|<span data-ttu-id="33dcc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="33dcc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33dcc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="33dcc-123">Authorization</span></span>|<span data-ttu-id="33dcc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33dcc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33dcc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="33dcc-125">Accept</span></span>|<span data-ttu-id="33dcc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33dcc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33dcc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33dcc-127">Request body</span></span>
<span data-ttu-id="33dcc-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="33dcc-128">In the request body, supply a JSON representation for the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

<span data-ttu-id="33dcc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).</span><span class="sxs-lookup"><span data-stu-id="33dcc-129">The following table shows the properties that are required when you create the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).</span></span>

|<span data-ttu-id="33dcc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33dcc-130">Property</span></span>|<span data-ttu-id="33dcc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="33dcc-131">Type</span></span>|<span data-ttu-id="33dcc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="33dcc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33dcc-133">id</span><span class="sxs-lookup"><span data-stu-id="33dcc-133">id</span></span>|<span data-ttu-id="33dcc-134">String</span><span class="sxs-lookup"><span data-stu-id="33dcc-134">String</span></span>|<span data-ttu-id="33dcc-135">Chave da entidade de atribuição de script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="33dcc-135">Key of the device health script assignment entity.</span></span> <span data-ttu-id="33dcc-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="33dcc-136">This property is read-only.</span></span>|
|<span data-ttu-id="33dcc-137">destino</span><span class="sxs-lookup"><span data-stu-id="33dcc-137">target</span></span>|[<span data-ttu-id="33dcc-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="33dcc-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="33dcc-139">O grupo do Azure Active Directory que estamos direcionando o script para</span><span class="sxs-lookup"><span data-stu-id="33dcc-139">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="33dcc-140">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="33dcc-140">runRemediationScript</span></span>|<span data-ttu-id="33dcc-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="33dcc-141">Boolean</span></span>|<span data-ttu-id="33dcc-142">Determinar se queremos executar somente o script de detecção ou executar o script de detecção e o script de correção</span><span class="sxs-lookup"><span data-stu-id="33dcc-142">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="33dcc-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="33dcc-143">runSchedule</span></span>|[<span data-ttu-id="33dcc-144">runSchedule</span><span class="sxs-lookup"><span data-stu-id="33dcc-144">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="33dcc-145">Agendamento de execução de script para o grupo de destino</span><span class="sxs-lookup"><span data-stu-id="33dcc-145">Script run schedule for the target group</span></span>|



## <a name="response"></a><span data-ttu-id="33dcc-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="33dcc-146">Response</span></span>
<span data-ttu-id="33dcc-147">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33dcc-147">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33dcc-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33dcc-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="33dcc-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33dcc-149">Request</span></span>
<span data-ttu-id="33dcc-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33dcc-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
Content-type: application/json
Content-length: 277

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "runRemediationScript": true,
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  }
}
```

### <a name="response"></a><span data-ttu-id="33dcc-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="33dcc-151">Response</span></span>
<span data-ttu-id="33dcc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33dcc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 326

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
  "id": "c08c4eb1-4eb1-c08c-b14e-8cc0b14e8cc0",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "runRemediationScript": true,
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  }
}
```



