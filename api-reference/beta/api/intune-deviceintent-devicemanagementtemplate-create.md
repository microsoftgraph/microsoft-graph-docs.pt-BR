---
title: Criar deviceManagementTemplate
description: Criar um novo objeto deviceManagementTemplate.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fc741640f5f8762985ccbe7ad2d261524f9ee73c
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122753"
---
# <a name="create-devicemanagementtemplate"></a><span data-ttu-id="d3ed6-103">Criar deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="d3ed6-103">Create deviceManagementTemplate</span></span>

<span data-ttu-id="d3ed6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3ed6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3ed6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3ed6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3ed6-107">Criar um novo objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="d3ed6-107">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3ed6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3ed6-108">Prerequisites</span></span>
<span data-ttu-id="d3ed6-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d3ed6-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3ed6-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3ed6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3ed6-111">Permission type</span></span>|<span data-ttu-id="d3ed6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3ed6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3ed6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3ed6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3ed6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3ed6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d3ed6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3ed6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3ed6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-116">Not supported.</span></span>|
|<span data-ttu-id="d3ed6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3ed6-117">Application</span></span>|<span data-ttu-id="d3ed6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3ed6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3ed6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3ed6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="d3ed6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3ed6-120">Request headers</span></span>
|<span data-ttu-id="d3ed6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3ed6-121">Header</span></span>|<span data-ttu-id="d3ed6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d3ed6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3ed6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3ed6-123">Authorization</span></span>|<span data-ttu-id="d3ed6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3ed6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d3ed6-125">Accept</span></span>|<span data-ttu-id="d3ed6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3ed6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3ed6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3ed6-127">Request body</span></span>
<span data-ttu-id="d3ed6-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementTemplate.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-128">In the request body, supply a JSON representation for the deviceManagementTemplate object.</span></span>

<span data-ttu-id="d3ed6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementTemplate.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-129">The following table shows the properties that are required when you create the deviceManagementTemplate.</span></span>

|<span data-ttu-id="d3ed6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3ed6-130">Property</span></span>|<span data-ttu-id="d3ed6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3ed6-131">Type</span></span>|<span data-ttu-id="d3ed6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3ed6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3ed6-133">id</span><span class="sxs-lookup"><span data-stu-id="d3ed6-133">id</span></span>|<span data-ttu-id="d3ed6-134">String</span><span class="sxs-lookup"><span data-stu-id="d3ed6-134">String</span></span>|<span data-ttu-id="d3ed6-135">A ID do modelo</span><span class="sxs-lookup"><span data-stu-id="d3ed6-135">The template ID</span></span>|
|<span data-ttu-id="d3ed6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d3ed6-136">displayName</span></span>|<span data-ttu-id="d3ed6-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3ed6-137">String</span></span>|<span data-ttu-id="d3ed6-138">O nome de exibição do modelo</span><span class="sxs-lookup"><span data-stu-id="d3ed6-138">The template's display name</span></span>|
|<span data-ttu-id="d3ed6-139">descrição</span><span class="sxs-lookup"><span data-stu-id="d3ed6-139">description</span></span>|<span data-ttu-id="d3ed6-140">String</span><span class="sxs-lookup"><span data-stu-id="d3ed6-140">String</span></span>|<span data-ttu-id="d3ed6-141">A descrição do modelo</span><span class="sxs-lookup"><span data-stu-id="d3ed6-141">The template's description</span></span>|
|<span data-ttu-id="d3ed6-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="d3ed6-142">versionInfo</span></span>|<span data-ttu-id="d3ed6-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3ed6-143">String</span></span>|<span data-ttu-id="d3ed6-144">As informações de versão do modelo</span><span class="sxs-lookup"><span data-stu-id="d3ed6-144">The template's version information</span></span>|
|<span data-ttu-id="d3ed6-145">preterido</span><span class="sxs-lookup"><span data-stu-id="d3ed6-145">isDeprecated</span></span>|<span data-ttu-id="d3ed6-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="d3ed6-146">Boolean</span></span>|<span data-ttu-id="d3ed6-147">O modelo é preterido ou não.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-147">The template is deprecated or not.</span></span> <span data-ttu-id="d3ed6-148">Os propósitos não podem ser criados a partir de um modelo preterido.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-148">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="d3ed6-149">intentCount</span><span class="sxs-lookup"><span data-stu-id="d3ed6-149">intentCount</span></span>|<span data-ttu-id="d3ed6-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d3ed6-150">Int32</span></span>|<span data-ttu-id="d3ed6-151">Número de tentativas criadas a partir deste modelo.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-151">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="d3ed6-152">templateType</span><span class="sxs-lookup"><span data-stu-id="d3ed6-152">templateType</span></span>|[<span data-ttu-id="d3ed6-153">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="d3ed6-153">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="d3ed6-154">O tipo do modelo.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-154">The template's type.</span></span> <span data-ttu-id="d3ed6-155">Os valores possíveis são: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-155">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`.</span></span>|
|<span data-ttu-id="d3ed6-156">platformType</span><span class="sxs-lookup"><span data-stu-id="d3ed6-156">platformType</span></span>|[<span data-ttu-id="d3ed6-157">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="d3ed6-157">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="d3ed6-158">A plataforma do modelo.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-158">The template's platform.</span></span> <span data-ttu-id="d3ed6-159">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-159">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="d3ed6-160">templateSubtype</span><span class="sxs-lookup"><span data-stu-id="d3ed6-160">templateSubtype</span></span>|[<span data-ttu-id="d3ed6-161">deviceManagementTemplateSubtype</span><span class="sxs-lookup"><span data-stu-id="d3ed6-161">deviceManagementTemplateSubtype</span></span>](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|<span data-ttu-id="d3ed6-162">O subtipo do modelo.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-162">The template's subtype.</span></span> <span data-ttu-id="d3ed6-163">Os valores possíveis são: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-163">Possible values are: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`.</span></span>|
|<span data-ttu-id="d3ed6-164">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3ed6-164">publishedDateTime</span></span>|<span data-ttu-id="d3ed6-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3ed6-165">DateTimeOffset</span></span>|<span data-ttu-id="d3ed6-166">Quando o modelo foi publicado</span><span class="sxs-lookup"><span data-stu-id="d3ed6-166">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="d3ed6-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3ed6-167">Response</span></span>
<span data-ttu-id="d3ed6-168">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-168">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3ed6-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3ed6-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3ed6-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3ed6-170">Request</span></span>
<span data-ttu-id="d3ed6-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 405

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
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

### <a name="response"></a><span data-ttu-id="d3ed6-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3ed6-172">Response</span></span>
<span data-ttu-id="d3ed6-173">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-173">Here is an example of the response.</span></span> <span data-ttu-id="d3ed6-174">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-174">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d3ed6-175">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="d3ed6-175">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 454

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
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



