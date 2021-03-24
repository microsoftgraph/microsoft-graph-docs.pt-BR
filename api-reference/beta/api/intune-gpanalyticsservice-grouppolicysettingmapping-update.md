---
title: Atualizar groupPolicySettingMapping
description: Atualize as propriedades de um objeto groupPolicySettingMapping.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 82575a97badaba93f179c841502727e07ebff0af
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149825"
---
# <a name="update-grouppolicysettingmapping"></a><span data-ttu-id="f8bdd-103">Atualizar groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="f8bdd-103">Update groupPolicySettingMapping</span></span>

<span data-ttu-id="f8bdd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8bdd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8bdd-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8bdd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8bdd-107">Atualize as propriedades de [um objeto groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)</span><span class="sxs-lookup"><span data-stu-id="f8bdd-107">Update the properties of a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8bdd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8bdd-108">Prerequisites</span></span>
<span data-ttu-id="f8bdd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8bdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8bdd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8bdd-111">Permission type</span></span>|<span data-ttu-id="f8bdd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f8bdd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8bdd-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8bdd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8bdd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8bdd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f8bdd-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8bdd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8bdd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-116">Not supported.</span></span>|
|<span data-ttu-id="f8bdd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8bdd-117">Application</span></span>|<span data-ttu-id="f8bdd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8bdd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8bdd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8bdd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

## <a name="request-headers"></a><span data-ttu-id="f8bdd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8bdd-120">Request headers</span></span>
|<span data-ttu-id="f8bdd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8bdd-121">Header</span></span>|<span data-ttu-id="f8bdd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f8bdd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8bdd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8bdd-123">Authorization</span></span>|<span data-ttu-id="f8bdd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8bdd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f8bdd-125">Accept</span></span>|<span data-ttu-id="f8bdd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8bdd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8bdd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8bdd-127">Request body</span></span>
<span data-ttu-id="f8bdd-128">No corpo da solicitação, fornece uma representação JSON para o [objeto groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)</span><span class="sxs-lookup"><span data-stu-id="f8bdd-128">In the request body, supply a JSON representation for the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

<span data-ttu-id="f8bdd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span><span class="sxs-lookup"><span data-stu-id="f8bdd-129">The following table shows the properties that are required when you create the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span></span>

