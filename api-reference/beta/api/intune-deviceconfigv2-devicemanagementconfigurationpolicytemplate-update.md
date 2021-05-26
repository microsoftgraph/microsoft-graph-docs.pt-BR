---
title: Atualizar deviceManagementConfigurationPolicyTemplate
description: Atualize as propriedades de um objeto deviceManagementConfigurationPolicyTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7c3856862b0706c4eb30340d76c35275eb797e68
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665627"
---
# <a name="update-devicemanagementconfigurationpolicytemplate"></a><span data-ttu-id="e69f0-103">Atualizar deviceManagementConfigurationPolicyTemplate</span><span class="sxs-lookup"><span data-stu-id="e69f0-103">Update deviceManagementConfigurationPolicyTemplate</span></span>

<span data-ttu-id="e69f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e69f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e69f0-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e69f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e69f0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e69f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e69f0-107">Atualize as propriedades de [um objeto deviceManagementConfigurationPolicyTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e69f0-107">Update the properties of a [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e69f0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e69f0-108">Prerequisites</span></span>
<span data-ttu-id="e69f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e69f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e69f0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e69f0-111">Permission type</span></span>|<span data-ttu-id="e69f0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e69f0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e69f0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e69f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e69f0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e69f0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e69f0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e69f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e69f0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e69f0-116">Not supported.</span></span>|
|<span data-ttu-id="e69f0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e69f0-117">Application</span></span>|<span data-ttu-id="e69f0-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e69f0-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e69f0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e69f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="e69f0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e69f0-120">Request headers</span></span>
|<span data-ttu-id="e69f0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e69f0-121">Header</span></span>|<span data-ttu-id="e69f0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e69f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e69f0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e69f0-123">Authorization</span></span>|<span data-ttu-id="e69f0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e69f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e69f0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e69f0-125">Accept</span></span>|<span data-ttu-id="e69f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e69f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e69f0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e69f0-127">Request body</span></span>
<span data-ttu-id="e69f0-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementConfigurationPolicyTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e69f0-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) object.</span></span>

<span data-ttu-id="e69f0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md).</span><span class="sxs-lookup"><span data-stu-id="e69f0-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md).</span></span>

