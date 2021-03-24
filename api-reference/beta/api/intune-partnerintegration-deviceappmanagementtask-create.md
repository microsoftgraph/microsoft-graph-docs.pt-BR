---
title: Criar deviceAppManagementTask
description: Crie um novo objeto deviceAppManagementTask.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8f90599d0feefaa7a40e8ced47ab1653eb2e4d97
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134904"
---
# <a name="create-deviceappmanagementtask"></a><span data-ttu-id="9f56b-103">Criar deviceAppManagementTask</span><span class="sxs-lookup"><span data-stu-id="9f56b-103">Create deviceAppManagementTask</span></span>

<span data-ttu-id="9f56b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f56b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f56b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9f56b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f56b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9f56b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f56b-107">Crie um novo [objeto deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="9f56b-107">Create a new [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f56b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9f56b-108">Prerequisites</span></span>
<span data-ttu-id="9f56b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f56b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f56b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f56b-111">Permission type</span></span>|<span data-ttu-id="9f56b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f56b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f56b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f56b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f56b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f56b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9f56b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f56b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f56b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f56b-116">Not supported.</span></span>|
|<span data-ttu-id="9f56b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f56b-117">Application</span></span>|<span data-ttu-id="9f56b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f56b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f56b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f56b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a><span data-ttu-id="9f56b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f56b-120">Request headers</span></span>
|<span data-ttu-id="9f56b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9f56b-121">Header</span></span>|<span data-ttu-id="9f56b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9f56b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f56b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f56b-123">Authorization</span></span>|<span data-ttu-id="9f56b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f56b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f56b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9f56b-125">Accept</span></span>|<span data-ttu-id="9f56b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f56b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f56b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f56b-127">Request body</span></span>
<span data-ttu-id="9f56b-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceAppManagementTask.</span><span class="sxs-lookup"><span data-stu-id="9f56b-128">In the request body, supply a JSON representation for the deviceAppManagementTask object.</span></span>

<span data-ttu-id="9f56b-129">A tabela a seguir mostra as propriedades necessárias ao criar deviceAppManagementTask.</span><span class="sxs-lookup"><span data-stu-id="9f56b-129">The following table shows the properties that are required when you create the deviceAppManagementTask.</span></span>

|<span data-ttu-id="9f56b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f56b-130">Property</span></span>|<span data-ttu-id="9f56b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f56b-131">Type</span></span>|<span data-ttu-id="9f56b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f56b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f56b-133">id</span><span class="sxs-lookup"><span data-stu-id="9f56b-133">id</span></span>|<span data-ttu-id="9f56b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f56b-134">String</span></span>|<span data-ttu-id="9f56b-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9f56b-135">The entity key.</span></span>|
|<span data-ttu-id="9f56b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9f56b-136">displayName</span></span>|<span data-ttu-id="9f56b-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f56b-137">String</span></span>|<span data-ttu-id="9f56b-138">O nome.</span><span class="sxs-lookup"><span data-stu-id="9f56b-138">The name.</span></span>|
|<span data-ttu-id="9f56b-139">descrição</span><span class="sxs-lookup"><span data-stu-id="9f56b-139">description</span></span>|<span data-ttu-id="9f56b-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f56b-140">String</span></span>|<span data-ttu-id="9f56b-141">A descrição.</span><span class="sxs-lookup"><span data-stu-id="9f56b-141">The description.</span></span>|
|<span data-ttu-id="9f56b-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f56b-142">createdDateTime</span></span>|<span data-ttu-id="9f56b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f56b-143">DateTimeOffset</span></span>|<span data-ttu-id="9f56b-144">A data criada.</span><span class="sxs-lookup"><span data-stu-id="9f56b-144">The created date.</span></span>|
|<span data-ttu-id="9f56b-145">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="9f56b-145">dueDateTime</span></span>|<span data-ttu-id="9f56b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f56b-146">DateTimeOffset</span></span>|<span data-ttu-id="9f56b-147">A data de vencimento.</span><span class="sxs-lookup"><span data-stu-id="9f56b-147">The due date.</span></span>|
|<span data-ttu-id="9f56b-148">category</span><span class="sxs-lookup"><span data-stu-id="9f56b-148">category</span></span>|[<span data-ttu-id="9f56b-149">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="9f56b-149">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="9f56b-150">A categoria.</span><span class="sxs-lookup"><span data-stu-id="9f56b-150">The category.</span></span> <span data-ttu-id="9f56b-151">Os valores possíveis são: `unknown` e `advancedThreatProtection`.</span><span class="sxs-lookup"><span data-stu-id="9f56b-151">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="9f56b-152">prioridade</span><span class="sxs-lookup"><span data-stu-id="9f56b-152">priority</span></span>|[<span data-ttu-id="9f56b-153">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="9f56b-153">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="9f56b-154">A prioridade.</span><span class="sxs-lookup"><span data-stu-id="9f56b-154">The priority.</span></span> <span data-ttu-id="9f56b-155">Os valores possíveis são: `none`, `high`, `low`.</span><span class="sxs-lookup"><span data-stu-id="9f56b-155">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="9f56b-156">criador</span><span class="sxs-lookup"><span data-stu-id="9f56b-156">creator</span></span>|<span data-ttu-id="9f56b-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f56b-157">String</span></span>|<span data-ttu-id="9f56b-158">O endereço de email do criador.</span><span class="sxs-lookup"><span data-stu-id="9f56b-158">The email address of the creator.</span></span>|
|<span data-ttu-id="9f56b-159">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="9f56b-159">creatorNotes</span></span>|<span data-ttu-id="9f56b-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f56b-160">String</span></span>|<span data-ttu-id="9f56b-161">Observações do criador.</span><span class="sxs-lookup"><span data-stu-id="9f56b-161">Notes from the creator.</span></span>|
|<span data-ttu-id="9f56b-162">assignedTo</span><span class="sxs-lookup"><span data-stu-id="9f56b-162">assignedTo</span></span>|<span data-ttu-id="9f56b-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f56b-163">String</span></span>|<span data-ttu-id="9f56b-164">O nome ou o email do administrador ao que essa tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="9f56b-164">The name or email of the admin this task is assigned to.</span></span>|
|<span data-ttu-id="9f56b-165">status</span><span class="sxs-lookup"><span data-stu-id="9f56b-165">status</span></span>|[<span data-ttu-id="9f56b-166">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="9f56b-166">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="9f56b-167">O status.</span><span class="sxs-lookup"><span data-stu-id="9f56b-167">The status.</span></span> <span data-ttu-id="9f56b-168">Os valores possíveis são: `unknown`, `pending`, `active`, `completed`, `rejected`.</span><span class="sxs-lookup"><span data-stu-id="9f56b-168">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|



## <a name="response"></a><span data-ttu-id="9f56b-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f56b-169">Response</span></span>
<span data-ttu-id="9f56b-170">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f56b-170">If successful, this method returns a `201 Created` response code and a [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f56b-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f56b-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f56b-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f56b-172">Request</span></span>
<span data-ttu-id="9f56b-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f56b-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f56b-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f56b-174">Response</span></span>
<span data-ttu-id="9f56b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f56b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




