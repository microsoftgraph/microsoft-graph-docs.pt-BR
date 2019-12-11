---
title: Criar deviceHealthScriptAssignment
description: Criar um novo objeto deviceHealthScriptAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aada43e65d2d970719d37aa1a5b5f1abdf88f5ba
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945127"
---
# <a name="create-devicehealthscriptassignment"></a><span data-ttu-id="ecf84-103">Criar deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="ecf84-103">Create deviceHealthScriptAssignment</span></span>

> <span data-ttu-id="ecf84-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ecf84-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ecf84-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ecf84-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecf84-106">Criar um novo objeto [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ecf84-106">Create a new [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecf84-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ecf84-107">Prerequisites</span></span>
<span data-ttu-id="ecf84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecf84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecf84-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ecf84-110">Permission type</span></span>|<span data-ttu-id="ecf84-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ecf84-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecf84-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ecf84-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ecf84-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecf84-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ecf84-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ecf84-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecf84-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecf84-115">Not supported.</span></span>|
|<span data-ttu-id="ecf84-116">Application</span><span class="sxs-lookup"><span data-stu-id="ecf84-116">Application</span></span>|<span data-ttu-id="ecf84-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecf84-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecf84-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ecf84-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ecf84-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ecf84-119">Request headers</span></span>
|<span data-ttu-id="ecf84-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ecf84-120">Header</span></span>|<span data-ttu-id="ecf84-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ecf84-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecf84-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ecf84-122">Authorization</span></span>|<span data-ttu-id="ecf84-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecf84-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecf84-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ecf84-124">Accept</span></span>|<span data-ttu-id="ecf84-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ecf84-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecf84-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ecf84-126">Request body</span></span>
<span data-ttu-id="ecf84-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceHealthScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="ecf84-127">In the request body, supply a JSON representation for the deviceHealthScriptAssignment object.</span></span>

<span data-ttu-id="ecf84-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceHealthScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="ecf84-128">The following table shows the properties that are required when you create the deviceHealthScriptAssignment.</span></span>

|<span data-ttu-id="ecf84-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ecf84-129">Property</span></span>|<span data-ttu-id="ecf84-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ecf84-130">Type</span></span>|<span data-ttu-id="ecf84-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecf84-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecf84-132">id</span><span class="sxs-lookup"><span data-stu-id="ecf84-132">id</span></span>|<span data-ttu-id="ecf84-133">String</span><span class="sxs-lookup"><span data-stu-id="ecf84-133">String</span></span>|<span data-ttu-id="ecf84-134">Chave da entidade de atribuição de script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ecf84-134">Key of the device health script assignment entity.</span></span> <span data-ttu-id="ecf84-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ecf84-135">This property is read-only.</span></span>|
|<span data-ttu-id="ecf84-136">destino</span><span class="sxs-lookup"><span data-stu-id="ecf84-136">target</span></span>|[<span data-ttu-id="ecf84-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ecf84-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ecf84-138">O grupo do Azure Active Directory que estamos direcionando o script para</span><span class="sxs-lookup"><span data-stu-id="ecf84-138">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="ecf84-139">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="ecf84-139">runRemediationScript</span></span>|<span data-ttu-id="ecf84-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="ecf84-140">Boolean</span></span>|<span data-ttu-id="ecf84-141">Determinar se queremos executar somente o script de detecção ou executar o script de detecção e o script de correção</span><span class="sxs-lookup"><span data-stu-id="ecf84-141">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="ecf84-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="ecf84-142">runSchedule</span></span>|[<span data-ttu-id="ecf84-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="ecf84-143">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="ecf84-144">Agendamento de execução de script para o grupo de destino</span><span class="sxs-lookup"><span data-stu-id="ecf84-144">Script run schedule for the target group</span></span>|



## <a name="response"></a><span data-ttu-id="ecf84-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecf84-145">Response</span></span>
<span data-ttu-id="ecf84-146">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ecf84-146">If successful, this method returns a `201 Created` response code and a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecf84-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ecf84-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecf84-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ecf84-148">Request</span></span>
<span data-ttu-id="ecf84-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ecf84-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ecf84-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecf84-150">Response</span></span>
<span data-ttu-id="ecf84-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ecf84-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





