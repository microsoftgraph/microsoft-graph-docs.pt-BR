---
title: Atualizar securityConfigurationTask
description: Atualiza as propriedades de um objeto securityConfigurationTask.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 18a89b0570a17752d82d2dc050b5683c8c947760
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49296304"
---
# <a name="update-securityconfigurationtask"></a><span data-ttu-id="d758b-103">Atualizar securityConfigurationTask</span><span class="sxs-lookup"><span data-stu-id="d758b-103">Update securityConfigurationTask</span></span>

<span data-ttu-id="d758b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d758b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d758b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d758b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d758b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d758b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d758b-107">Atualiza as propriedades de um objeto [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) .</span><span class="sxs-lookup"><span data-stu-id="d758b-107">Update the properties of a [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d758b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d758b-108">Prerequisites</span></span>
<span data-ttu-id="d758b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d758b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d758b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d758b-111">Permission type</span></span>|<span data-ttu-id="d758b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d758b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d758b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d758b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d758b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d758b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d758b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d758b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d758b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d758b-116">Not supported.</span></span>|
|<span data-ttu-id="d758b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d758b-117">Application</span></span>|<span data-ttu-id="d758b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d758b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d758b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d758b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="request-headers"></a><span data-ttu-id="d758b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d758b-120">Request headers</span></span>
|<span data-ttu-id="d758b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d758b-121">Header</span></span>|<span data-ttu-id="d758b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d758b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d758b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d758b-123">Authorization</span></span>|<span data-ttu-id="d758b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d758b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d758b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d758b-125">Accept</span></span>|<span data-ttu-id="d758b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d758b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d758b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d758b-127">Request body</span></span>
<span data-ttu-id="d758b-128">No corpo da solicitação, forneça uma representação JSON do objeto [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) .</span><span class="sxs-lookup"><span data-stu-id="d758b-128">In the request body, supply a JSON representation for the [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object.</span></span>

<span data-ttu-id="d758b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md).</span><span class="sxs-lookup"><span data-stu-id="d758b-129">The following table shows the properties that are required when you create the [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md).</span></span>

|<span data-ttu-id="d758b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d758b-130">Property</span></span>|<span data-ttu-id="d758b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d758b-131">Type</span></span>|<span data-ttu-id="d758b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d758b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d758b-133">id</span><span class="sxs-lookup"><span data-stu-id="d758b-133">id</span></span>|<span data-ttu-id="d758b-134">String</span><span class="sxs-lookup"><span data-stu-id="d758b-134">String</span></span>|<span data-ttu-id="d758b-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d758b-135">The entity key.</span></span> <span data-ttu-id="d758b-136">Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="d758b-136">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="d758b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d758b-137">displayName</span></span>|<span data-ttu-id="d758b-138">String</span><span class="sxs-lookup"><span data-stu-id="d758b-138">String</span></span>|<span data-ttu-id="d758b-139">O nome.</span><span class="sxs-lookup"><span data-stu-id="d758b-139">The name.</span></span> <span data-ttu-id="d758b-140">Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="d758b-140">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="d758b-141">description</span><span class="sxs-lookup"><span data-stu-id="d758b-141">description</span></span>|<span data-ttu-id="d758b-142">String</span><span class="sxs-lookup"><span data-stu-id="d758b-142">String</span></span>|<span data-ttu-id="d758b-143">A descrição.</span><span class="sxs-lookup"><span data-stu-id="d758b-143">The description.</span></span> <span data-ttu-id="d758b-144">Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="d758b-144">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="d758b-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d758b-145">createdDateTime</span></span>|<span data-ttu-id="d758b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d758b-146">DateTimeOffset</span></span>|<span data-ttu-id="d758b-147">A data de criação.</span><span class="sxs-lookup"><span data-stu-id="d758b-147">The created date.</span></span> <span data-ttu-id="d758b-148">Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="d758b-148">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="d758b-149">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="d758b-149">dueDateTime</span></span>|<span data-ttu-id="d758b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d758b-150">DateTimeOffset</span></span>|<span data-ttu-id="d758b-151">A data de conclusão.</span><span class="sxs-lookup"><span data-stu-id="d758b-151">The due date.</span></span> <span data-ttu-id="d758b-152">Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="d758b-152">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="d758b-153">category</span><span class="sxs-lookup"><span data-stu-id="d758b-153">category</span></span>|[<span data-ttu-id="d758b-154">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="d758b-154">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="d758b-155">A categoria.</span><span class="sxs-lookup"><span data-stu-id="d758b-155">The category.</span></span> <span data-ttu-id="d758b-156">Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="d758b-156">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="d758b-157">Os valores possíveis são: `unknown` e `advancedThreatProtection`.</span><span class="sxs-lookup"><span data-stu-id="d758b-157">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="d758b-158">prioridade</span><span class="sxs-lookup"><span data-stu-id="d758b-158">priority</span></span>|[<span data-ttu-id="d758b-159">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="d758b-159">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="d758b-160">A prioridade.</span><span class="sxs-lookup"><span data-stu-id="d758b-160">The priority.</span></span> <span data-ttu-id="d758b-161">Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="d758b-161">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="d758b-162">Os valores possíveis são: `none`, `high`, `low`.</span><span class="sxs-lookup"><span data-stu-id="d758b-162">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="d758b-163">criador</span><span class="sxs-lookup"><span data-stu-id="d758b-163">creator</span></span>|<span data-ttu-id="d758b-164">String</span><span class="sxs-lookup"><span data-stu-id="d758b-164">String</span></span>|<span data-ttu-id="d758b-165">O endereço de email do criador.</span><span class="sxs-lookup"><span data-stu-id="d758b-165">The email address of the creator.</span></span> <span data-ttu-id="d758b-166">Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="d758b-166">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="d758b-167">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="d758b-167">creatorNotes</span></span>|<span data-ttu-id="d758b-168">String</span><span class="sxs-lookup"><span data-stu-id="d758b-168">String</span></span>|<span data-ttu-id="d758b-169">Observações do criador.</span><span class="sxs-lookup"><span data-stu-id="d758b-169">Notes from the creator.</span></span> <span data-ttu-id="d758b-170">Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="d758b-170">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="d758b-171">assignedTo</span><span class="sxs-lookup"><span data-stu-id="d758b-171">assignedTo</span></span>|<span data-ttu-id="d758b-172">String</span><span class="sxs-lookup"><span data-stu-id="d758b-172">String</span></span>|<span data-ttu-id="d758b-173">O nome ou email do administrador ao qual esta tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="d758b-173">The name or email of the admin this task is assigned to.</span></span> <span data-ttu-id="d758b-174">Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="d758b-174">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="d758b-175">status</span><span class="sxs-lookup"><span data-stu-id="d758b-175">status</span></span>|[<span data-ttu-id="d758b-176">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="d758b-176">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="d758b-177">O status.</span><span class="sxs-lookup"><span data-stu-id="d758b-177">The status.</span></span> <span data-ttu-id="d758b-178">Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="d758b-178">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="d758b-179">Os valores possíveis são: `unknown`, `pending`, `active`, `completed`, `rejected`.</span><span class="sxs-lookup"><span data-stu-id="d758b-179">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|
|<span data-ttu-id="d758b-180">endpointSecurityPolicy</span><span class="sxs-lookup"><span data-stu-id="d758b-180">endpointSecurityPolicy</span></span>|[<span data-ttu-id="d758b-181">endpointSecurityConfigurationType</span><span class="sxs-lookup"><span data-stu-id="d758b-181">endpointSecurityConfigurationType</span></span>](../resources/intune-partnerintegration-endpointsecurityconfigurationtype.md)|<span data-ttu-id="d758b-182">O tipo de política de segurança do ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="d758b-182">The endpoint security policy type.</span></span> <span data-ttu-id="d758b-183">Os valores possíveis são: `unknown`, `antivirus`, `diskEncryption`, `firewall`, `endpointDetectionAndResponse`, `attackSurfaceReduction`, `accountProtection`.</span><span class="sxs-lookup"><span data-stu-id="d758b-183">Possible values are: `unknown`, `antivirus`, `diskEncryption`, `firewall`, `endpointDetectionAndResponse`, `attackSurfaceReduction`, `accountProtection`.</span></span>|
|<span data-ttu-id="d758b-184">applicablePlatform</span><span class="sxs-lookup"><span data-stu-id="d758b-184">applicablePlatform</span></span>|[<span data-ttu-id="d758b-185">endpointSecurityConfigurationApplicablePlatform</span><span class="sxs-lookup"><span data-stu-id="d758b-185">endpointSecurityConfigurationApplicablePlatform</span></span>](../resources/intune-partnerintegration-endpointsecurityconfigurationapplicableplatform.md)|<span data-ttu-id="d758b-186">A plataforma aplicável.</span><span class="sxs-lookup"><span data-stu-id="d758b-186">The applicable platform.</span></span> <span data-ttu-id="d758b-187">Os valores possíveis são: `unknown`, `macOS`, `windows10AndLater`, `windows10AndWindowsServer`.</span><span class="sxs-lookup"><span data-stu-id="d758b-187">Possible values are: `unknown`, `macOS`, `windows10AndLater`, `windows10AndWindowsServer`.</span></span>|
|<span data-ttu-id="d758b-188">endpointSecurityPolicyProfile</span><span class="sxs-lookup"><span data-stu-id="d758b-188">endpointSecurityPolicyProfile</span></span>|[<span data-ttu-id="d758b-189">endpointSecurityConfigurationProfileType</span><span class="sxs-lookup"><span data-stu-id="d758b-189">endpointSecurityConfigurationProfileType</span></span>](../resources/intune-partnerintegration-endpointsecurityconfigurationprofiletype.md)|<span data-ttu-id="d758b-190">O perfil da política de segurança do ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="d758b-190">The endpoint security policy profile.</span></span> <span data-ttu-id="d758b-191">Os valores possíveis são:, `unknown` `antivirus` , `windowsSecurity` , `bitLocker` , `fileVault` , `firewall` , `firewallRules` , `endpointDetectionAndResponse` , `deviceControl` , `appAndBrowserIsolation` , `exploitProtection` , `webProtection` ,, `applicationControl` `attackSurfaceReductionRules` `accountProtection` .</span><span class="sxs-lookup"><span data-stu-id="d758b-191">Possible values are: `unknown`, `antivirus`, `windowsSecurity`, `bitLocker`, `fileVault`, `firewall`, `firewallRules`, `endpointDetectionAndResponse`, `deviceControl`, `appAndBrowserIsolation`, `exploitProtection`, `webProtection`, `applicationControl`, `attackSurfaceReductionRules`, `accountProtection`.</span></span>|
|<span data-ttu-id="d758b-192">insights</span><span class="sxs-lookup"><span data-stu-id="d758b-192">insights</span></span>|<span data-ttu-id="d758b-193">String</span><span class="sxs-lookup"><span data-stu-id="d758b-193">String</span></span>|<span data-ttu-id="d758b-194">Informações sobre a mitigação.</span><span class="sxs-lookup"><span data-stu-id="d758b-194">Information about the mitigation.</span></span>|
|<span data-ttu-id="d758b-195">managedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d758b-195">managedDeviceCount</span></span>|<span data-ttu-id="d758b-196">Int32</span><span class="sxs-lookup"><span data-stu-id="d758b-196">Int32</span></span>|<span data-ttu-id="d758b-197">O número de dispositivos vulneráveis.</span><span class="sxs-lookup"><span data-stu-id="d758b-197">The number of vulnerable devices.</span></span>|
|<span data-ttu-id="d758b-198">intendedSettings</span><span class="sxs-lookup"><span data-stu-id="d758b-198">intendedSettings</span></span>|<span data-ttu-id="d758b-199">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="d758b-199">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="d758b-200">As configurações pretendidas e seus valores.</span><span class="sxs-lookup"><span data-stu-id="d758b-200">The intended settings and their values.</span></span>|



## <a name="response"></a><span data-ttu-id="d758b-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="d758b-201">Response</span></span>
<span data-ttu-id="d758b-202">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d758b-202">If successful, this method returns a `200 OK` response code and an updated [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d758b-203">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d758b-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="d758b-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d758b-204">Request</span></span>
<span data-ttu-id="d758b-205">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d758b-205">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
Content-type: application/json
Content-length: 746

{
  "@odata.type": "#microsoft.graph.securityConfigurationTask",
  "displayName": "Display Name value",
  "description": "Description value",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending",
  "endpointSecurityPolicy": "antivirus",
  "applicablePlatform": "macOS",
  "endpointSecurityPolicyProfile": "antivirus",
  "insights": "Insights value",
  "managedDeviceCount": 2,
  "intendedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d758b-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="d758b-206">Response</span></span>
<span data-ttu-id="d758b-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d758b-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 854

{
  "@odata.type": "#microsoft.graph.securityConfigurationTask",
  "id": "5d630f12-0f12-5d63-120f-635d120f635d",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending",
  "endpointSecurityPolicy": "antivirus",
  "applicablePlatform": "macOS",
  "endpointSecurityPolicyProfile": "antivirus",
  "insights": "Insights value",
  "managedDeviceCount": 2,
  "intendedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```




