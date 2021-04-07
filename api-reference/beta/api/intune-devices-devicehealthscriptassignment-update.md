---
title: Atualizar deviceHealthScriptAssignment
description: Atualize as propriedades de um objeto deviceHealthScriptAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 93909516b037e7545716156920dfec7a089cebca
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610001"
---
# <a name="update-devicehealthscriptassignment"></a><span data-ttu-id="085ec-103">Atualizar deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="085ec-103">Update deviceHealthScriptAssignment</span></span>

<span data-ttu-id="085ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="085ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="085ec-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="085ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="085ec-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="085ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="085ec-107">Atualize as propriedades de um [objeto deviceHealthScriptAssignment.](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="085ec-107">Update the properties of a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="085ec-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="085ec-108">Prerequisites</span></span>
<span data-ttu-id="085ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="085ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="085ec-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="085ec-111">Permission type</span></span>|<span data-ttu-id="085ec-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="085ec-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="085ec-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="085ec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="085ec-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="085ec-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="085ec-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="085ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="085ec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="085ec-116">Not supported.</span></span>|
|<span data-ttu-id="085ec-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="085ec-117">Application</span></span>|<span data-ttu-id="085ec-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="085ec-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="085ec-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="085ec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assignments/{deviceHealthScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="085ec-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="085ec-120">Request headers</span></span>
|<span data-ttu-id="085ec-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="085ec-121">Header</span></span>|<span data-ttu-id="085ec-122">Valor</span><span class="sxs-lookup"><span data-stu-id="085ec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="085ec-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="085ec-123">Authorization</span></span>|<span data-ttu-id="085ec-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="085ec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="085ec-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="085ec-125">Accept</span></span>|<span data-ttu-id="085ec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="085ec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="085ec-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="085ec-127">Request body</span></span>
<span data-ttu-id="085ec-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceHealthScriptAssignment.](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="085ec-128">In the request body, supply a JSON representation for the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

<span data-ttu-id="085ec-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).</span><span class="sxs-lookup"><span data-stu-id="085ec-129">The following table shows the properties that are required when you create the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).</span></span>

|<span data-ttu-id="085ec-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="085ec-130">Property</span></span>|<span data-ttu-id="085ec-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="085ec-131">Type</span></span>|<span data-ttu-id="085ec-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="085ec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="085ec-133">id</span><span class="sxs-lookup"><span data-stu-id="085ec-133">id</span></span>|<span data-ttu-id="085ec-134">String</span><span class="sxs-lookup"><span data-stu-id="085ec-134">String</span></span>|<span data-ttu-id="085ec-135">Chave da entidade de atribuição de script de saúde do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="085ec-135">Key of the device health script assignment entity.</span></span> <span data-ttu-id="085ec-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="085ec-136">This property is read-only.</span></span>|
|<span data-ttu-id="085ec-137">destino</span><span class="sxs-lookup"><span data-stu-id="085ec-137">target</span></span>|[<span data-ttu-id="085ec-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="085ec-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="085ec-139">O grupo do Azure Active Directory para o qual estamos direcionando o script</span><span class="sxs-lookup"><span data-stu-id="085ec-139">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="085ec-140">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="085ec-140">runRemediationScript</span></span>|<span data-ttu-id="085ec-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="085ec-141">Boolean</span></span>|<span data-ttu-id="085ec-142">Determinar se queremos executar somente script de detecção ou executar script de detecção e script de correção</span><span class="sxs-lookup"><span data-stu-id="085ec-142">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="085ec-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="085ec-143">runSchedule</span></span>|[<span data-ttu-id="085ec-144">deviceHealthScriptRunSchedule</span><span class="sxs-lookup"><span data-stu-id="085ec-144">deviceHealthScriptRunSchedule</span></span>](../resources/intune-devices-devicehealthscriptrunschedule.md)|<span data-ttu-id="085ec-145">Agenda de executar scripts para o grupo de destino</span><span class="sxs-lookup"><span data-stu-id="085ec-145">Script run schedule for the target group</span></span>|



## <a name="response"></a><span data-ttu-id="085ec-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="085ec-146">Response</span></span>
<span data-ttu-id="085ec-147">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="085ec-147">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="085ec-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="085ec-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="085ec-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="085ec-149">Request</span></span>
<span data-ttu-id="085ec-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="085ec-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="085ec-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="085ec-151">Response</span></span>
<span data-ttu-id="085ec-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="085ec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




