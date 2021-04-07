---
title: Criar deviceHealthScriptAssignment
description: Crie um novo objeto deviceHealthScriptAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c9cd04a6cb2bbc1a2b9cf103349cca40d49368a7
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611128"
---
# <a name="create-devicehealthscriptassignment"></a><span data-ttu-id="6882c-103">Criar deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="6882c-103">Create deviceHealthScriptAssignment</span></span>

<span data-ttu-id="6882c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6882c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6882c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6882c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6882c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6882c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6882c-107">Crie um novo [objeto deviceHealthScriptAssignment.](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6882c-107">Create a new [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6882c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6882c-108">Prerequisites</span></span>
<span data-ttu-id="6882c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6882c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6882c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6882c-111">Permission type</span></span>|<span data-ttu-id="6882c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6882c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6882c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6882c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6882c-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6882c-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6882c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6882c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6882c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6882c-116">Not supported.</span></span>|
|<span data-ttu-id="6882c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6882c-117">Application</span></span>|<span data-ttu-id="6882c-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6882c-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6882c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6882c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="6882c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6882c-120">Request headers</span></span>
|<span data-ttu-id="6882c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6882c-121">Header</span></span>|<span data-ttu-id="6882c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6882c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6882c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6882c-123">Authorization</span></span>|<span data-ttu-id="6882c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6882c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6882c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6882c-125">Accept</span></span>|<span data-ttu-id="6882c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6882c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6882c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6882c-127">Request body</span></span>
<span data-ttu-id="6882c-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceHealthScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="6882c-128">In the request body, supply a JSON representation for the deviceHealthScriptAssignment object.</span></span>

<span data-ttu-id="6882c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceHealthScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="6882c-129">The following table shows the properties that are required when you create the deviceHealthScriptAssignment.</span></span>

|<span data-ttu-id="6882c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6882c-130">Property</span></span>|<span data-ttu-id="6882c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6882c-131">Type</span></span>|<span data-ttu-id="6882c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6882c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6882c-133">id</span><span class="sxs-lookup"><span data-stu-id="6882c-133">id</span></span>|<span data-ttu-id="6882c-134">String</span><span class="sxs-lookup"><span data-stu-id="6882c-134">String</span></span>|<span data-ttu-id="6882c-135">Chave da entidade de atribuição de script de saúde do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6882c-135">Key of the device health script assignment entity.</span></span> <span data-ttu-id="6882c-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6882c-136">This property is read-only.</span></span>|
|<span data-ttu-id="6882c-137">destino</span><span class="sxs-lookup"><span data-stu-id="6882c-137">target</span></span>|[<span data-ttu-id="6882c-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6882c-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6882c-139">O grupo do Azure Active Directory para o qual estamos direcionando o script</span><span class="sxs-lookup"><span data-stu-id="6882c-139">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="6882c-140">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="6882c-140">runRemediationScript</span></span>|<span data-ttu-id="6882c-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="6882c-141">Boolean</span></span>|<span data-ttu-id="6882c-142">Determinar se queremos executar somente script de detecção ou executar script de detecção e script de correção</span><span class="sxs-lookup"><span data-stu-id="6882c-142">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="6882c-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="6882c-143">runSchedule</span></span>|[<span data-ttu-id="6882c-144">deviceHealthScriptRunSchedule</span><span class="sxs-lookup"><span data-stu-id="6882c-144">deviceHealthScriptRunSchedule</span></span>](../resources/intune-devices-devicehealthscriptrunschedule.md)|<span data-ttu-id="6882c-145">Agenda de executar scripts para o grupo de destino</span><span class="sxs-lookup"><span data-stu-id="6882c-145">Script run schedule for the target group</span></span>|



## <a name="response"></a><span data-ttu-id="6882c-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="6882c-146">Response</span></span>
<span data-ttu-id="6882c-147">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6882c-147">If successful, this method returns a `201 Created` response code and a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6882c-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6882c-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="6882c-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6882c-149">Request</span></span>
<span data-ttu-id="6882c-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6882c-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
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

### <a name="response"></a><span data-ttu-id="6882c-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="6882c-151">Response</span></span>
<span data-ttu-id="6882c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6882c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