|<span data-ttu-id="f8bdd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8bdd-130">Property</span></span>|<span data-ttu-id="f8bdd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8bdd-131">Type</span></span>|<span data-ttu-id="f8bdd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8bdd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8bdd-133">id</span><span class="sxs-lookup"><span data-stu-id="f8bdd-133">id</span></span>|<span data-ttu-id="f8bdd-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8bdd-134">String</span></span>|<span data-ttu-id="f8bdd-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f8bdd-135">Not yet documented</span></span>|
|<span data-ttu-id="f8bdd-136">parentId</span><span class="sxs-lookup"><span data-stu-id="f8bdd-136">parentId</span></span>|<span data-ttu-id="f8bdd-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8bdd-137">String</span></span>|<span data-ttu-id="f8bdd-138">ID pai da configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-138">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="f8bdd-139">childIdList</span><span class="sxs-lookup"><span data-stu-id="f8bdd-139">childIdList</span></span>|<span data-ttu-id="f8bdd-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8bdd-140">String collection</span></span>|<span data-ttu-id="f8bdd-141">Lista de IDs Filho da configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-141">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="f8bdd-142">settingName</span><span class="sxs-lookup"><span data-stu-id="f8bdd-142">settingName</span></span>|<span data-ttu-id="f8bdd-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8bdd-143">String</span></span>|<span data-ttu-id="f8bdd-144">O nome dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-144">The name of this group policy setting.</span></span>|
|<span data-ttu-id="f8bdd-145">settingValue</span><span class="sxs-lookup"><span data-stu-id="f8bdd-145">settingValue</span></span>|<span data-ttu-id="f8bdd-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8bdd-146">String</span></span>|<span data-ttu-id="f8bdd-147">O valor dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-147">The value of this group policy setting.</span></span>|
|<span data-ttu-id="f8bdd-148">settingValueType</span><span class="sxs-lookup"><span data-stu-id="f8bdd-148">settingValueType</span></span>|<span data-ttu-id="f8bdd-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8bdd-149">String</span></span>|<span data-ttu-id="f8bdd-150">O tipo de valor dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-150">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="f8bdd-151">settingDisplayName</span><span class="sxs-lookup"><span data-stu-id="f8bdd-151">settingDisplayName</span></span>|<span data-ttu-id="f8bdd-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8bdd-152">String</span></span>|<span data-ttu-id="f8bdd-153">O nome de exibição dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-153">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="f8bdd-154">settingDisplayValue</span><span class="sxs-lookup"><span data-stu-id="f8bdd-154">settingDisplayValue</span></span>|<span data-ttu-id="f8bdd-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8bdd-155">String</span></span>|<span data-ttu-id="f8bdd-156">O valor de exibição dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-156">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="f8bdd-157">settingDisplayValueType</span><span class="sxs-lookup"><span data-stu-id="f8bdd-157">settingDisplayValueType</span></span>|<span data-ttu-id="f8bdd-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8bdd-158">String</span></span>|<span data-ttu-id="f8bdd-159">O tipo de valor de exibição dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-159">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="f8bdd-160">settingValueDisplayUnits</span><span class="sxs-lookup"><span data-stu-id="f8bdd-160">settingValueDisplayUnits</span></span>|<span data-ttu-id="f8bdd-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8bdd-161">String</span></span>|<span data-ttu-id="f8bdd-162">As unidades de exibição desse valor de configuração de política de grupo</span><span class="sxs-lookup"><span data-stu-id="f8bdd-162">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="f8bdd-163">settingCategory</span><span class="sxs-lookup"><span data-stu-id="f8bdd-163">settingCategory</span></span>|<span data-ttu-id="f8bdd-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8bdd-164">String</span></span>|<span data-ttu-id="f8bdd-165">A categoria em que a configuração da política de grupo está.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-165">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="f8bdd-166">mdmCspName</span><span class="sxs-lookup"><span data-stu-id="f8bdd-166">mdmCspName</span></span>|<span data-ttu-id="f8bdd-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8bdd-167">String</span></span>|<span data-ttu-id="f8bdd-168">O nome CSP para o que a configuração da política de grupo mapeia.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-168">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="f8bdd-169">mdmSettingUri</span><span class="sxs-lookup"><span data-stu-id="f8bdd-169">mdmSettingUri</span></span>|<span data-ttu-id="f8bdd-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8bdd-170">String</span></span>|<span data-ttu-id="f8bdd-171">O URI CSP do MDM para o que a política de grupo mapeia.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-171">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="f8bdd-172">mdmMinimumOSVersion</span><span class="sxs-lookup"><span data-stu-id="f8bdd-172">mdmMinimumOSVersion</span></span>|<span data-ttu-id="f8bdd-173">Int32</span><span class="sxs-lookup"><span data-stu-id="f8bdd-173">Int32</span></span>|<span data-ttu-id="f8bdd-174">A versão mínima do sistema operacional compatível com essa configuração mdm.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-174">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="f8bdd-175">settingType</span><span class="sxs-lookup"><span data-stu-id="f8bdd-175">settingType</span></span>|[<span data-ttu-id="f8bdd-176">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="f8bdd-176">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="f8bdd-177">O tipo de configuração (segurança ou admx) da Política de Grupo.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-177">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="f8bdd-178">Os valores possíveis são: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-178">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="f8bdd-179">isMdmSupported</span><span class="sxs-lookup"><span data-stu-id="f8bdd-179">isMdmSupported</span></span>|<span data-ttu-id="f8bdd-180">Booleano</span><span class="sxs-lookup"><span data-stu-id="f8bdd-180">Boolean</span></span>|<span data-ttu-id="f8bdd-181">Indica se a configuração é suportada pelo Intune ou não</span><span class="sxs-lookup"><span data-stu-id="f8bdd-181">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="f8bdd-182">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="f8bdd-182">mdmSupportedState</span></span>|[<span data-ttu-id="f8bdd-183">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="f8bdd-183">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="f8bdd-184">Indica se a configuração é suportada no Mdm ou não.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-184">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="f8bdd-185">Os valores possíveis são: `unknown`, `supported`, `unsupported`, `deprecated`.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-185">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="f8bdd-186">settingScope</span><span class="sxs-lookup"><span data-stu-id="f8bdd-186">settingScope</span></span>|[<span data-ttu-id="f8bdd-187">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="f8bdd-187">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="f8bdd-188">O escopo da configuração.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-188">The scope of the setting.</span></span> <span data-ttu-id="f8bdd-189">Os valores possíveis são: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-189">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="f8bdd-190">intuneSettingUriList</span><span class="sxs-lookup"><span data-stu-id="f8bdd-190">intuneSettingUriList</span></span>|<span data-ttu-id="f8bdd-191">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8bdd-191">String collection</span></span>|<span data-ttu-id="f8bdd-192">A lista de URIs de configuração do Intune para as configurações de política de grupo mapeia para</span><span class="sxs-lookup"><span data-stu-id="f8bdd-192">The list of Intune Setting URIs this group policy setting maps to</span></span>|
|<span data-ttu-id="f8bdd-193">intuneSettingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f8bdd-193">intuneSettingDefinitionId</span></span>|<span data-ttu-id="f8bdd-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8bdd-194">String</span></span>|<span data-ttu-id="f8bdd-195">A ID de Definição de Configuração do Intune</span><span class="sxs-lookup"><span data-stu-id="f8bdd-195">The Intune Setting Definition Id</span></span>|
|<span data-ttu-id="f8bdd-196">admxSettingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f8bdd-196">admxSettingDefinitionId</span></span>|<span data-ttu-id="f8bdd-197">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8bdd-197">String</span></span>|<span data-ttu-id="f8bdd-198">ID da Política de Grupo Admx</span><span class="sxs-lookup"><span data-stu-id="f8bdd-198">Admx Group Policy Id</span></span>|



## <a name="response"></a><span data-ttu-id="f8bdd-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8bdd-199">Response</span></span>
<span data-ttu-id="f8bdd-200">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-200">If successful, this method returns a `200 OK` response code and an updated [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8bdd-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8bdd-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8bdd-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8bdd-202">Request</span></span>
<span data-ttu-id="f8bdd-203">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-203">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
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

### <a name="response"></a><span data-ttu-id="f8bdd-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8bdd-204">Response</span></span>
<span data-ttu-id="f8bdd-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8bdd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




