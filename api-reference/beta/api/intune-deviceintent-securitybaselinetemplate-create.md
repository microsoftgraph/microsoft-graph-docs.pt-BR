---
title: Criar securityBaselineTemplate
description: Crie um novo objeto securityBaselineTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c56758ab2f1cc75149fb63aa77a83a67873d0fb7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154501"
---
# <a name="create-securitybaselinetemplate"></a><span data-ttu-id="a0d7f-103">Criar securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="a0d7f-103">Create securityBaselineTemplate</span></span>

<span data-ttu-id="a0d7f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0d7f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0d7f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a0d7f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0d7f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0d7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0d7f-107">Crie um novo [objeto securityBaselineTemplate.](../resources/intune-deviceintent-securitybaselinetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="a0d7f-107">Create a new [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0d7f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0d7f-108">Prerequisites</span></span>
<span data-ttu-id="a0d7f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0d7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0d7f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0d7f-111">Permission type</span></span>|<span data-ttu-id="a0d7f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0d7f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0d7f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0d7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0d7f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0d7f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0d7f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0d7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0d7f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0d7f-116">Not supported.</span></span>|
|<span data-ttu-id="a0d7f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0d7f-117">Application</span></span>|<span data-ttu-id="a0d7f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0d7f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0d7f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0d7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="a0d7f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0d7f-120">Request headers</span></span>
|<span data-ttu-id="a0d7f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0d7f-121">Header</span></span>|<span data-ttu-id="a0d7f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a0d7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0d7f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0d7f-123">Authorization</span></span>|<span data-ttu-id="a0d7f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0d7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0d7f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0d7f-125">Accept</span></span>|<span data-ttu-id="a0d7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0d7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0d7f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0d7f-127">Request body</span></span>
<span data-ttu-id="a0d7f-128">No corpo da solicitação, fornece uma representação JSON para o objeto securityBaselineTemplate.</span><span class="sxs-lookup"><span data-stu-id="a0d7f-128">In the request body, supply a JSON representation for the securityBaselineTemplate object.</span></span>

<span data-ttu-id="a0d7f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o securityBaselineTemplate.</span><span class="sxs-lookup"><span data-stu-id="a0d7f-129">The following table shows the properties that are required when you create the securityBaselineTemplate.</span></span>

|<span data-ttu-id="a0d7f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0d7f-130">Property</span></span>|<span data-ttu-id="a0d7f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0d7f-131">Type</span></span>|<span data-ttu-id="a0d7f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0d7f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0d7f-133">id</span><span class="sxs-lookup"><span data-stu-id="a0d7f-133">id</span></span>|<span data-ttu-id="a0d7f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0d7f-134">String</span></span>|<span data-ttu-id="a0d7f-135">A ID do modelo Herdada [de deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="a0d7f-135">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="a0d7f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a0d7f-136">displayName</span></span>|<span data-ttu-id="a0d7f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0d7f-137">String</span></span>|<span data-ttu-id="a0d7f-138">O nome de exibição do modelo Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="a0d7f-138">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="a0d7f-139">descrição</span><span class="sxs-lookup"><span data-stu-id="a0d7f-139">description</span></span>|<span data-ttu-id="a0d7f-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0d7f-140">String</span></span>|<span data-ttu-id="a0d7f-141">Descrição do modelo Herdada de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="a0d7f-141">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="a0d7f-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="a0d7f-142">versionInfo</span></span>|<span data-ttu-id="a0d7f-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0d7f-143">String</span></span>|<span data-ttu-id="a0d7f-144">Informações de versão do modelo Herdadas de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="a0d7f-144">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="a0d7f-145">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="a0d7f-145">isDeprecated</span></span>|<span data-ttu-id="a0d7f-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="a0d7f-146">Boolean</span></span>|<span data-ttu-id="a0d7f-147">O modelo está preterido ou não.</span><span class="sxs-lookup"><span data-stu-id="a0d7f-147">The template is deprecated or not.</span></span> <span data-ttu-id="a0d7f-148">As intenções não podem ser criadas a partir de um modelo preterido.</span><span class="sxs-lookup"><span data-stu-id="a0d7f-148">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="a0d7f-149">Herdado [de deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="a0d7f-149">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="a0d7f-150">intentCount</span><span class="sxs-lookup"><span data-stu-id="a0d7f-150">intentCount</span></span>|<span data-ttu-id="a0d7f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="a0d7f-151">Int32</span></span>|<span data-ttu-id="a0d7f-152">Número de Intenções criadas a partir deste modelo.</span><span class="sxs-lookup"><span data-stu-id="a0d7f-152">Number of Intents created from this template.</span></span> <span data-ttu-id="a0d7f-153">Herdado [de deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="a0d7f-153">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="a0d7f-154">templateType</span><span class="sxs-lookup"><span data-stu-id="a0d7f-154">templateType</span></span>|[<span data-ttu-id="a0d7f-155">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="a0d7f-155">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="a0d7f-156">O tipo do modelo.</span><span class="sxs-lookup"><span data-stu-id="a0d7f-156">The template's type.</span></span> <span data-ttu-id="a0d7f-157">Herdado [de deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="a0d7f-157">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="a0d7f-158">Os valores possíveis são: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.</span><span class="sxs-lookup"><span data-stu-id="a0d7f-158">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.</span></span>|
|<span data-ttu-id="a0d7f-159">platformType</span><span class="sxs-lookup"><span data-stu-id="a0d7f-159">platformType</span></span>|[<span data-ttu-id="a0d7f-160">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="a0d7f-160">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="a0d7f-161">A plataforma do modelo.</span><span class="sxs-lookup"><span data-stu-id="a0d7f-161">The template's platform.</span></span> <span data-ttu-id="a0d7f-162">Herdado [de deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="a0d7f-162">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="a0d7f-163">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="a0d7f-163">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="a0d7f-164">templateSubtype</span><span class="sxs-lookup"><span data-stu-id="a0d7f-164">templateSubtype</span></span>|[<span data-ttu-id="a0d7f-165">deviceManagementTemplateSubtype</span><span class="sxs-lookup"><span data-stu-id="a0d7f-165">deviceManagementTemplateSubtype</span></span>](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|<span data-ttu-id="a0d7f-166">O subtipo do modelo.</span><span class="sxs-lookup"><span data-stu-id="a0d7f-166">The template's subtype.</span></span> <span data-ttu-id="a0d7f-167">Herdado [de deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="a0d7f-167">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="a0d7f-168">Os valores possíveis são: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.</span><span class="sxs-lookup"><span data-stu-id="a0d7f-168">Possible values are: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.</span></span>|
|<span data-ttu-id="a0d7f-169">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0d7f-169">publishedDateTime</span></span>|<span data-ttu-id="a0d7f-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0d7f-170">DateTimeOffset</span></span>|<span data-ttu-id="a0d7f-171">Quando o modelo foi publicado Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="a0d7f-171">When the template was published Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a0d7f-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0d7f-172">Response</span></span>
<span data-ttu-id="a0d7f-173">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0d7f-173">If successful, this method returns a `201 Created` response code and a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0d7f-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0d7f-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0d7f-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0d7f-175">Request</span></span>
<span data-ttu-id="a0d7f-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0d7f-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 405

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "platformType": "androidForWork",
  "templateSubtype": "firewall",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a><span data-ttu-id="a0d7f-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0d7f-177">Response</span></span>
<span data-ttu-id="a0d7f-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0d7f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 454

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "platformType": "androidForWork",
  "templateSubtype": "firewall",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```




