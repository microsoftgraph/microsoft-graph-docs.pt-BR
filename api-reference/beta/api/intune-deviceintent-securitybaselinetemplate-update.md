---
title: Atualizar securityBaselineTemplate
description: Atualiza as propriedades de um objeto securityBaselineTemplate.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 18a2281455f0611f745abe35c2ce1e6e5d6b61a6
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122725"
---
# <a name="update-securitybaselinetemplate"></a><span data-ttu-id="14531-103">Atualizar securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="14531-103">Update securityBaselineTemplate</span></span>

<span data-ttu-id="14531-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14531-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14531-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="14531-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14531-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14531-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14531-107">Atualiza as propriedades de um objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="14531-107">Update the properties of a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14531-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="14531-108">Prerequisites</span></span>
<span data-ttu-id="14531-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14531-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14531-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14531-111">Permission type</span></span>|<span data-ttu-id="14531-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="14531-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14531-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14531-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14531-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14531-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14531-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14531-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14531-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14531-116">Not supported.</span></span>|
|<span data-ttu-id="14531-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14531-117">Application</span></span>|<span data-ttu-id="14531-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14531-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14531-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14531-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="14531-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14531-120">Request headers</span></span>
|<span data-ttu-id="14531-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14531-121">Header</span></span>|<span data-ttu-id="14531-122">Valor</span><span class="sxs-lookup"><span data-stu-id="14531-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14531-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="14531-123">Authorization</span></span>|<span data-ttu-id="14531-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14531-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14531-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="14531-125">Accept</span></span>|<span data-ttu-id="14531-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14531-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14531-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14531-127">Request body</span></span>
<span data-ttu-id="14531-128">No corpo da solicitação, forneça uma representação JSON do objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="14531-128">In the request body, supply a JSON representation for the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

<span data-ttu-id="14531-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="14531-129">The following table shows the properties that are required when you create the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span></span>

|<span data-ttu-id="14531-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14531-130">Property</span></span>|<span data-ttu-id="14531-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="14531-131">Type</span></span>|<span data-ttu-id="14531-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="14531-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14531-133">id</span><span class="sxs-lookup"><span data-stu-id="14531-133">id</span></span>|<span data-ttu-id="14531-134">String</span><span class="sxs-lookup"><span data-stu-id="14531-134">String</span></span>|<span data-ttu-id="14531-135">A ID do modelo herdada de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="14531-135">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="14531-136">displayName</span><span class="sxs-lookup"><span data-stu-id="14531-136">displayName</span></span>|<span data-ttu-id="14531-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14531-137">String</span></span>|<span data-ttu-id="14531-138">O nome de exibição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="14531-138">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="14531-139">descrição</span><span class="sxs-lookup"><span data-stu-id="14531-139">description</span></span>|<span data-ttu-id="14531-140">String</span><span class="sxs-lookup"><span data-stu-id="14531-140">String</span></span>|<span data-ttu-id="14531-141">A descrição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="14531-141">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="14531-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="14531-142">versionInfo</span></span>|<span data-ttu-id="14531-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14531-143">String</span></span>|<span data-ttu-id="14531-144">As informações de versão do modelo herdadas de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="14531-144">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="14531-145">preterido</span><span class="sxs-lookup"><span data-stu-id="14531-145">isDeprecated</span></span>|<span data-ttu-id="14531-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="14531-146">Boolean</span></span>|<span data-ttu-id="14531-147">O modelo é preterido ou não.</span><span class="sxs-lookup"><span data-stu-id="14531-147">The template is deprecated or not.</span></span> <span data-ttu-id="14531-148">Os propósitos não podem ser criados a partir de um modelo preterido.</span><span class="sxs-lookup"><span data-stu-id="14531-148">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="14531-149">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="14531-149">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="14531-150">intentCount</span><span class="sxs-lookup"><span data-stu-id="14531-150">intentCount</span></span>|<span data-ttu-id="14531-151">Int32</span><span class="sxs-lookup"><span data-stu-id="14531-151">Int32</span></span>|<span data-ttu-id="14531-152">Número de tentativas criadas a partir deste modelo.</span><span class="sxs-lookup"><span data-stu-id="14531-152">Number of Intents created from this template.</span></span> <span data-ttu-id="14531-153">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="14531-153">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="14531-154">templateType</span><span class="sxs-lookup"><span data-stu-id="14531-154">templateType</span></span>|[<span data-ttu-id="14531-155">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="14531-155">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="14531-156">O tipo do modelo.</span><span class="sxs-lookup"><span data-stu-id="14531-156">The template's type.</span></span> <span data-ttu-id="14531-157">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="14531-157">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="14531-158">Os valores possíveis são: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`.</span><span class="sxs-lookup"><span data-stu-id="14531-158">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`.</span></span>|
|<span data-ttu-id="14531-159">platformType</span><span class="sxs-lookup"><span data-stu-id="14531-159">platformType</span></span>|[<span data-ttu-id="14531-160">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="14531-160">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="14531-161">A plataforma do modelo.</span><span class="sxs-lookup"><span data-stu-id="14531-161">The template's platform.</span></span> <span data-ttu-id="14531-162">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="14531-162">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="14531-163">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="14531-163">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="14531-164">templateSubtype</span><span class="sxs-lookup"><span data-stu-id="14531-164">templateSubtype</span></span>|[<span data-ttu-id="14531-165">deviceManagementTemplateSubtype</span><span class="sxs-lookup"><span data-stu-id="14531-165">deviceManagementTemplateSubtype</span></span>](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|<span data-ttu-id="14531-166">O subtipo do modelo.</span><span class="sxs-lookup"><span data-stu-id="14531-166">The template's subtype.</span></span> <span data-ttu-id="14531-167">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="14531-167">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="14531-168">Os valores possíveis são: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`.</span><span class="sxs-lookup"><span data-stu-id="14531-168">Possible values are: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`.</span></span>|
|<span data-ttu-id="14531-169">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="14531-169">publishedDateTime</span></span>|<span data-ttu-id="14531-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14531-170">DateTimeOffset</span></span>|<span data-ttu-id="14531-171">Quando o modelo foi publicado herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="14531-171">When the template was published Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="14531-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="14531-172">Response</span></span>
<span data-ttu-id="14531-173">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14531-173">If successful, this method returns a `200 OK` response code and an updated [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14531-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14531-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="14531-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14531-175">Request</span></span>
<span data-ttu-id="14531-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14531-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
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

### <a name="response"></a><span data-ttu-id="14531-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="14531-177">Response</span></span>
<span data-ttu-id="14531-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14531-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



