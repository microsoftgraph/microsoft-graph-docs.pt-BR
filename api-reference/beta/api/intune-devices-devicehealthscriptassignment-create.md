---
title: Criar deviceHealthScriptAssignment
description: Criar um novo objeto deviceHealthScriptAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 605b21c3de1a7408224c3544e6f3bbb7d4adf04f
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792412"
---
# <a name="create-devicehealthscriptassignment"></a><span data-ttu-id="773d8-103">Criar deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="773d8-103">Create deviceHealthScriptAssignment</span></span>

<span data-ttu-id="773d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="773d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="773d8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="773d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="773d8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="773d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="773d8-107">Criar um novo objeto [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="773d8-107">Create a new [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="773d8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="773d8-108">Prerequisites</span></span>
<span data-ttu-id="773d8-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="773d8-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="773d8-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="773d8-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="773d8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="773d8-111">Permission type</span></span>|<span data-ttu-id="773d8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="773d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="773d8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="773d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="773d8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="773d8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="773d8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="773d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="773d8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="773d8-116">Not supported.</span></span>|
|<span data-ttu-id="773d8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="773d8-117">Application</span></span>|<span data-ttu-id="773d8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="773d8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="773d8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="773d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="773d8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="773d8-120">Request headers</span></span>
|<span data-ttu-id="773d8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="773d8-121">Header</span></span>|<span data-ttu-id="773d8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="773d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="773d8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="773d8-123">Authorization</span></span>|<span data-ttu-id="773d8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="773d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="773d8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="773d8-125">Accept</span></span>|<span data-ttu-id="773d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="773d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="773d8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="773d8-127">Request body</span></span>
<span data-ttu-id="773d8-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceHealthScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="773d8-128">In the request body, supply a JSON representation for the deviceHealthScriptAssignment object.</span></span>

<span data-ttu-id="773d8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceHealthScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="773d8-129">The following table shows the properties that are required when you create the deviceHealthScriptAssignment.</span></span>

|<span data-ttu-id="773d8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="773d8-130">Property</span></span>|<span data-ttu-id="773d8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="773d8-131">Type</span></span>|<span data-ttu-id="773d8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="773d8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="773d8-133">id</span><span class="sxs-lookup"><span data-stu-id="773d8-133">id</span></span>|<span data-ttu-id="773d8-134">String</span><span class="sxs-lookup"><span data-stu-id="773d8-134">String</span></span>|<span data-ttu-id="773d8-135">Chave da entidade de atribuição de script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="773d8-135">Key of the device health script assignment entity.</span></span> <span data-ttu-id="773d8-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="773d8-136">This property is read-only.</span></span>|
|<span data-ttu-id="773d8-137">destino</span><span class="sxs-lookup"><span data-stu-id="773d8-137">target</span></span>|[<span data-ttu-id="773d8-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="773d8-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="773d8-139">O grupo do Azure Active Directory que estamos direcionando o script para</span><span class="sxs-lookup"><span data-stu-id="773d8-139">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="773d8-140">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="773d8-140">runRemediationScript</span></span>|<span data-ttu-id="773d8-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="773d8-141">Boolean</span></span>|<span data-ttu-id="773d8-142">Determinar se queremos executar somente o script de detecção ou executar o script de detecção e o script de correção</span><span class="sxs-lookup"><span data-stu-id="773d8-142">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="773d8-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="773d8-143">runSchedule</span></span>|[<span data-ttu-id="773d8-144">deviceHealthScriptRunSchedule</span><span class="sxs-lookup"><span data-stu-id="773d8-144">deviceHealthScriptRunSchedule</span></span>](../resources/intune-devices-devicehealthscriptrunschedule.md)|<span data-ttu-id="773d8-145">Agendamento de execução de script para o grupo de destino</span><span class="sxs-lookup"><span data-stu-id="773d8-145">Script run schedule for the target group</span></span>|



## <a name="response"></a><span data-ttu-id="773d8-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="773d8-146">Response</span></span>
<span data-ttu-id="773d8-147">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="773d8-147">If successful, this method returns a `201 Created` response code and a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="773d8-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="773d8-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="773d8-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="773d8-149">Request</span></span>
<span data-ttu-id="773d8-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="773d8-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
Content-type: application/json
Content-length: 526

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
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
```

### <a name="response"></a><span data-ttu-id="773d8-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="773d8-151">Response</span></span>
<span data-ttu-id="773d8-152">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="773d8-152">Here is an example of the response.</span></span> <span data-ttu-id="773d8-153">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="773d8-153">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="773d8-154">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="773d8-154">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 575

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
```



