---
title: Criar deviceHealthScriptAssignment
description: Criar um novo objeto deviceHealthScriptAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4d0ad1e7ac64b1f849a2e95a427ad41f8571138e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732857"
---
# <a name="create-devicehealthscriptassignment"></a><span data-ttu-id="a5e9e-103">Criar deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="a5e9e-103">Create deviceHealthScriptAssignment</span></span>

<span data-ttu-id="a5e9e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5e9e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5e9e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a5e9e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5e9e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a5e9e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5e9e-107">Criar um novo objeto [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a5e9e-107">Create a new [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5e9e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a5e9e-108">Prerequisites</span></span>
<span data-ttu-id="a5e9e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5e9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5e9e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5e9e-111">Permission type</span></span>|<span data-ttu-id="a5e9e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a5e9e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5e9e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5e9e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a5e9e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5e9e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a5e9e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5e9e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5e9e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5e9e-116">Not supported.</span></span>|
|<span data-ttu-id="a5e9e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5e9e-117">Application</span></span>|<span data-ttu-id="a5e9e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5e9e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5e9e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5e9e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a5e9e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e9e-120">Request headers</span></span>
|<span data-ttu-id="a5e9e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a5e9e-121">Header</span></span>|<span data-ttu-id="a5e9e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a5e9e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5e9e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5e9e-123">Authorization</span></span>|<span data-ttu-id="a5e9e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5e9e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5e9e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a5e9e-125">Accept</span></span>|<span data-ttu-id="a5e9e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5e9e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5e9e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e9e-127">Request body</span></span>
<span data-ttu-id="a5e9e-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceHealthScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="a5e9e-128">In the request body, supply a JSON representation for the deviceHealthScriptAssignment object.</span></span>

<span data-ttu-id="a5e9e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceHealthScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="a5e9e-129">The following table shows the properties that are required when you create the deviceHealthScriptAssignment.</span></span>

|<span data-ttu-id="a5e9e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5e9e-130">Property</span></span>|<span data-ttu-id="a5e9e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5e9e-131">Type</span></span>|<span data-ttu-id="a5e9e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5e9e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5e9e-133">id</span><span class="sxs-lookup"><span data-stu-id="a5e9e-133">id</span></span>|<span data-ttu-id="a5e9e-134">String</span><span class="sxs-lookup"><span data-stu-id="a5e9e-134">String</span></span>|<span data-ttu-id="a5e9e-135">Chave da entidade de atribuição de script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a5e9e-135">Key of the device health script assignment entity.</span></span> <span data-ttu-id="a5e9e-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a5e9e-136">This property is read-only.</span></span>|
|<span data-ttu-id="a5e9e-137">destino</span><span class="sxs-lookup"><span data-stu-id="a5e9e-137">target</span></span>|[<span data-ttu-id="a5e9e-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a5e9e-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a5e9e-139">O grupo do Azure Active Directory que estamos direcionando o script para</span><span class="sxs-lookup"><span data-stu-id="a5e9e-139">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="a5e9e-140">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="a5e9e-140">runRemediationScript</span></span>|<span data-ttu-id="a5e9e-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="a5e9e-141">Boolean</span></span>|<span data-ttu-id="a5e9e-142">Determinar se queremos executar somente o script de detecção ou executar o script de detecção e o script de correção</span><span class="sxs-lookup"><span data-stu-id="a5e9e-142">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="a5e9e-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="a5e9e-143">runSchedule</span></span>|[<span data-ttu-id="a5e9e-144">deviceHealthScriptRunSchedule</span><span class="sxs-lookup"><span data-stu-id="a5e9e-144">deviceHealthScriptRunSchedule</span></span>](../resources/intune-devices-devicehealthscriptrunschedule.md)|<span data-ttu-id="a5e9e-145">Agendamento de execução de script para o grupo de destino</span><span class="sxs-lookup"><span data-stu-id="a5e9e-145">Script run schedule for the target group</span></span>|



## <a name="response"></a><span data-ttu-id="a5e9e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5e9e-146">Response</span></span>
<span data-ttu-id="a5e9e-147">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5e9e-147">If successful, this method returns a `201 Created` response code and a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5e9e-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5e9e-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5e9e-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e9e-149">Request</span></span>
<span data-ttu-id="a5e9e-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5e9e-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a5e9e-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5e9e-151">Response</span></span>
<span data-ttu-id="a5e9e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5e9e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





