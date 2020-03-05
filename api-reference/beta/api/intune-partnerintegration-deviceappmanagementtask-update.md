---
title: Atualizar deviceAppManagementTask
description: Atualiza as propriedades de um objeto deviceAppManagementTask.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 814ac463d788ffe6749ac1c472ba945be4d58c2b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42461240"
---
# <a name="update-deviceappmanagementtask"></a><span data-ttu-id="6d814-103">Atualizar deviceAppManagementTask</span><span class="sxs-lookup"><span data-stu-id="6d814-103">Update deviceAppManagementTask</span></span>

<span data-ttu-id="6d814-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6d814-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d814-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6d814-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d814-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d814-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d814-107">Atualiza as propriedades de um objeto [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) .</span><span class="sxs-lookup"><span data-stu-id="6d814-107">Update the properties of a [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d814-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6d814-108">Prerequisites</span></span>
<span data-ttu-id="6d814-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d814-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d814-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d814-111">Permission type</span></span>|<span data-ttu-id="6d814-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6d814-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d814-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d814-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6d814-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d814-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6d814-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d814-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d814-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d814-116">Not supported.</span></span>|
|<span data-ttu-id="6d814-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d814-117">Application</span></span>|<span data-ttu-id="6d814-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d814-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d814-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d814-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="request-headers"></a><span data-ttu-id="6d814-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d814-120">Request headers</span></span>
|<span data-ttu-id="6d814-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6d814-121">Header</span></span>|<span data-ttu-id="6d814-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6d814-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d814-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d814-123">Authorization</span></span>|<span data-ttu-id="6d814-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d814-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d814-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6d814-125">Accept</span></span>|<span data-ttu-id="6d814-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d814-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d814-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d814-127">Request body</span></span>
<span data-ttu-id="6d814-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) .</span><span class="sxs-lookup"><span data-stu-id="6d814-128">In the request body, supply a JSON representation for the [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

<span data-ttu-id="6d814-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="6d814-129">The following table shows the properties that are required when you create the [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span>

|<span data-ttu-id="6d814-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d814-130">Property</span></span>|<span data-ttu-id="6d814-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d814-131">Type</span></span>|<span data-ttu-id="6d814-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d814-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d814-133">id</span><span class="sxs-lookup"><span data-stu-id="6d814-133">id</span></span>|<span data-ttu-id="6d814-134">String</span><span class="sxs-lookup"><span data-stu-id="6d814-134">String</span></span>|<span data-ttu-id="6d814-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6d814-135">The entity key.</span></span>|
|<span data-ttu-id="6d814-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6d814-136">displayName</span></span>|<span data-ttu-id="6d814-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d814-137">String</span></span>|<span data-ttu-id="6d814-138">O nome.</span><span class="sxs-lookup"><span data-stu-id="6d814-138">The name.</span></span>|
|<span data-ttu-id="6d814-139">description</span><span class="sxs-lookup"><span data-stu-id="6d814-139">description</span></span>|<span data-ttu-id="6d814-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d814-140">String</span></span>|<span data-ttu-id="6d814-141">A descrição.</span><span class="sxs-lookup"><span data-stu-id="6d814-141">The description.</span></span>|
|<span data-ttu-id="6d814-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d814-142">createdDateTime</span></span>|<span data-ttu-id="6d814-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d814-143">DateTimeOffset</span></span>|<span data-ttu-id="6d814-144">A data de criação.</span><span class="sxs-lookup"><span data-stu-id="6d814-144">The created date.</span></span>|
|<span data-ttu-id="6d814-145">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="6d814-145">dueDateTime</span></span>|<span data-ttu-id="6d814-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d814-146">DateTimeOffset</span></span>|<span data-ttu-id="6d814-147">A data de conclusão.</span><span class="sxs-lookup"><span data-stu-id="6d814-147">The due date.</span></span>|
|<span data-ttu-id="6d814-148">category</span><span class="sxs-lookup"><span data-stu-id="6d814-148">category</span></span>|[<span data-ttu-id="6d814-149">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="6d814-149">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="6d814-150">A categoria.</span><span class="sxs-lookup"><span data-stu-id="6d814-150">The category.</span></span> <span data-ttu-id="6d814-151">Os valores possíveis são: `unknown` e `advancedThreatProtection`.</span><span class="sxs-lookup"><span data-stu-id="6d814-151">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="6d814-152">prioridade</span><span class="sxs-lookup"><span data-stu-id="6d814-152">priority</span></span>|[<span data-ttu-id="6d814-153">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="6d814-153">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="6d814-154">A prioridade.</span><span class="sxs-lookup"><span data-stu-id="6d814-154">The priority.</span></span> <span data-ttu-id="6d814-155">Os valores possíveis são: `none`, `high`, `low`.</span><span class="sxs-lookup"><span data-stu-id="6d814-155">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="6d814-156">Criador</span><span class="sxs-lookup"><span data-stu-id="6d814-156">creator</span></span>|<span data-ttu-id="6d814-157">String</span><span class="sxs-lookup"><span data-stu-id="6d814-157">String</span></span>|<span data-ttu-id="6d814-158">O endereço de email do criador.</span><span class="sxs-lookup"><span data-stu-id="6d814-158">The email address of the creator.</span></span>|
|<span data-ttu-id="6d814-159">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="6d814-159">creatorNotes</span></span>|<span data-ttu-id="6d814-160">String</span><span class="sxs-lookup"><span data-stu-id="6d814-160">String</span></span>|<span data-ttu-id="6d814-161">Observações do criador.</span><span class="sxs-lookup"><span data-stu-id="6d814-161">Notes from the creator.</span></span>|
|<span data-ttu-id="6d814-162">assignedTo</span><span class="sxs-lookup"><span data-stu-id="6d814-162">assignedTo</span></span>|<span data-ttu-id="6d814-163">String</span><span class="sxs-lookup"><span data-stu-id="6d814-163">String</span></span>|<span data-ttu-id="6d814-164">O nome ou email do administrador ao qual esta tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="6d814-164">The name or email of the admin this task is assigned to.</span></span>|
|<span data-ttu-id="6d814-165">status</span><span class="sxs-lookup"><span data-stu-id="6d814-165">status</span></span>|[<span data-ttu-id="6d814-166">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="6d814-166">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="6d814-167">O status.</span><span class="sxs-lookup"><span data-stu-id="6d814-167">The status.</span></span> <span data-ttu-id="6d814-168">Os valores possíveis são: `unknown`, `pending`, `active`, `completed`, `rejected`.</span><span class="sxs-lookup"><span data-stu-id="6d814-168">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|



## <a name="response"></a><span data-ttu-id="6d814-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d814-169">Response</span></span>
<span data-ttu-id="6d814-170">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d814-170">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d814-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d814-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d814-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d814-172">Request</span></span>
<span data-ttu-id="6d814-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d814-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
Content-type: application/json
Content-length: 400

{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "displayName": "Display Name value",
  "description": "Description value",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="6d814-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d814-174">Response</span></span>
<span data-ttu-id="6d814-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d814-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 508

{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "id": "814545cc-45cc-8145-cc45-4581cc454581",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending"
}
```





