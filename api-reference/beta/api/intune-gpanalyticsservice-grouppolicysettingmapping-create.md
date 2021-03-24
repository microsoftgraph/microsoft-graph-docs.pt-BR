---
title: Criar groupPolicySettingMapping
description: Crie um novo objeto groupPolicySettingMapping.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26639ae0547cc9cb81c10b370f1323b4d5f8663c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135520"
---
# <a name="create-grouppolicysettingmapping"></a><span data-ttu-id="a1da2-103">Criar groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="a1da2-103">Create groupPolicySettingMapping</span></span>

<span data-ttu-id="a1da2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1da2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1da2-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1da2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1da2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1da2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1da2-107">Crie um novo [objeto groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)</span><span class="sxs-lookup"><span data-stu-id="a1da2-107">Create a new [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1da2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1da2-108">Prerequisites</span></span>
<span data-ttu-id="a1da2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1da2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1da2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1da2-111">Permission type</span></span>|<span data-ttu-id="a1da2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1da2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1da2-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1da2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1da2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1da2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1da2-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1da2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1da2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1da2-116">Not supported.</span></span>|
|<span data-ttu-id="a1da2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1da2-117">Application</span></span>|<span data-ttu-id="a1da2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1da2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1da2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1da2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

## <a name="request-headers"></a><span data-ttu-id="a1da2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1da2-120">Request headers</span></span>
|<span data-ttu-id="a1da2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1da2-121">Header</span></span>|<span data-ttu-id="a1da2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a1da2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1da2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1da2-123">Authorization</span></span>|<span data-ttu-id="a1da2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1da2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1da2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1da2-125">Accept</span></span>|<span data-ttu-id="a1da2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1da2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1da2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1da2-127">Request body</span></span>
<span data-ttu-id="a1da2-128">No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicySettingMapping.</span><span class="sxs-lookup"><span data-stu-id="a1da2-128">In the request body, supply a JSON representation for the groupPolicySettingMapping object.</span></span>

<span data-ttu-id="a1da2-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicySettingMapping.</span><span class="sxs-lookup"><span data-stu-id="a1da2-129">The following table shows the properties that are required when you create the groupPolicySettingMapping.</span></span>

|<span data-ttu-id="a1da2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1da2-130">Property</span></span>|<span data-ttu-id="a1da2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1da2-131">Type</span></span>|<span data-ttu-id="a1da2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1da2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1da2-133">id</span><span class="sxs-lookup"><span data-stu-id="a1da2-133">id</span></span>|<span data-ttu-id="a1da2-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1da2-134">String</span></span>|<span data-ttu-id="a1da2-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a1da2-135">Not yet documented</span></span>|
|<span data-ttu-id="a1da2-136">parentId</span><span class="sxs-lookup"><span data-stu-id="a1da2-136">parentId</span></span>|<span data-ttu-id="a1da2-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1da2-137">String</span></span>|<span data-ttu-id="a1da2-138">ID pai da configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="a1da2-138">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="a1da2-139">childIdList</span><span class="sxs-lookup"><span data-stu-id="a1da2-139">childIdList</span></span>|<span data-ttu-id="a1da2-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1da2-140">String collection</span></span>|<span data-ttu-id="a1da2-141">Lista de IDs Filho da configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="a1da2-141">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="a1da2-142">settingName</span><span class="sxs-lookup"><span data-stu-id="a1da2-142">settingName</span></span>|<span data-ttu-id="a1da2-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1da2-143">String</span></span>|<span data-ttu-id="a1da2-144">O nome dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="a1da2-144">The name of this group policy setting.</span></span>|
|<span data-ttu-id="a1da2-145">settingValue</span><span class="sxs-lookup"><span data-stu-id="a1da2-145">settingValue</span></span>|<span data-ttu-id="a1da2-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1da2-146">String</span></span>|<span data-ttu-id="a1da2-147">O valor dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="a1da2-147">The value of this group policy setting.</span></span>|
|<span data-ttu-id="a1da2-148">settingValueType</span><span class="sxs-lookup"><span data-stu-id="a1da2-148">settingValueType</span></span>|<span data-ttu-id="a1da2-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1da2-149">String</span></span>|<span data-ttu-id="a1da2-150">O tipo de valor dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="a1da2-150">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="a1da2-151">settingDisplayName</span><span class="sxs-lookup"><span data-stu-id="a1da2-151">settingDisplayName</span></span>|<span data-ttu-id="a1da2-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1da2-152">String</span></span>|<span data-ttu-id="a1da2-153">O nome de exibição dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="a1da2-153">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="a1da2-154">settingDisplayValue</span><span class="sxs-lookup"><span data-stu-id="a1da2-154">settingDisplayValue</span></span>|<span data-ttu-id="a1da2-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1da2-155">String</span></span>|<span data-ttu-id="a1da2-156">O valor de exibição dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="a1da2-156">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="a1da2-157">settingDisplayValueType</span><span class="sxs-lookup"><span data-stu-id="a1da2-157">settingDisplayValueType</span></span>|<span data-ttu-id="a1da2-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1da2-158">String</span></span>|<span data-ttu-id="a1da2-159">O tipo de valor de exibição dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="a1da2-159">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="a1da2-160">settingValueDisplayUnits</span><span class="sxs-lookup"><span data-stu-id="a1da2-160">settingValueDisplayUnits</span></span>|<span data-ttu-id="a1da2-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1da2-161">String</span></span>|<span data-ttu-id="a1da2-162">As unidades de exibição desse valor de configuração de política de grupo</span><span class="sxs-lookup"><span data-stu-id="a1da2-162">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="a1da2-163">settingCategory</span><span class="sxs-lookup"><span data-stu-id="a1da2-163">settingCategory</span></span>|<span data-ttu-id="a1da2-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1da2-164">String</span></span>|<span data-ttu-id="a1da2-165">A categoria em que a configuração da política de grupo está.</span><span class="sxs-lookup"><span data-stu-id="a1da2-165">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="a1da2-166">mdmCspName</span><span class="sxs-lookup"><span data-stu-id="a1da2-166">mdmCspName</span></span>|<span data-ttu-id="a1da2-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1da2-167">String</span></span>|<span data-ttu-id="a1da2-168">O nome CSP para o que a configuração da política de grupo mapeia.</span><span class="sxs-lookup"><span data-stu-id="a1da2-168">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="a1da2-169">mdmSettingUri</span><span class="sxs-lookup"><span data-stu-id="a1da2-169">mdmSettingUri</span></span>|<span data-ttu-id="a1da2-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1da2-170">String</span></span>|<span data-ttu-id="a1da2-171">O URI CSP do MDM para o que a política de grupo mapeia.</span><span class="sxs-lookup"><span data-stu-id="a1da2-171">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="a1da2-172">mdmMinimumOSVersion</span><span class="sxs-lookup"><span data-stu-id="a1da2-172">mdmMinimumOSVersion</span></span>|<span data-ttu-id="a1da2-173">Int32</span><span class="sxs-lookup"><span data-stu-id="a1da2-173">Int32</span></span>|<span data-ttu-id="a1da2-174">A versão mínima do sistema operacional compatível com essa configuração mdm.</span><span class="sxs-lookup"><span data-stu-id="a1da2-174">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="a1da2-175">settingType</span><span class="sxs-lookup"><span data-stu-id="a1da2-175">settingType</span></span>|[<span data-ttu-id="a1da2-176">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="a1da2-176">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="a1da2-177">O tipo de configuração (segurança ou admx) da Política de Grupo.</span><span class="sxs-lookup"><span data-stu-id="a1da2-177">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="a1da2-178">Os valores possíveis são: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span><span class="sxs-lookup"><span data-stu-id="a1da2-178">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="a1da2-179">isMdmSupported</span><span class="sxs-lookup"><span data-stu-id="a1da2-179">isMdmSupported</span></span>|<span data-ttu-id="a1da2-180">Booleano</span><span class="sxs-lookup"><span data-stu-id="a1da2-180">Boolean</span></span>|<span data-ttu-id="a1da2-181">Indica se a configuração é suportada pelo Intune ou não</span><span class="sxs-lookup"><span data-stu-id="a1da2-181">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="a1da2-182">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="a1da2-182">mdmSupportedState</span></span>|[<span data-ttu-id="a1da2-183">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="a1da2-183">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="a1da2-184">Indica se a configuração é suportada no Mdm ou não.</span><span class="sxs-lookup"><span data-stu-id="a1da2-184">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="a1da2-185">Os valores possíveis são: `unknown`, `supported`, `unsupported`, `deprecated`.</span><span class="sxs-lookup"><span data-stu-id="a1da2-185">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="a1da2-186">settingScope</span><span class="sxs-lookup"><span data-stu-id="a1da2-186">settingScope</span></span>|[<span data-ttu-id="a1da2-187">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="a1da2-187">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="a1da2-188">O escopo da configuração.</span><span class="sxs-lookup"><span data-stu-id="a1da2-188">The scope of the setting.</span></span> <span data-ttu-id="a1da2-189">Os valores possíveis são: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="a1da2-189">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="a1da2-190">intuneSettingUriList</span><span class="sxs-lookup"><span data-stu-id="a1da2-190">intuneSettingUriList</span></span>|<span data-ttu-id="a1da2-191">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1da2-191">String collection</span></span>|<span data-ttu-id="a1da2-192">A lista de URIs de configuração do Intune para as configurações de política de grupo mapeia para</span><span class="sxs-lookup"><span data-stu-id="a1da2-192">The list of Intune Setting URIs this group policy setting maps to</span></span>|
|<span data-ttu-id="a1da2-193">intuneSettingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a1da2-193">intuneSettingDefinitionId</span></span>|<span data-ttu-id="a1da2-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1da2-194">String</span></span>|<span data-ttu-id="a1da2-195">A ID de Definição de Configuração do Intune</span><span class="sxs-lookup"><span data-stu-id="a1da2-195">The Intune Setting Definition Id</span></span>|
|<span data-ttu-id="a1da2-196">admxSettingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a1da2-196">admxSettingDefinitionId</span></span>|<span data-ttu-id="a1da2-197">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1da2-197">String</span></span>|<span data-ttu-id="a1da2-198">ID da Política de Grupo Admx</span><span class="sxs-lookup"><span data-stu-id="a1da2-198">Admx Group Policy Id</span></span>|



## <a name="response"></a><span data-ttu-id="a1da2-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1da2-199">Response</span></span>
<span data-ttu-id="a1da2-200">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1da2-200">If successful, this method returns a `201 Created` response code and a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1da2-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1da2-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1da2-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1da2-202">Request</span></span>
<span data-ttu-id="a1da2-203">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1da2-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
Content-type: application/json
Content-length: 1023

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
  ],
  "intuneSettingDefinitionId": "Intune Setting Definition Id value",
  "admxSettingDefinitionId": "Admx Setting Definition Id value"
}
```

### <a name="response"></a><span data-ttu-id="a1da2-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1da2-204">Response</span></span>
<span data-ttu-id="a1da2-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1da2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1072

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
  ],
  "intuneSettingDefinitionId": "Intune Setting Definition Id value",
  "admxSettingDefinitionId": "Admx Setting Definition Id value"
}
```




