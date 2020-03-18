---
title: Atualizar groupPolicySettingMapping
description: Atualiza as propriedades de um objeto groupPolicySettingMapping.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a98970a6bef6a17ab134322d1b9d41bfcd195ef5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804573"
---
# <a name="update-grouppolicysettingmapping"></a><span data-ttu-id="63066-103">Atualizar groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="63066-103">Update groupPolicySettingMapping</span></span>

> <span data-ttu-id="63066-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="63066-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63066-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63066-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63066-106">Atualiza as propriedades de um objeto [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .</span><span class="sxs-lookup"><span data-stu-id="63066-106">Update the properties of a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63066-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63066-107">Prerequisites</span></span>
<span data-ttu-id="63066-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63066-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63066-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63066-110">Permission type</span></span>|<span data-ttu-id="63066-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="63066-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63066-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63066-112">Delegated (work or school account)</span></span>|<span data-ttu-id="63066-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63066-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="63066-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63066-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63066-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63066-115">Not supported.</span></span>|
|<span data-ttu-id="63066-116">Application</span><span class="sxs-lookup"><span data-stu-id="63066-116">Application</span></span>|<span data-ttu-id="63066-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63066-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63066-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63066-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

## <a name="request-headers"></a><span data-ttu-id="63066-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63066-119">Request headers</span></span>
|<span data-ttu-id="63066-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63066-120">Header</span></span>|<span data-ttu-id="63066-121">Valor</span><span class="sxs-lookup"><span data-stu-id="63066-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63066-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="63066-122">Authorization</span></span>|<span data-ttu-id="63066-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63066-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63066-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="63066-124">Accept</span></span>|<span data-ttu-id="63066-125">application/json</span><span class="sxs-lookup"><span data-stu-id="63066-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63066-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63066-126">Request body</span></span>
<span data-ttu-id="63066-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .</span><span class="sxs-lookup"><span data-stu-id="63066-127">In the request body, supply a JSON representation for the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

<span data-ttu-id="63066-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span><span class="sxs-lookup"><span data-stu-id="63066-128">The following table shows the properties that are required when you create the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span></span>