|<span data-ttu-id="e69f0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e69f0-130">Property</span></span>|<span data-ttu-id="e69f0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e69f0-131">Type</span></span>|<span data-ttu-id="e69f0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e69f0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e69f0-133">id</span><span class="sxs-lookup"><span data-stu-id="e69f0-133">id</span></span>|<span data-ttu-id="e69f0-134">String</span><span class="sxs-lookup"><span data-stu-id="e69f0-134">String</span></span>|<span data-ttu-id="e69f0-135">Chave do documento do modelo, composta por BaseId e Version.</span><span class="sxs-lookup"><span data-stu-id="e69f0-135">Key of the template document, composed of BaseId and Version.</span></span> <span data-ttu-id="e69f0-136">Gerado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="e69f0-136">Automatically generated.</span></span>|
|<span data-ttu-id="e69f0-137">baseId</span><span class="sxs-lookup"><span data-stu-id="e69f0-137">baseId</span></span>|<span data-ttu-id="e69f0-138">String</span><span class="sxs-lookup"><span data-stu-id="e69f0-138">String</span></span>|<span data-ttu-id="e69f0-139">Identificador de base de modelos</span><span class="sxs-lookup"><span data-stu-id="e69f0-139">Template base identifier</span></span>|
|<span data-ttu-id="e69f0-140">versão</span><span class="sxs-lookup"><span data-stu-id="e69f0-140">version</span></span>|<span data-ttu-id="e69f0-141">Int32</span><span class="sxs-lookup"><span data-stu-id="e69f0-141">Int32</span></span>|<span data-ttu-id="e69f0-142">Versão do modelo.</span><span class="sxs-lookup"><span data-stu-id="e69f0-142">Template version.</span></span> <span data-ttu-id="e69f0-143">Valores válidos de 1 a 2147483647.</span><span class="sxs-lookup"><span data-stu-id="e69f0-143">Valid values 1 to 2147483647.</span></span> <span data-ttu-id="e69f0-144">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e69f0-144">This property is read-only.</span></span>|
|<span data-ttu-id="e69f0-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e69f0-145">displayName</span></span>|<span data-ttu-id="e69f0-146">String</span><span class="sxs-lookup"><span data-stu-id="e69f0-146">String</span></span>|<span data-ttu-id="e69f0-147">Nome de exibição do modelo</span><span class="sxs-lookup"><span data-stu-id="e69f0-147">Template display name</span></span>|
|<span data-ttu-id="e69f0-148">descrição</span><span class="sxs-lookup"><span data-stu-id="e69f0-148">description</span></span>|<span data-ttu-id="e69f0-149">String</span><span class="sxs-lookup"><span data-stu-id="e69f0-149">String</span></span>|<span data-ttu-id="e69f0-150">Descrição do modelo</span><span class="sxs-lookup"><span data-stu-id="e69f0-150">Template description</span></span>|
|<span data-ttu-id="e69f0-151">displayVersion</span><span class="sxs-lookup"><span data-stu-id="e69f0-151">displayVersion</span></span>|<span data-ttu-id="e69f0-152">String</span><span class="sxs-lookup"><span data-stu-id="e69f0-152">String</span></span>|<span data-ttu-id="e69f0-153">Descrição da versão do modelo</span><span class="sxs-lookup"><span data-stu-id="e69f0-153">Description of template version</span></span>|
|<span data-ttu-id="e69f0-154">lifecycleState</span><span class="sxs-lookup"><span data-stu-id="e69f0-154">lifecycleState</span></span>|[<span data-ttu-id="e69f0-155">deviceManagementTemplateLifecycleState</span><span class="sxs-lookup"><span data-stu-id="e69f0-155">deviceManagementTemplateLifecycleState</span></span>](../resources/intune-deviceconfigv2-devicemanagementtemplatelifecyclestate.md)|<span data-ttu-id="e69f0-156">Indique o estado atual do modelo de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="e69f0-156">Indicate current lifecycle state of template.</span></span> <span data-ttu-id="e69f0-157">Os possíveis valores são: `invalid`, `draft`, `active`, `superseded`, `deprecated`, `retired`.</span><span class="sxs-lookup"><span data-stu-id="e69f0-157">Possible values are: `invalid`, `draft`, `active`, `superseded`, `deprecated`, `retired`.</span></span>|
|<span data-ttu-id="e69f0-158">plataformas</span><span class="sxs-lookup"><span data-stu-id="e69f0-158">platforms</span></span>|[<span data-ttu-id="e69f0-159">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="e69f0-159">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="e69f0-160">Plataformas para este modelo.</span><span class="sxs-lookup"><span data-stu-id="e69f0-160">Platforms for this template.</span></span> <span data-ttu-id="e69f0-161">Os valores possíveis são: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="e69f0-161">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="e69f0-162">technologies</span><span class="sxs-lookup"><span data-stu-id="e69f0-162">technologies</span></span>|[<span data-ttu-id="e69f0-163">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="e69f0-163">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="e69f0-164">Tecnologias para este modelo.</span><span class="sxs-lookup"><span data-stu-id="e69f0-164">Technologies for this template.</span></span> <span data-ttu-id="e69f0-165">Os valores possíveis são: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span><span class="sxs-lookup"><span data-stu-id="e69f0-165">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span></span>|
|<span data-ttu-id="e69f0-166">templateFamily</span><span class="sxs-lookup"><span data-stu-id="e69f0-166">templateFamily</span></span>|[<span data-ttu-id="e69f0-167">deviceManagementConfigurationTemplateFamily</span><span class="sxs-lookup"><span data-stu-id="e69f0-167">deviceManagementConfigurationTemplateFamily</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtemplatefamily.md)|<span data-ttu-id="e69f0-168">TemplateFamily para este modelo.</span><span class="sxs-lookup"><span data-stu-id="e69f0-168">TemplateFamily for this template.</span></span> <span data-ttu-id="e69f0-169">Os valores possíveis são: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDetectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`.</span><span class="sxs-lookup"><span data-stu-id="e69f0-169">Possible values are: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDetectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`.</span></span>|
|<span data-ttu-id="e69f0-170">allowUnmanagedSettings</span><span class="sxs-lookup"><span data-stu-id="e69f0-170">allowUnmanagedSettings</span></span>|<span data-ttu-id="e69f0-171">Booleano</span><span class="sxs-lookup"><span data-stu-id="e69f0-171">Boolean</span></span>|<span data-ttu-id="e69f0-172">Permitir modelos de configuração nãomanageados</span><span class="sxs-lookup"><span data-stu-id="e69f0-172">Allow unmanaged setting templates</span></span>|
|<span data-ttu-id="e69f0-173">settingTemplateCount</span><span class="sxs-lookup"><span data-stu-id="e69f0-173">settingTemplateCount</span></span>|<span data-ttu-id="e69f0-174">Int32</span><span class="sxs-lookup"><span data-stu-id="e69f0-174">Int32</span></span>|<span data-ttu-id="e69f0-175">Número de modelos de configuração.</span><span class="sxs-lookup"><span data-stu-id="e69f0-175">Number of setting templates.</span></span> <span data-ttu-id="e69f0-176">Valores válidos de 0 a 2147483647.</span><span class="sxs-lookup"><span data-stu-id="e69f0-176">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="e69f0-177">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e69f0-177">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="e69f0-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="e69f0-178">Response</span></span>
<span data-ttu-id="e69f0-179">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e69f0-179">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e69f0-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e69f0-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="e69f0-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e69f0-181">Request</span></span>
<span data-ttu-id="e69f0-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e69f0-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}
Content-type: application/json
Content-length: 453

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplate",
  "baseId": "Base Id value",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "displayVersion": "Display Version value",
  "lifecycleState": "draft",
  "platforms": "macOS",
  "technologies": "mdm",
  "templateFamily": "endpointSecurityAntivirus",
  "allowUnmanagedSettings": true,
  "settingTemplateCount": 4
}
```

### <a name="response"></a><span data-ttu-id="e69f0-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="e69f0-183">Response</span></span>
<span data-ttu-id="e69f0-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e69f0-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 502

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplate",
  "id": "424ddb9a-db9a-424d-9adb-4d429adb4d42",
  "baseId": "Base Id value",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "displayVersion": "Display Version value",
  "lifecycleState": "draft",
  "platforms": "macOS",
  "technologies": "mdm",
  "templateFamily": "endpointSecurityAntivirus",
  "allowUnmanagedSettings": true,
  "settingTemplateCount": 4
}
```




