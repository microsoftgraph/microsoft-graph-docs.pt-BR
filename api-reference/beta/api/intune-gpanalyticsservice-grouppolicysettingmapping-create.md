---
title: Criar groupPolicySettingMapping
description: Criar um novo objeto groupPolicySettingMapping.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b8e6a557bebac11004b5548bc90d931356ba852d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943267"
---
# <a name="create-grouppolicysettingmapping"></a><span data-ttu-id="e7554-103">Criar groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="e7554-103">Create groupPolicySettingMapping</span></span>

> <span data-ttu-id="e7554-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e7554-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7554-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e7554-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7554-106">Criar um novo objeto [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .</span><span class="sxs-lookup"><span data-stu-id="e7554-106">Create a new [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7554-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7554-107">Prerequisites</span></span>
<span data-ttu-id="e7554-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7554-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7554-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7554-110">Permission type</span></span>|<span data-ttu-id="e7554-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e7554-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7554-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7554-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7554-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7554-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7554-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7554-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7554-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7554-115">Not supported.</span></span>|
|<span data-ttu-id="e7554-116">Application</span><span class="sxs-lookup"><span data-stu-id="e7554-116">Application</span></span>|<span data-ttu-id="e7554-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7554-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7554-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7554-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

## <a name="request-headers"></a><span data-ttu-id="e7554-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7554-119">Request headers</span></span>
|<span data-ttu-id="e7554-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7554-120">Header</span></span>|<span data-ttu-id="e7554-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e7554-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7554-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7554-122">Authorization</span></span>|<span data-ttu-id="e7554-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7554-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7554-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e7554-124">Accept</span></span>|<span data-ttu-id="e7554-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7554-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7554-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7554-126">Request body</span></span>
<span data-ttu-id="e7554-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicySettingMapping.</span><span class="sxs-lookup"><span data-stu-id="e7554-127">In the request body, supply a JSON representation for the groupPolicySettingMapping object.</span></span>

<span data-ttu-id="e7554-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicySettingMapping.</span><span class="sxs-lookup"><span data-stu-id="e7554-128">The following table shows the properties that are required when you create the groupPolicySettingMapping.</span></span>

|<span data-ttu-id="e7554-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7554-129">Property</span></span>|<span data-ttu-id="e7554-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7554-130">Type</span></span>|<span data-ttu-id="e7554-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7554-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7554-132">id</span><span class="sxs-lookup"><span data-stu-id="e7554-132">id</span></span>|<span data-ttu-id="e7554-133">String</span><span class="sxs-lookup"><span data-stu-id="e7554-133">String</span></span>|<span data-ttu-id="e7554-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e7554-134">Not yet documented</span></span>|
|<span data-ttu-id="e7554-135">parentId</span><span class="sxs-lookup"><span data-stu-id="e7554-135">parentId</span></span>|<span data-ttu-id="e7554-136">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="e7554-136">String</span></span>|<span data-ttu-id="e7554-137">ID pai da configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="e7554-137">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="e7554-138">childIdList</span><span class="sxs-lookup"><span data-stu-id="e7554-138">childIdList</span></span>|<span data-ttu-id="e7554-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7554-139">String collection</span></span>|<span data-ttu-id="e7554-140">Lista de IDs filhos da configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="e7554-140">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="e7554-141">settingName</span><span class="sxs-lookup"><span data-stu-id="e7554-141">settingName</span></span>|<span data-ttu-id="e7554-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7554-142">String</span></span>|<span data-ttu-id="e7554-143">O nome dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="e7554-143">The name of this group policy setting.</span></span>|
|<span data-ttu-id="e7554-144">settingValue</span><span class="sxs-lookup"><span data-stu-id="e7554-144">settingValue</span></span>|<span data-ttu-id="e7554-145">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="e7554-145">String</span></span>|<span data-ttu-id="e7554-146">O valor dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="e7554-146">The value of this group policy setting.</span></span>|
|<span data-ttu-id="e7554-147">settingValueType</span><span class="sxs-lookup"><span data-stu-id="e7554-147">settingValueType</span></span>|<span data-ttu-id="e7554-148">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="e7554-148">String</span></span>|<span data-ttu-id="e7554-149">O tipo de valor dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="e7554-149">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="e7554-150">settingDisplayName</span><span class="sxs-lookup"><span data-stu-id="e7554-150">settingDisplayName</span></span>|<span data-ttu-id="e7554-151">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="e7554-151">String</span></span>|<span data-ttu-id="e7554-152">O nome de exibição dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="e7554-152">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="e7554-153">settingDisplayValue</span><span class="sxs-lookup"><span data-stu-id="e7554-153">settingDisplayValue</span></span>|<span data-ttu-id="e7554-154">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="e7554-154">String</span></span>|<span data-ttu-id="e7554-155">O valor de exibição dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="e7554-155">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="e7554-156">settingDisplayValueType</span><span class="sxs-lookup"><span data-stu-id="e7554-156">settingDisplayValueType</span></span>|<span data-ttu-id="e7554-157">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="e7554-157">String</span></span>|<span data-ttu-id="e7554-158">O tipo de valor de exibição dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="e7554-158">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="e7554-159">settingValueDisplayUnits</span><span class="sxs-lookup"><span data-stu-id="e7554-159">settingValueDisplayUnits</span></span>|<span data-ttu-id="e7554-160">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="e7554-160">String</span></span>|<span data-ttu-id="e7554-161">As unidades de exibição desse valor de configuração da política de grupo</span><span class="sxs-lookup"><span data-stu-id="e7554-161">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="e7554-162">settingCategory</span><span class="sxs-lookup"><span data-stu-id="e7554-162">settingCategory</span></span>|<span data-ttu-id="e7554-163">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="e7554-163">String</span></span>|<span data-ttu-id="e7554-164">A categoria em que a configuração da política de grupo está.</span><span class="sxs-lookup"><span data-stu-id="e7554-164">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="e7554-165">mdmCspName</span><span class="sxs-lookup"><span data-stu-id="e7554-165">mdmCspName</span></span>|<span data-ttu-id="e7554-166">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="e7554-166">String</span></span>|<span data-ttu-id="e7554-167">O nome do CSP para o qual esta configuração de política de grupo é mapeada.</span><span class="sxs-lookup"><span data-stu-id="e7554-167">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="e7554-168">mdmSettingUri</span><span class="sxs-lookup"><span data-stu-id="e7554-168">mdmSettingUri</span></span>|<span data-ttu-id="e7554-169">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="e7554-169">String</span></span>|<span data-ttu-id="e7554-170">O URI de CSP do MDM para o qual essa configuração de política de grupo é mapeada.</span><span class="sxs-lookup"><span data-stu-id="e7554-170">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="e7554-171">mdmMinimumOSVersion</span><span class="sxs-lookup"><span data-stu-id="e7554-171">mdmMinimumOSVersion</span></span>|<span data-ttu-id="e7554-172">Int32</span><span class="sxs-lookup"><span data-stu-id="e7554-172">Int32</span></span>|<span data-ttu-id="e7554-173">A versão mínima do sistema operacional para a qual esta configuração MDM oferece suporte.</span><span class="sxs-lookup"><span data-stu-id="e7554-173">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="e7554-174">SettingType</span><span class="sxs-lookup"><span data-stu-id="e7554-174">settingType</span></span>|[<span data-ttu-id="e7554-175">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="e7554-175">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="e7554-176">O tipo de configuração (segurança ou ADMX) da política de grupo.</span><span class="sxs-lookup"><span data-stu-id="e7554-176">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="e7554-177">Os valores possíveis são: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span><span class="sxs-lookup"><span data-stu-id="e7554-177">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="e7554-178">isMdmSupported</span><span class="sxs-lookup"><span data-stu-id="e7554-178">isMdmSupported</span></span>|<span data-ttu-id="e7554-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7554-179">Boolean</span></span>|<span data-ttu-id="e7554-180">Indica se a configuração é suportada pelo Intune ou não</span><span class="sxs-lookup"><span data-stu-id="e7554-180">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="e7554-181">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="e7554-181">mdmSupportedState</span></span>|[<span data-ttu-id="e7554-182">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="e7554-182">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="e7554-183">Indica se a configuração é suportada no MDM ou não.</span><span class="sxs-lookup"><span data-stu-id="e7554-183">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="e7554-184">Os valores possíveis são: `unknown`, `supported`, `unsupported`, `deprecated`.</span><span class="sxs-lookup"><span data-stu-id="e7554-184">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="e7554-185">settingScope</span><span class="sxs-lookup"><span data-stu-id="e7554-185">settingScope</span></span>|[<span data-ttu-id="e7554-186">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="e7554-186">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="e7554-187">O escopo da configuração.</span><span class="sxs-lookup"><span data-stu-id="e7554-187">The scope of the setting.</span></span> <span data-ttu-id="e7554-188">Os valores possíveis são: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="e7554-188">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="e7554-189">intuneSettingUriList</span><span class="sxs-lookup"><span data-stu-id="e7554-189">intuneSettingUriList</span></span>|<span data-ttu-id="e7554-190">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7554-190">String collection</span></span>|<span data-ttu-id="e7554-191">A lista de URIs de configuração do Intune que esta configuração de política de grupo mapeia para</span><span class="sxs-lookup"><span data-stu-id="e7554-191">The list of Intune Setting URIs this group policy setting maps to</span></span>|



## <a name="response"></a><span data-ttu-id="e7554-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7554-192">Response</span></span>
<span data-ttu-id="e7554-193">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7554-193">If successful, this method returns a `201 Created` response code and a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7554-194">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7554-194">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7554-195">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7554-195">Request</span></span>
<span data-ttu-id="e7554-196">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7554-196">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
Content-type: application/json
Content-length: 887

{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "parentId": "Parent Id value",
  "childIdList": [
    "Child Id List value"
  ],
  "settingName": "Setting Name value",
  "settingValue": "Setting Value value",
  "settingValueType": "Setting Value Type value",
  "settingDisplayName": "Setting Display Name value",
  "settingDisplayValue": "Setting Display Value value",
  "settingDisplayValueType": "Setting Display Value Type value",
  "settingValueDisplayUnits": "Setting Value Display Units value",
  "settingCategory": "Setting Category value",
  "mdmCspName": "Mdm Csp Name value",
  "mdmSettingUri": "Mdm Setting Uri value",
  "mdmMinimumOSVersion": 3,
  "settingType": "policy",
  "isMdmSupported": true,
  "mdmSupportedState": "supported",
  "settingScope": "device",
  "intuneSettingUriList": [
    "Intune Setting Uri List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="e7554-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7554-197">Response</span></span>
<span data-ttu-id="e7554-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7554-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 936

{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "id": "8fa04560-4560-8fa0-6045-a08f6045a08f",
  "parentId": "Parent Id value",
  "childIdList": [
    "Child Id List value"
  ],
  "settingName": "Setting Name value",
  "settingValue": "Setting Value value",
  "settingValueType": "Setting Value Type value",
  "settingDisplayName": "Setting Display Name value",
  "settingDisplayValue": "Setting Display Value value",
  "settingDisplayValueType": "Setting Display Value Type value",
  "settingValueDisplayUnits": "Setting Value Display Units value",
  "settingCategory": "Setting Category value",
  "mdmCspName": "Mdm Csp Name value",
  "mdmSettingUri": "Mdm Setting Uri value",
  "mdmMinimumOSVersion": 3,
  "settingType": "policy",
  "isMdmSupported": true,
  "mdmSupportedState": "supported",
  "settingScope": "device",
  "intuneSettingUriList": [
    "Intune Setting Uri List value"
  ]
}
```





