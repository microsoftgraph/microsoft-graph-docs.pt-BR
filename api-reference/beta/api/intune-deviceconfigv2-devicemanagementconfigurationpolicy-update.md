---
title: Atualizar deviceManagementConfigurationPolicy
description: Atualize as propriedades de um objeto deviceManagementConfigurationPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b72cc45d68b4070b909ca2c3eb0c315dec6768db
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666117"
---
# <a name="update-devicemanagementconfigurationpolicy"></a><span data-ttu-id="61de1-103">Atualizar deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="61de1-103">Update deviceManagementConfigurationPolicy</span></span>

<span data-ttu-id="61de1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61de1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61de1-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="61de1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61de1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="61de1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61de1-107">Atualize as propriedades de [um objeto deviceManagementConfigurationPolicy.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="61de1-107">Update the properties of a [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61de1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61de1-108">Prerequisites</span></span>
<span data-ttu-id="61de1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61de1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61de1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61de1-111">Permission type</span></span>|<span data-ttu-id="61de1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61de1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61de1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61de1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="61de1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61de1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="61de1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61de1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61de1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61de1-116">Not supported.</span></span>|
|<span data-ttu-id="61de1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61de1-117">Application</span></span>|<span data-ttu-id="61de1-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61de1-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="61de1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61de1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}
PATCH /deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}/referencingConfigurationPolicies/{deviceManagementConfigurationPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="61de1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61de1-120">Request headers</span></span>
|<span data-ttu-id="61de1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="61de1-121">Header</span></span>|<span data-ttu-id="61de1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="61de1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61de1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="61de1-123">Authorization</span></span>|<span data-ttu-id="61de1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61de1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61de1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="61de1-125">Accept</span></span>|<span data-ttu-id="61de1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="61de1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61de1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61de1-127">Request body</span></span>
<span data-ttu-id="61de1-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementConfigurationPolicy.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="61de1-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object.</span></span>

<span data-ttu-id="61de1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="61de1-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md).</span></span>

