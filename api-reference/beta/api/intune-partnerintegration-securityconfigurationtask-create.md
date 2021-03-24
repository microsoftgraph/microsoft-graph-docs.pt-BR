---
title: Criar securityConfigurationTask
description: Crie um novo objeto securityConfigurationTask.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4eb74131d95a15dd4cad64107d7452ca4cf9f071
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134827"
---
# <a name="create-securityconfigurationtask"></a><span data-ttu-id="26da7-103">Criar securityConfigurationTask</span><span class="sxs-lookup"><span data-stu-id="26da7-103">Create securityConfigurationTask</span></span>

<span data-ttu-id="26da7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26da7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26da7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26da7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26da7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26da7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26da7-107">Crie um novo [objeto securityConfigurationTask.](../resources/intune-partnerintegration-securityconfigurationtask.md)</span><span class="sxs-lookup"><span data-stu-id="26da7-107">Create a new [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26da7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="26da7-108">Prerequisites</span></span>
<span data-ttu-id="26da7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26da7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26da7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26da7-111">Permission type</span></span>|<span data-ttu-id="26da7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26da7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26da7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26da7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26da7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26da7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="26da7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26da7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26da7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26da7-116">Not supported.</span></span>|
|<span data-ttu-id="26da7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26da7-117">Application</span></span>|<span data-ttu-id="26da7-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26da7-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26da7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26da7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a><span data-ttu-id="26da7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26da7-120">Request headers</span></span>
|<span data-ttu-id="26da7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26da7-121">Header</span></span>|<span data-ttu-id="26da7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="26da7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26da7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="26da7-123">Authorization</span></span>|<span data-ttu-id="26da7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26da7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26da7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="26da7-125">Accept</span></span>|<span data-ttu-id="26da7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26da7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26da7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26da7-127">Request body</span></span>
<span data-ttu-id="26da7-128">No corpo da solicitação, fornece uma representação JSON para o objeto securityConfigurationTask.</span><span class="sxs-lookup"><span data-stu-id="26da7-128">In the request body, supply a JSON representation for the securityConfigurationTask object.</span></span>

<span data-ttu-id="26da7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o securityConfigurationTask.</span><span class="sxs-lookup"><span data-stu-id="26da7-129">The following table shows the properties that are required when you create the securityConfigurationTask.</span></span>

|<span data-ttu-id="26da7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26da7-130">Property</span></span>|<span data-ttu-id="26da7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="26da7-131">Type</span></span>|<span data-ttu-id="26da7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="26da7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26da7-133">id</span><span class="sxs-lookup"><span data-stu-id="26da7-133">id</span></span>|<span data-ttu-id="26da7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26da7-134">String</span></span>|<span data-ttu-id="26da7-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="26da7-135">The entity key.</span></span> <span data-ttu-id="26da7-136">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="26da7-136">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="26da7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="26da7-137">displayName</span></span>|<span data-ttu-id="26da7-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26da7-138">String</span></span>|<span data-ttu-id="26da7-139">O nome.</span><span class="sxs-lookup"><span data-stu-id="26da7-139">The name.</span></span> <span data-ttu-id="26da7-140">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="26da7-140">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="26da7-141">descrição</span><span class="sxs-lookup"><span data-stu-id="26da7-141">description</span></span>|<span data-ttu-id="26da7-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26da7-142">String</span></span>|<span data-ttu-id="26da7-143">A descrição.</span><span class="sxs-lookup"><span data-stu-id="26da7-143">The description.</span></span> <span data-ttu-id="26da7-144">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="26da7-144">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="26da7-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26da7-145">createdDateTime</span></span>|<span data-ttu-id="26da7-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26da7-146">DateTimeOffset</span></span>|<span data-ttu-id="26da7-147">A data criada.</span><span class="sxs-lookup"><span data-stu-id="26da7-147">The created date.</span></span> <span data-ttu-id="26da7-148">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="26da7-148">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="26da7-149">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="26da7-149">dueDateTime</span></span>|<span data-ttu-id="26da7-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26da7-150">DateTimeOffset</span></span>|<span data-ttu-id="26da7-151">A data de vencimento.</span><span class="sxs-lookup"><span data-stu-id="26da7-151">The due date.</span></span> <span data-ttu-id="26da7-152">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="26da7-152">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="26da7-153">category</span><span class="sxs-lookup"><span data-stu-id="26da7-153">category</span></span>|[<span data-ttu-id="26da7-154">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="26da7-154">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="26da7-155">A categoria.</span><span class="sxs-lookup"><span data-stu-id="26da7-155">The category.</span></span> <span data-ttu-id="26da7-156">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="26da7-156">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="26da7-157">Os valores possíveis são: `unknown` e `advancedThreatProtection`.</span><span class="sxs-lookup"><span data-stu-id="26da7-157">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="26da7-158">prioridade</span><span class="sxs-lookup"><span data-stu-id="26da7-158">priority</span></span>|[<span data-ttu-id="26da7-159">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="26da7-159">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="26da7-160">A prioridade.</span><span class="sxs-lookup"><span data-stu-id="26da7-160">The priority.</span></span> <span data-ttu-id="26da7-161">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="26da7-161">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="26da7-162">Os valores possíveis são: `none`, `high`, `low`.</span><span class="sxs-lookup"><span data-stu-id="26da7-162">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="26da7-163">criador</span><span class="sxs-lookup"><span data-stu-id="26da7-163">creator</span></span>|<span data-ttu-id="26da7-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26da7-164">String</span></span>|<span data-ttu-id="26da7-165">O endereço de email do criador.</span><span class="sxs-lookup"><span data-stu-id="26da7-165">The email address of the creator.</span></span> <span data-ttu-id="26da7-166">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="26da7-166">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="26da7-167">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="26da7-167">creatorNotes</span></span>|<span data-ttu-id="26da7-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26da7-168">String</span></span>|<span data-ttu-id="26da7-169">Observações do criador.</span><span class="sxs-lookup"><span data-stu-id="26da7-169">Notes from the creator.</span></span> <span data-ttu-id="26da7-170">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="26da7-170">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="26da7-171">assignedTo</span><span class="sxs-lookup"><span data-stu-id="26da7-171">assignedTo</span></span>|<span data-ttu-id="26da7-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26da7-172">String</span></span>|<span data-ttu-id="26da7-173">O nome ou o email do administrador ao que essa tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="26da7-173">The name or email of the admin this task is assigned to.</span></span> <span data-ttu-id="26da7-174">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="26da7-174">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="26da7-175">status</span><span class="sxs-lookup"><span data-stu-id="26da7-175">status</span></span>|[<span data-ttu-id="26da7-176">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="26da7-176">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="26da7-177">O status.</span><span class="sxs-lookup"><span data-stu-id="26da7-177">The status.</span></span> <span data-ttu-id="26da7-178">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="26da7-178">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="26da7-179">Os valores possíveis são: `unknown`, `pending`, `active`, `completed`, `rejected`.</span><span class="sxs-lookup"><span data-stu-id="26da7-179">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|
|<span data-ttu-id="26da7-180">endpointSecurityPolicy</span><span class="sxs-lookup"><span data-stu-id="26da7-180">endpointSecurityPolicy</span></span>|[<span data-ttu-id="26da7-181">endpointSecurityConfigurationType</span><span class="sxs-lookup"><span data-stu-id="26da7-181">endpointSecurityConfigurationType</span></span>](../resources/intune-partnerintegration-endpointsecurityconfigurationtype.md)|<span data-ttu-id="26da7-182">O tipo de política de segurança do ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="26da7-182">The endpoint security policy type.</span></span> <span data-ttu-id="26da7-183">Os valores possíveis são: `unknown`, `antivirus`, `diskEncryption`, `firewall`, `endpointDetectionAndResponse`, `attackSurfaceReduction`, `accountProtection`.</span><span class="sxs-lookup"><span data-stu-id="26da7-183">Possible values are: `unknown`, `antivirus`, `diskEncryption`, `firewall`, `endpointDetectionAndResponse`, `attackSurfaceReduction`, `accountProtection`.</span></span>|
|<span data-ttu-id="26da7-184">applicablePlatform</span><span class="sxs-lookup"><span data-stu-id="26da7-184">applicablePlatform</span></span>|[<span data-ttu-id="26da7-185">endpointSecurityConfigurationApplicablePlatform</span><span class="sxs-lookup"><span data-stu-id="26da7-185">endpointSecurityConfigurationApplicablePlatform</span></span>](../resources/intune-partnerintegration-endpointsecurityconfigurationapplicableplatform.md)|<span data-ttu-id="26da7-186">A plataforma aplicável.</span><span class="sxs-lookup"><span data-stu-id="26da7-186">The applicable platform.</span></span> <span data-ttu-id="26da7-187">Os valores possíveis são: `unknown`, `macOS`, `windows10AndLater`, `windows10AndWindowsServer`.</span><span class="sxs-lookup"><span data-stu-id="26da7-187">Possible values are: `unknown`, `macOS`, `windows10AndLater`, `windows10AndWindowsServer`.</span></span>|
|<span data-ttu-id="26da7-188">endpointSecurityPolicyProfile</span><span class="sxs-lookup"><span data-stu-id="26da7-188">endpointSecurityPolicyProfile</span></span>|[<span data-ttu-id="26da7-189">endpointSecurityConfigurationProfileType</span><span class="sxs-lookup"><span data-stu-id="26da7-189">endpointSecurityConfigurationProfileType</span></span>](../resources/intune-partnerintegration-endpointsecurityconfigurationprofiletype.md)|<span data-ttu-id="26da7-190">O perfil da política de segurança do ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="26da7-190">The endpoint security policy profile.</span></span> <span data-ttu-id="26da7-191">Os valores possíveis são: `unknown` , , , , , , , , , `antivirus` , , `windowsSecurity` , , , `bitLocker` `fileVault` `firewall` , `firewallRules` `endpointDetectionAndResponse` `deviceControl` `appAndBrowserIsolation` `exploitProtection` `webProtection` `applicationControl` `attackSurfaceReductionRules` `accountProtection` .</span><span class="sxs-lookup"><span data-stu-id="26da7-191">Possible values are: `unknown`, `antivirus`, `windowsSecurity`, `bitLocker`, `fileVault`, `firewall`, `firewallRules`, `endpointDetectionAndResponse`, `deviceControl`, `appAndBrowserIsolation`, `exploitProtection`, `webProtection`, `applicationControl`, `attackSurfaceReductionRules`, `accountProtection`.</span></span>|
|<span data-ttu-id="26da7-192">insights</span><span class="sxs-lookup"><span data-stu-id="26da7-192">insights</span></span>|<span data-ttu-id="26da7-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26da7-193">String</span></span>|<span data-ttu-id="26da7-194">Informações sobre a mitigação.</span><span class="sxs-lookup"><span data-stu-id="26da7-194">Information about the mitigation.</span></span>|
|<span data-ttu-id="26da7-195">managedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26da7-195">managedDeviceCount</span></span>|<span data-ttu-id="26da7-196">Int32</span><span class="sxs-lookup"><span data-stu-id="26da7-196">Int32</span></span>|<span data-ttu-id="26da7-197">O número de dispositivos vulneráveis.</span><span class="sxs-lookup"><span data-stu-id="26da7-197">The number of vulnerable devices.</span></span>|
|<span data-ttu-id="26da7-198">intendedSettings</span><span class="sxs-lookup"><span data-stu-id="26da7-198">intendedSettings</span></span>|<span data-ttu-id="26da7-199">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="26da7-199">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="26da7-200">As configurações pretenddas e seus valores.</span><span class="sxs-lookup"><span data-stu-id="26da7-200">The intended settings and their values.</span></span>|



## <a name="response"></a><span data-ttu-id="26da7-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="26da7-201">Response</span></span>
<span data-ttu-id="26da7-202">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26da7-202">If successful, this method returns a `201 Created` response code and a [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26da7-203">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26da7-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="26da7-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26da7-204">Request</span></span>
<span data-ttu-id="26da7-205">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26da7-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
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

### <a name="response"></a><span data-ttu-id="26da7-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="26da7-206">Response</span></span>
<span data-ttu-id="26da7-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26da7-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




