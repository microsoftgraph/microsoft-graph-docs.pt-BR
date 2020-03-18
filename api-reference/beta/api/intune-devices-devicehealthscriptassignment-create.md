---
title: Criar deviceHealthScriptAssignment
description: Criar um novo objeto deviceHealthScriptAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 54e365b3984bb313f5fa4dd5795f7534a38596d2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42769133"
---
# <a name="create-devicehealthscriptassignment"></a><span data-ttu-id="1efbd-103">Criar deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="1efbd-103">Create deviceHealthScriptAssignment</span></span>

> <span data-ttu-id="1efbd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1efbd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1efbd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1efbd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1efbd-106">Criar um novo objeto [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="1efbd-106">Create a new [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1efbd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1efbd-107">Prerequisites</span></span>
<span data-ttu-id="1efbd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1efbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1efbd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1efbd-110">Permission type</span></span>|<span data-ttu-id="1efbd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1efbd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1efbd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1efbd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1efbd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1efbd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1efbd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1efbd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1efbd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1efbd-115">Not supported.</span></span>|
|<span data-ttu-id="1efbd-116">Application</span><span class="sxs-lookup"><span data-stu-id="1efbd-116">Application</span></span>|<span data-ttu-id="1efbd-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1efbd-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1efbd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1efbd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1efbd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1efbd-119">Request headers</span></span>
|<span data-ttu-id="1efbd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1efbd-120">Header</span></span>|<span data-ttu-id="1efbd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1efbd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1efbd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1efbd-122">Authorization</span></span>|<span data-ttu-id="1efbd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1efbd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1efbd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1efbd-124">Accept</span></span>|<span data-ttu-id="1efbd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1efbd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1efbd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1efbd-126">Request body</span></span>
<span data-ttu-id="1efbd-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceHealthScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="1efbd-127">In the request body, supply a JSON representation for the deviceHealthScriptAssignment object.</span></span>

<span data-ttu-id="1efbd-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceHealthScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="1efbd-128">The following table shows the properties that are required when you create the deviceHealthScriptAssignment.</span></span>

|<span data-ttu-id="1efbd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1efbd-129">Property</span></span>|<span data-ttu-id="1efbd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1efbd-130">Type</span></span>|<span data-ttu-id="1efbd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1efbd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1efbd-132">id</span><span class="sxs-lookup"><span data-stu-id="1efbd-132">id</span></span>|<span data-ttu-id="1efbd-133">String</span><span class="sxs-lookup"><span data-stu-id="1efbd-133">String</span></span>|<span data-ttu-id="1efbd-134">Chave da entidade de atribuição de script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1efbd-134">Key of the device health script assignment entity.</span></span> <span data-ttu-id="1efbd-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1efbd-135">This property is read-only.</span></span>|
|<span data-ttu-id="1efbd-136">destino</span><span class="sxs-lookup"><span data-stu-id="1efbd-136">target</span></span>|[<span data-ttu-id="1efbd-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1efbd-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1efbd-138">O grupo do Azure Active Directory que estamos direcionando o script para</span><span class="sxs-lookup"><span data-stu-id="1efbd-138">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="1efbd-139">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="1efbd-139">runRemediationScript</span></span>|<span data-ttu-id="1efbd-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="1efbd-140">Boolean</span></span>|<span data-ttu-id="1efbd-141">Determinar se queremos executar somente o script de detecção ou executar o script de detecção e o script de correção</span><span class="sxs-lookup"><span data-stu-id="1efbd-141">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="1efbd-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="1efbd-142">runSchedule</span></span>|[<span data-ttu-id="1efbd-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="1efbd-143">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="1efbd-144">Agendamento de execução de script para o grupo de destino</span><span class="sxs-lookup"><span data-stu-id="1efbd-144">Script run schedule for the target group</span></span>|



## <a name="response"></a><span data-ttu-id="1efbd-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1efbd-145">Response</span></span>
<span data-ttu-id="1efbd-146">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1efbd-146">If successful, this method returns a `201 Created` response code and a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1efbd-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1efbd-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="1efbd-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1efbd-148">Request</span></span>
<span data-ttu-id="1efbd-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1efbd-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
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

### <a name="response"></a><span data-ttu-id="1efbd-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="1efbd-150">Response</span></span>
<span data-ttu-id="1efbd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1efbd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




