---
title: Criar deviceAppManagementTask
description: Criar um novo objeto deviceAppManagementTask.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0fdf298dddb37be4b7e858e75aaa4b5cb82babf5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36351732"
---
# <a name="create-deviceappmanagementtask"></a><span data-ttu-id="66d39-103">Criar deviceAppManagementTask</span><span class="sxs-lookup"><span data-stu-id="66d39-103">Create deviceAppManagementTask</span></span>

> <span data-ttu-id="66d39-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="66d39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66d39-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="66d39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66d39-106">Criar um novo objeto [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) .</span><span class="sxs-lookup"><span data-stu-id="66d39-106">Create a new [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66d39-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="66d39-107">Prerequisites</span></span>
<span data-ttu-id="66d39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66d39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66d39-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66d39-110">Permission type</span></span>|<span data-ttu-id="66d39-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="66d39-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66d39-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66d39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66d39-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66d39-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="66d39-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66d39-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66d39-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66d39-115">Not supported.</span></span>|
|<span data-ttu-id="66d39-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66d39-116">Application</span></span>|<span data-ttu-id="66d39-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66d39-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="66d39-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66d39-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a><span data-ttu-id="66d39-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66d39-119">Request headers</span></span>
|<span data-ttu-id="66d39-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="66d39-120">Header</span></span>|<span data-ttu-id="66d39-121">Valor</span><span class="sxs-lookup"><span data-stu-id="66d39-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66d39-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="66d39-122">Authorization</span></span>|<span data-ttu-id="66d39-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66d39-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66d39-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="66d39-124">Accept</span></span>|<span data-ttu-id="66d39-125">application/json</span><span class="sxs-lookup"><span data-stu-id="66d39-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66d39-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66d39-126">Request body</span></span>
<span data-ttu-id="66d39-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceAppManagementTask.</span><span class="sxs-lookup"><span data-stu-id="66d39-127">In the request body, supply a JSON representation for the deviceAppManagementTask object.</span></span>

<span data-ttu-id="66d39-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceAppManagementTask.</span><span class="sxs-lookup"><span data-stu-id="66d39-128">The following table shows the properties that are required when you create the deviceAppManagementTask.</span></span>

|<span data-ttu-id="66d39-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66d39-129">Property</span></span>|<span data-ttu-id="66d39-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="66d39-130">Type</span></span>|<span data-ttu-id="66d39-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="66d39-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66d39-132">id</span><span class="sxs-lookup"><span data-stu-id="66d39-132">id</span></span>|<span data-ttu-id="66d39-133">String</span><span class="sxs-lookup"><span data-stu-id="66d39-133">String</span></span>|<span data-ttu-id="66d39-134">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="66d39-134">The entity key.</span></span>|
|<span data-ttu-id="66d39-135">displayName</span><span class="sxs-lookup"><span data-stu-id="66d39-135">displayName</span></span>|<span data-ttu-id="66d39-136">String</span><span class="sxs-lookup"><span data-stu-id="66d39-136">String</span></span>|<span data-ttu-id="66d39-137">O nome.</span><span class="sxs-lookup"><span data-stu-id="66d39-137">The name.</span></span>|
|<span data-ttu-id="66d39-138">descrição</span><span class="sxs-lookup"><span data-stu-id="66d39-138">description</span></span>|<span data-ttu-id="66d39-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66d39-139">String</span></span>|<span data-ttu-id="66d39-140">A descrição.</span><span class="sxs-lookup"><span data-stu-id="66d39-140">The description.</span></span>|
|<span data-ttu-id="66d39-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66d39-141">createdDateTime</span></span>|<span data-ttu-id="66d39-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66d39-142">DateTimeOffset</span></span>|<span data-ttu-id="66d39-143">A data de criação.</span><span class="sxs-lookup"><span data-stu-id="66d39-143">The created date.</span></span>|
|<span data-ttu-id="66d39-144">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="66d39-144">dueDateTime</span></span>|<span data-ttu-id="66d39-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66d39-145">DateTimeOffset</span></span>|<span data-ttu-id="66d39-146">A data de conclusão.</span><span class="sxs-lookup"><span data-stu-id="66d39-146">The due date.</span></span>|
|<span data-ttu-id="66d39-147">category</span><span class="sxs-lookup"><span data-stu-id="66d39-147">category</span></span>|[<span data-ttu-id="66d39-148">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="66d39-148">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="66d39-149">A categoria.</span><span class="sxs-lookup"><span data-stu-id="66d39-149">The category.</span></span> <span data-ttu-id="66d39-150">Os valores possíveis são: `unknown` e `advancedThreatProtection`.</span><span class="sxs-lookup"><span data-stu-id="66d39-150">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="66d39-151">prioridade</span><span class="sxs-lookup"><span data-stu-id="66d39-151">priority</span></span>|[<span data-ttu-id="66d39-152">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="66d39-152">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="66d39-153">A prioridade.</span><span class="sxs-lookup"><span data-stu-id="66d39-153">The priority.</span></span> <span data-ttu-id="66d39-154">Os valores possíveis são: `none`, `high`, `low`.</span><span class="sxs-lookup"><span data-stu-id="66d39-154">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="66d39-155">Criador</span><span class="sxs-lookup"><span data-stu-id="66d39-155">creator</span></span>|<span data-ttu-id="66d39-156">String</span><span class="sxs-lookup"><span data-stu-id="66d39-156">String</span></span>|<span data-ttu-id="66d39-157">O endereço de email do criador.</span><span class="sxs-lookup"><span data-stu-id="66d39-157">The email address of the creator.</span></span>|
|<span data-ttu-id="66d39-158">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="66d39-158">creatorNotes</span></span>|<span data-ttu-id="66d39-159">String</span><span class="sxs-lookup"><span data-stu-id="66d39-159">String</span></span>|<span data-ttu-id="66d39-160">Observações do criador.</span><span class="sxs-lookup"><span data-stu-id="66d39-160">Notes from the creator.</span></span>|
|<span data-ttu-id="66d39-161">assignedTo</span><span class="sxs-lookup"><span data-stu-id="66d39-161">assignedTo</span></span>|<span data-ttu-id="66d39-162">String</span><span class="sxs-lookup"><span data-stu-id="66d39-162">String</span></span>|<span data-ttu-id="66d39-163">O nome ou email do administrador ao qual esta tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="66d39-163">The name or email of the admin this task is assigned to.</span></span>|
|<span data-ttu-id="66d39-164">status</span><span class="sxs-lookup"><span data-stu-id="66d39-164">status</span></span>|[<span data-ttu-id="66d39-165">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="66d39-165">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="66d39-166">O status.</span><span class="sxs-lookup"><span data-stu-id="66d39-166">The status.</span></span> <span data-ttu-id="66d39-167">Os valores possíveis são: `unknown`, `pending`, `active`, `completed`, `rejected`.</span><span class="sxs-lookup"><span data-stu-id="66d39-167">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|



## <a name="response"></a><span data-ttu-id="66d39-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="66d39-168">Response</span></span>
<span data-ttu-id="66d39-169">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66d39-169">If successful, this method returns a `201 Created` response code and a [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66d39-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66d39-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="66d39-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66d39-171">Request</span></span>
<span data-ttu-id="66d39-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66d39-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
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

### <a name="response"></a><span data-ttu-id="66d39-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="66d39-173">Response</span></span>
<span data-ttu-id="66d39-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66d39-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