|<span data-ttu-id="61de1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61de1-130">Property</span></span>|<span data-ttu-id="61de1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="61de1-131">Type</span></span>|<span data-ttu-id="61de1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="61de1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61de1-133">id</span><span class="sxs-lookup"><span data-stu-id="61de1-133">id</span></span>|<span data-ttu-id="61de1-134">String</span><span class="sxs-lookup"><span data-stu-id="61de1-134">String</span></span>|<span data-ttu-id="61de1-135">Chave do documento de política.</span><span class="sxs-lookup"><span data-stu-id="61de1-135">Key of the policy document.</span></span> <span data-ttu-id="61de1-136">Gerado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="61de1-136">Automatically generated.</span></span>|
|<span data-ttu-id="61de1-137">nome</span><span class="sxs-lookup"><span data-stu-id="61de1-137">name</span></span>|<span data-ttu-id="61de1-138">String</span><span class="sxs-lookup"><span data-stu-id="61de1-138">String</span></span>|<span data-ttu-id="61de1-139">Nome da política</span><span class="sxs-lookup"><span data-stu-id="61de1-139">Policy name</span></span>|
|<span data-ttu-id="61de1-140">descrição</span><span class="sxs-lookup"><span data-stu-id="61de1-140">description</span></span>|<span data-ttu-id="61de1-141">String</span><span class="sxs-lookup"><span data-stu-id="61de1-141">String</span></span>|<span data-ttu-id="61de1-142">Descrição da política</span><span class="sxs-lookup"><span data-stu-id="61de1-142">Policy description</span></span>|
|<span data-ttu-id="61de1-143">plataformas</span><span class="sxs-lookup"><span data-stu-id="61de1-143">platforms</span></span>|[<span data-ttu-id="61de1-144">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="61de1-144">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="61de1-145">Plataformas para essa política.</span><span class="sxs-lookup"><span data-stu-id="61de1-145">Platforms for this policy.</span></span> <span data-ttu-id="61de1-146">Os valores possíveis são: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="61de1-146">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="61de1-147">technologies</span><span class="sxs-lookup"><span data-stu-id="61de1-147">technologies</span></span>|[<span data-ttu-id="61de1-148">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="61de1-148">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="61de1-149">Tecnologias para essa política.</span><span class="sxs-lookup"><span data-stu-id="61de1-149">Technologies for this policy.</span></span> <span data-ttu-id="61de1-150">Os valores possíveis são: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span><span class="sxs-lookup"><span data-stu-id="61de1-150">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span></span>|
|<span data-ttu-id="61de1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61de1-151">createdDateTime</span></span>|<span data-ttu-id="61de1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61de1-152">DateTimeOffset</span></span>|<span data-ttu-id="61de1-153">Data e hora de criação de política.</span><span class="sxs-lookup"><span data-stu-id="61de1-153">Policy creation date and time.</span></span> <span data-ttu-id="61de1-154">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="61de1-154">This property is read-only.</span></span>|
|<span data-ttu-id="61de1-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61de1-155">lastModifiedDateTime</span></span>|<span data-ttu-id="61de1-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61de1-156">DateTimeOffset</span></span>|<span data-ttu-id="61de1-157">Data e hora da última modificação da política.</span><span class="sxs-lookup"><span data-stu-id="61de1-157">Policy last modification date and time.</span></span> <span data-ttu-id="61de1-158">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="61de1-158">This property is read-only.</span></span>|
|<span data-ttu-id="61de1-159">settingCount</span><span class="sxs-lookup"><span data-stu-id="61de1-159">settingCount</span></span>|<span data-ttu-id="61de1-160">Int32</span><span class="sxs-lookup"><span data-stu-id="61de1-160">Int32</span></span>|<span data-ttu-id="61de1-161">Número de configurações.</span><span class="sxs-lookup"><span data-stu-id="61de1-161">Number of settings.</span></span> <span data-ttu-id="61de1-162">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="61de1-162">This property is read-only.</span></span>|
|<span data-ttu-id="61de1-163">creationSource</span><span class="sxs-lookup"><span data-stu-id="61de1-163">creationSource</span></span>|<span data-ttu-id="61de1-164">String</span><span class="sxs-lookup"><span data-stu-id="61de1-164">String</span></span>|<span data-ttu-id="61de1-165">Fonte de criação de política</span><span class="sxs-lookup"><span data-stu-id="61de1-165">Policy creation source</span></span>|
|<span data-ttu-id="61de1-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="61de1-166">roleScopeTagIds</span></span>|<span data-ttu-id="61de1-167">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="61de1-167">String collection</span></span>|<span data-ttu-id="61de1-168">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="61de1-168">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="61de1-169">isAssigned</span><span class="sxs-lookup"><span data-stu-id="61de1-169">isAssigned</span></span>|<span data-ttu-id="61de1-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="61de1-170">Boolean</span></span>|<span data-ttu-id="61de1-171">Status da atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="61de1-171">Policy assignment status.</span></span> <span data-ttu-id="61de1-172">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="61de1-172">This property is read-only.</span></span>|
|<span data-ttu-id="61de1-173">templateReference</span><span class="sxs-lookup"><span data-stu-id="61de1-173">templateReference</span></span>|[<span data-ttu-id="61de1-174">deviceManagementConfigurationPolicyTemplateReference</span><span class="sxs-lookup"><span data-stu-id="61de1-174">deviceManagementConfigurationPolicyTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplatereference.md)|<span data-ttu-id="61de1-175">Informações de referência do modelo</span><span class="sxs-lookup"><span data-stu-id="61de1-175">Template reference information</span></span>|



## <a name="response"></a><span data-ttu-id="61de1-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="61de1-176">Response</span></span>
<span data-ttu-id="61de1-177">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61de1-177">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61de1-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61de1-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="61de1-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61de1-179">Request</span></span>
<span data-ttu-id="61de1-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61de1-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}
Content-type: application/json
Content-length: 685

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicy",
  "name": "Name value",
  "description": "Description value",
  "platforms": "macOS",
  "technologies": "mdm",
  "settingCount": 12,
  "creationSource": "Creation Source value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "isAssigned": true,
  "templateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplateReference",
    "templateId": "Template Id value",
    "templateFamily": "endpointSecurityAntivirus",
    "templateDisplayName": "Template Display Name value",
    "templateDisplayVersion": "Template Display Version value"
  }
}
```

### <a name="response"></a><span data-ttu-id="61de1-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="61de1-181">Response</span></span>
<span data-ttu-id="61de1-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61de1-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 857

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicy",
  "id": "3ffd7cd0-7cd0-3ffd-d07c-fd3fd07cfd3f",
  "name": "Name value",
  "description": "Description value",
  "platforms": "macOS",
  "technologies": "mdm",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "settingCount": 12,
  "creationSource": "Creation Source value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "isAssigned": true,
  "templateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplateReference",
    "templateId": "Template Id value",
    "templateFamily": "endpointSecurityAntivirus",
    "templateDisplayName": "Template Display Name value",
    "templateDisplayVersion": "Template Display Version value"
  }
}
```




