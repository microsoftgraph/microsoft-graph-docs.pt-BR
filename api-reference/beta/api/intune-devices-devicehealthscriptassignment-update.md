---
title: Atualizar deviceHealthScriptAssignment
description: Atualizar as propriedades de um objeto deviceHealthScriptAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1f391d3d829ca548fb1226307e836e1a8a7ed73e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159693"
---
# <a name="update-devicehealthscriptassignment"></a><span data-ttu-id="e7bcd-103">Atualizar deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="e7bcd-103">Update deviceHealthScriptAssignment</span></span>

<span data-ttu-id="e7bcd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7bcd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7bcd-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e7bcd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7bcd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e7bcd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7bcd-107">Atualizar as propriedades de um [objeto deviceHealthScriptAssignment.](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e7bcd-107">Update the properties of a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7bcd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7bcd-108">Prerequisites</span></span>
<span data-ttu-id="e7bcd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7bcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7bcd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7bcd-111">Permission type</span></span>|<span data-ttu-id="e7bcd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e7bcd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7bcd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7bcd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7bcd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7bcd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e7bcd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7bcd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7bcd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7bcd-116">Not supported.</span></span>|
|<span data-ttu-id="e7bcd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7bcd-117">Application</span></span>|<span data-ttu-id="e7bcd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7bcd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7bcd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7bcd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assignments/{deviceHealthScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e7bcd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7bcd-120">Request headers</span></span>
|<span data-ttu-id="e7bcd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7bcd-121">Header</span></span>|<span data-ttu-id="e7bcd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e7bcd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7bcd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7bcd-123">Authorization</span></span>|<span data-ttu-id="e7bcd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7bcd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7bcd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e7bcd-125">Accept</span></span>|<span data-ttu-id="e7bcd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7bcd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7bcd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7bcd-127">Request body</span></span>
<span data-ttu-id="e7bcd-128">No corpo da solicitação, fornece uma representação JSON do [objeto deviceHealthScriptAssignment.](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e7bcd-128">In the request body, supply a JSON representation for the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

<span data-ttu-id="e7bcd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e7bcd-129">The following table shows the properties that are required when you create the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).</span></span>

|<span data-ttu-id="e7bcd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7bcd-130">Property</span></span>|<span data-ttu-id="e7bcd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7bcd-131">Type</span></span>|<span data-ttu-id="e7bcd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7bcd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7bcd-133">id</span><span class="sxs-lookup"><span data-stu-id="e7bcd-133">id</span></span>|<span data-ttu-id="e7bcd-134">String</span><span class="sxs-lookup"><span data-stu-id="e7bcd-134">String</span></span>|<span data-ttu-id="e7bcd-135">Chave da entidade de atribuição de script de saúde do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e7bcd-135">Key of the device health script assignment entity.</span></span> <span data-ttu-id="e7bcd-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7bcd-136">This property is read-only.</span></span>|
|<span data-ttu-id="e7bcd-137">destino</span><span class="sxs-lookup"><span data-stu-id="e7bcd-137">target</span></span>|[<span data-ttu-id="e7bcd-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e7bcd-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e7bcd-139">O grupo do Azure Active Directory para o qual estamos direcionando o script</span><span class="sxs-lookup"><span data-stu-id="e7bcd-139">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="e7bcd-140">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="e7bcd-140">runRemediationScript</span></span>|<span data-ttu-id="e7bcd-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bcd-141">Boolean</span></span>|<span data-ttu-id="e7bcd-142">Determinar se desejamos executar apenas o script de detecção ou executar o script de detecção e o script de correção</span><span class="sxs-lookup"><span data-stu-id="e7bcd-142">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="e7bcd-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="e7bcd-143">runSchedule</span></span>|[<span data-ttu-id="e7bcd-144">deviceHealthScriptRunSchedule</span><span class="sxs-lookup"><span data-stu-id="e7bcd-144">deviceHealthScriptRunSchedule</span></span>](../resources/intune-devices-devicehealthscriptrunschedule.md)|<span data-ttu-id="e7bcd-145">Cronograma de executar scripts para o grupo de destino</span><span class="sxs-lookup"><span data-stu-id="e7bcd-145">Script run schedule for the target group</span></span>|



## <a name="response"></a><span data-ttu-id="e7bcd-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7bcd-146">Response</span></span>
<span data-ttu-id="e7bcd-147">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7bcd-147">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7bcd-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7bcd-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7bcd-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7bcd-149">Request</span></span>
<span data-ttu-id="e7bcd-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7bcd-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
Content-type: application/json
Content-length: 590

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
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
```

### <a name="response"></a><span data-ttu-id="e7bcd-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7bcd-151">Response</span></span>
<span data-ttu-id="e7bcd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7bcd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 639

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
```




