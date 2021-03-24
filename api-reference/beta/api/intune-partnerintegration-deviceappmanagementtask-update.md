---
title: Atualizar deviceAppManagementTask
description: Atualize as propriedades de um objeto deviceAppManagementTask.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c22587015dbf22b1537c7774244d551225e8690f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134876"
---
# <a name="update-deviceappmanagementtask"></a><span data-ttu-id="52602-103">Atualizar deviceAppManagementTask</span><span class="sxs-lookup"><span data-stu-id="52602-103">Update deviceAppManagementTask</span></span>

<span data-ttu-id="52602-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52602-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52602-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="52602-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52602-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52602-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52602-107">Atualize as propriedades de [um objeto deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="52602-107">Update the properties of a [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52602-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="52602-108">Prerequisites</span></span>
<span data-ttu-id="52602-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52602-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52602-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52602-111">Permission type</span></span>|<span data-ttu-id="52602-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52602-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52602-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52602-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52602-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52602-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="52602-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52602-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52602-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52602-116">Not supported.</span></span>|
|<span data-ttu-id="52602-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52602-117">Application</span></span>|<span data-ttu-id="52602-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52602-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52602-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52602-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="request-headers"></a><span data-ttu-id="52602-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52602-120">Request headers</span></span>
|<span data-ttu-id="52602-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="52602-121">Header</span></span>|<span data-ttu-id="52602-122">Valor</span><span class="sxs-lookup"><span data-stu-id="52602-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52602-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="52602-123">Authorization</span></span>|<span data-ttu-id="52602-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52602-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52602-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="52602-125">Accept</span></span>|<span data-ttu-id="52602-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52602-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52602-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52602-127">Request body</span></span>
<span data-ttu-id="52602-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="52602-128">In the request body, supply a JSON representation for the [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

<span data-ttu-id="52602-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="52602-129">The following table shows the properties that are required when you create the [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span>

|<span data-ttu-id="52602-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52602-130">Property</span></span>|<span data-ttu-id="52602-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="52602-131">Type</span></span>|<span data-ttu-id="52602-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="52602-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52602-133">id</span><span class="sxs-lookup"><span data-stu-id="52602-133">id</span></span>|<span data-ttu-id="52602-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52602-134">String</span></span>|<span data-ttu-id="52602-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="52602-135">The entity key.</span></span>|
|<span data-ttu-id="52602-136">displayName</span><span class="sxs-lookup"><span data-stu-id="52602-136">displayName</span></span>|<span data-ttu-id="52602-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52602-137">String</span></span>|<span data-ttu-id="52602-138">O nome.</span><span class="sxs-lookup"><span data-stu-id="52602-138">The name.</span></span>|
|<span data-ttu-id="52602-139">descrição</span><span class="sxs-lookup"><span data-stu-id="52602-139">description</span></span>|<span data-ttu-id="52602-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52602-140">String</span></span>|<span data-ttu-id="52602-141">A descrição.</span><span class="sxs-lookup"><span data-stu-id="52602-141">The description.</span></span>|
|<span data-ttu-id="52602-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="52602-142">createdDateTime</span></span>|<span data-ttu-id="52602-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52602-143">DateTimeOffset</span></span>|<span data-ttu-id="52602-144">A data criada.</span><span class="sxs-lookup"><span data-stu-id="52602-144">The created date.</span></span>|
|<span data-ttu-id="52602-145">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="52602-145">dueDateTime</span></span>|<span data-ttu-id="52602-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52602-146">DateTimeOffset</span></span>|<span data-ttu-id="52602-147">A data de vencimento.</span><span class="sxs-lookup"><span data-stu-id="52602-147">The due date.</span></span>|
|<span data-ttu-id="52602-148">category</span><span class="sxs-lookup"><span data-stu-id="52602-148">category</span></span>|[<span data-ttu-id="52602-149">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="52602-149">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="52602-150">A categoria.</span><span class="sxs-lookup"><span data-stu-id="52602-150">The category.</span></span> <span data-ttu-id="52602-151">Os valores possíveis são: `unknown` e `advancedThreatProtection`.</span><span class="sxs-lookup"><span data-stu-id="52602-151">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="52602-152">prioridade</span><span class="sxs-lookup"><span data-stu-id="52602-152">priority</span></span>|[<span data-ttu-id="52602-153">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="52602-153">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="52602-154">A prioridade.</span><span class="sxs-lookup"><span data-stu-id="52602-154">The priority.</span></span> <span data-ttu-id="52602-155">Os valores possíveis são: `none`, `high`, `low`.</span><span class="sxs-lookup"><span data-stu-id="52602-155">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="52602-156">criador</span><span class="sxs-lookup"><span data-stu-id="52602-156">creator</span></span>|<span data-ttu-id="52602-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52602-157">String</span></span>|<span data-ttu-id="52602-158">O endereço de email do criador.</span><span class="sxs-lookup"><span data-stu-id="52602-158">The email address of the creator.</span></span>|
|<span data-ttu-id="52602-159">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="52602-159">creatorNotes</span></span>|<span data-ttu-id="52602-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52602-160">String</span></span>|<span data-ttu-id="52602-161">Observações do criador.</span><span class="sxs-lookup"><span data-stu-id="52602-161">Notes from the creator.</span></span>|
|<span data-ttu-id="52602-162">assignedTo</span><span class="sxs-lookup"><span data-stu-id="52602-162">assignedTo</span></span>|<span data-ttu-id="52602-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52602-163">String</span></span>|<span data-ttu-id="52602-164">O nome ou o email do administrador ao que essa tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="52602-164">The name or email of the admin this task is assigned to.</span></span>|
|<span data-ttu-id="52602-165">status</span><span class="sxs-lookup"><span data-stu-id="52602-165">status</span></span>|[<span data-ttu-id="52602-166">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="52602-166">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="52602-167">O status.</span><span class="sxs-lookup"><span data-stu-id="52602-167">The status.</span></span> <span data-ttu-id="52602-168">Os valores possíveis são: `unknown`, `pending`, `active`, `completed`, `rejected`.</span><span class="sxs-lookup"><span data-stu-id="52602-168">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|



## <a name="response"></a><span data-ttu-id="52602-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="52602-169">Response</span></span>
<span data-ttu-id="52602-170">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52602-170">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52602-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52602-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="52602-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52602-172">Request</span></span>
<span data-ttu-id="52602-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52602-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="52602-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="52602-174">Response</span></span>
<span data-ttu-id="52602-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52602-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