|<span data-ttu-id="63066-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63066-129">Property</span></span>|<span data-ttu-id="63066-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="63066-130">Type</span></span>|<span data-ttu-id="63066-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="63066-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63066-132">id</span><span class="sxs-lookup"><span data-stu-id="63066-132">id</span></span>|<span data-ttu-id="63066-133">String</span><span class="sxs-lookup"><span data-stu-id="63066-133">String</span></span>|<span data-ttu-id="63066-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="63066-134">Not yet documented</span></span>|
|<span data-ttu-id="63066-135">parentId</span><span class="sxs-lookup"><span data-stu-id="63066-135">parentId</span></span>|<span data-ttu-id="63066-136">String</span><span class="sxs-lookup"><span data-stu-id="63066-136">String</span></span>|<span data-ttu-id="63066-137">ID pai da configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="63066-137">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="63066-138">childIdList</span><span class="sxs-lookup"><span data-stu-id="63066-138">childIdList</span></span>|<span data-ttu-id="63066-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="63066-139">String collection</span></span>|<span data-ttu-id="63066-140">Lista de IDs filhos da configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="63066-140">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="63066-141">settingName</span><span class="sxs-lookup"><span data-stu-id="63066-141">settingName</span></span>|<span data-ttu-id="63066-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63066-142">String</span></span>|<span data-ttu-id="63066-143">O nome dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="63066-143">The name of this group policy setting.</span></span>|
|<span data-ttu-id="63066-144">settingValue</span><span class="sxs-lookup"><span data-stu-id="63066-144">settingValue</span></span>|<span data-ttu-id="63066-145">String</span><span class="sxs-lookup"><span data-stu-id="63066-145">String</span></span>|<span data-ttu-id="63066-146">O valor dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="63066-146">The value of this group policy setting.</span></span>|
|<span data-ttu-id="63066-147">settingValueType</span><span class="sxs-lookup"><span data-stu-id="63066-147">settingValueType</span></span>|<span data-ttu-id="63066-148">String</span><span class="sxs-lookup"><span data-stu-id="63066-148">String</span></span>|<span data-ttu-id="63066-149">O tipo de valor dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="63066-149">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="63066-150">settingDisplayName</span><span class="sxs-lookup"><span data-stu-id="63066-150">settingDisplayName</span></span>|<span data-ttu-id="63066-151">String</span><span class="sxs-lookup"><span data-stu-id="63066-151">String</span></span>|<span data-ttu-id="63066-152">O nome de exibição dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="63066-152">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="63066-153">settingDisplayValue</span><span class="sxs-lookup"><span data-stu-id="63066-153">settingDisplayValue</span></span>|<span data-ttu-id="63066-154">String</span><span class="sxs-lookup"><span data-stu-id="63066-154">String</span></span>|<span data-ttu-id="63066-155">O valor de exibição dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="63066-155">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="63066-156">settingDisplayValueType</span><span class="sxs-lookup"><span data-stu-id="63066-156">settingDisplayValueType</span></span>|<span data-ttu-id="63066-157">String</span><span class="sxs-lookup"><span data-stu-id="63066-157">String</span></span>|<span data-ttu-id="63066-158">O tipo de valor de exibição dessa configuração de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="63066-158">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="63066-159">settingValueDisplayUnits</span><span class="sxs-lookup"><span data-stu-id="63066-159">settingValueDisplayUnits</span></span>|<span data-ttu-id="63066-160">String</span><span class="sxs-lookup"><span data-stu-id="63066-160">String</span></span>|<span data-ttu-id="63066-161">As unidades de exibição desse valor de configuração da política de grupo</span><span class="sxs-lookup"><span data-stu-id="63066-161">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="63066-162">settingCategory</span><span class="sxs-lookup"><span data-stu-id="63066-162">settingCategory</span></span>|<span data-ttu-id="63066-163">String</span><span class="sxs-lookup"><span data-stu-id="63066-163">String</span></span>|<span data-ttu-id="63066-164">A categoria em que a configuração da política de grupo está.</span><span class="sxs-lookup"><span data-stu-id="63066-164">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="63066-165">mdmCspName</span><span class="sxs-lookup"><span data-stu-id="63066-165">mdmCspName</span></span>|<span data-ttu-id="63066-166">String</span><span class="sxs-lookup"><span data-stu-id="63066-166">String</span></span>|<span data-ttu-id="63066-167">O nome do CSP para o qual esta configuração de política de grupo é mapeada.</span><span class="sxs-lookup"><span data-stu-id="63066-167">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="63066-168">mdmSettingUri</span><span class="sxs-lookup"><span data-stu-id="63066-168">mdmSettingUri</span></span>|<span data-ttu-id="63066-169">String</span><span class="sxs-lookup"><span data-stu-id="63066-169">String</span></span>|<span data-ttu-id="63066-170">O URI de CSP do MDM para o qual essa configuração de política de grupo é mapeada.</span><span class="sxs-lookup"><span data-stu-id="63066-170">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="63066-171">mdmMinimumOSVersion</span><span class="sxs-lookup"><span data-stu-id="63066-171">mdmMinimumOSVersion</span></span>|<span data-ttu-id="63066-172">Int32</span><span class="sxs-lookup"><span data-stu-id="63066-172">Int32</span></span>|<span data-ttu-id="63066-173">A versão mínima do sistema operacional para a qual esta configuração MDM oferece suporte.</span><span class="sxs-lookup"><span data-stu-id="63066-173">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="63066-174">SettingType</span><span class="sxs-lookup"><span data-stu-id="63066-174">settingType</span></span>|[<span data-ttu-id="63066-175">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="63066-175">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="63066-176">O tipo de configuração (segurança ou ADMX) da política de grupo.</span><span class="sxs-lookup"><span data-stu-id="63066-176">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="63066-177">Os valores possíveis são: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span><span class="sxs-lookup"><span data-stu-id="63066-177">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="63066-178">isMdmSupported</span><span class="sxs-lookup"><span data-stu-id="63066-178">isMdmSupported</span></span>|<span data-ttu-id="63066-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="63066-179">Boolean</span></span>|<span data-ttu-id="63066-180">Indica se a configuração é suportada pelo Intune ou não</span><span class="sxs-lookup"><span data-stu-id="63066-180">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="63066-181">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="63066-181">mdmSupportedState</span></span>|[<span data-ttu-id="63066-182">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="63066-182">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="63066-183">Indica se a configuração é suportada no MDM ou não.</span><span class="sxs-lookup"><span data-stu-id="63066-183">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="63066-184">Os valores possíveis são: `unknown`, `supported`, `unsupported`, `deprecated`.</span><span class="sxs-lookup"><span data-stu-id="63066-184">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="63066-185">settingScope</span><span class="sxs-lookup"><span data-stu-id="63066-185">settingScope</span></span>|[<span data-ttu-id="63066-186">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="63066-186">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="63066-187">O escopo da configuração.</span><span class="sxs-lookup"><span data-stu-id="63066-187">The scope of the setting.</span></span> <span data-ttu-id="63066-188">Os valores possíveis são: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="63066-188">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="63066-189">intuneSettingUriList</span><span class="sxs-lookup"><span data-stu-id="63066-189">intuneSettingUriList</span></span>|<span data-ttu-id="63066-190">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="63066-190">String collection</span></span>|<span data-ttu-id="63066-191">A lista de URIs de configuração do Intune que esta configuração de política de grupo mapeia para</span><span class="sxs-lookup"><span data-stu-id="63066-191">The list of Intune Setting URIs this group policy setting maps to</span></span>|
|<span data-ttu-id="63066-192">intuneSettingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="63066-192">intuneSettingDefinitionId</span></span>|<span data-ttu-id="63066-193">String</span><span class="sxs-lookup"><span data-stu-id="63066-193">String</span></span>|<span data-ttu-id="63066-194">A ID da definição da configuração do Intune</span><span class="sxs-lookup"><span data-stu-id="63066-194">The Intune Setting Definition Id</span></span>|



## <a name="response"></a><span data-ttu-id="63066-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="63066-195">Response</span></span>
<span data-ttu-id="63066-196">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63066-196">If successful, this method returns a `200 OK` response code and an updated [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63066-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63066-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="63066-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63066-198">Request</span></span>
<span data-ttu-id="63066-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63066-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
Content-type: application/json
Content-length: 957

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
  "intuneSettingDefinitionId": "Intune Setting Definition Id value"
}
```

### <a name="response"></a><span data-ttu-id="63066-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="63066-200">Response</span></span>
<span data-ttu-id="63066-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63066-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1006

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
  "intuneSettingDefinitionId": "Intune Setting Definition Id value"
}
```




