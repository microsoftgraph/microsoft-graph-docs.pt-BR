---
title: Criar securityBaselineTemplate
description: Criar um novo objeto securityBaselineTemplate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 99fa0a20027d84829bae5e7e29eedfc6f16b080c
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41635569"
---
# <a name="create-securitybaselinetemplate"></a><span data-ttu-id="17b3e-103">Criar securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="17b3e-103">Create securityBaselineTemplate</span></span>

> <span data-ttu-id="17b3e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="17b3e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17b3e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="17b3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17b3e-106">Criar um novo objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="17b3e-106">Create a new [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17b3e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="17b3e-107">Prerequisites</span></span>
<span data-ttu-id="17b3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17b3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17b3e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17b3e-110">Permission type</span></span>|<span data-ttu-id="17b3e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="17b3e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17b3e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17b3e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17b3e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17b3e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17b3e-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17b3e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17b3e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17b3e-115">Not supported.</span></span>|
|<span data-ttu-id="17b3e-116">Application</span><span class="sxs-lookup"><span data-stu-id="17b3e-116">Application</span></span>|<span data-ttu-id="17b3e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17b3e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17b3e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17b3e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="17b3e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17b3e-119">Request headers</span></span>
|<span data-ttu-id="17b3e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17b3e-120">Header</span></span>|<span data-ttu-id="17b3e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="17b3e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17b3e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="17b3e-122">Authorization</span></span>|<span data-ttu-id="17b3e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17b3e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17b3e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="17b3e-124">Accept</span></span>|<span data-ttu-id="17b3e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="17b3e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17b3e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17b3e-126">Request body</span></span>
<span data-ttu-id="17b3e-127">No corpo da solicitação, forneça uma representação JSON do objeto securityBaselineTemplate.</span><span class="sxs-lookup"><span data-stu-id="17b3e-127">In the request body, supply a JSON representation for the securityBaselineTemplate object.</span></span>

<span data-ttu-id="17b3e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar securityBaselineTemplate.</span><span class="sxs-lookup"><span data-stu-id="17b3e-128">The following table shows the properties that are required when you create the securityBaselineTemplate.</span></span>

|<span data-ttu-id="17b3e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17b3e-129">Property</span></span>|<span data-ttu-id="17b3e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="17b3e-130">Type</span></span>|<span data-ttu-id="17b3e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="17b3e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17b3e-132">id</span><span class="sxs-lookup"><span data-stu-id="17b3e-132">id</span></span>|<span data-ttu-id="17b3e-133">String</span><span class="sxs-lookup"><span data-stu-id="17b3e-133">String</span></span>|<span data-ttu-id="17b3e-134">A ID do modelo herdada de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="17b3e-134">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="17b3e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="17b3e-135">displayName</span></span>|<span data-ttu-id="17b3e-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17b3e-136">String</span></span>|<span data-ttu-id="17b3e-137">O nome de exibição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="17b3e-137">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="17b3e-138">description</span><span class="sxs-lookup"><span data-stu-id="17b3e-138">description</span></span>|<span data-ttu-id="17b3e-139">String</span><span class="sxs-lookup"><span data-stu-id="17b3e-139">String</span></span>|<span data-ttu-id="17b3e-140">A descrição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="17b3e-140">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="17b3e-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="17b3e-141">versionInfo</span></span>|<span data-ttu-id="17b3e-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17b3e-142">String</span></span>|<span data-ttu-id="17b3e-143">As informações de versão do modelo herdadas de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="17b3e-143">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="17b3e-144">preterido</span><span class="sxs-lookup"><span data-stu-id="17b3e-144">isDeprecated</span></span>|<span data-ttu-id="17b3e-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="17b3e-145">Boolean</span></span>|<span data-ttu-id="17b3e-146">O modelo é preterido ou não.</span><span class="sxs-lookup"><span data-stu-id="17b3e-146">The template is deprecated or not.</span></span> <span data-ttu-id="17b3e-147">Os propósitos não podem ser criados a partir de um modelo preterido.</span><span class="sxs-lookup"><span data-stu-id="17b3e-147">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="17b3e-148">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="17b3e-148">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="17b3e-149">intentCount</span><span class="sxs-lookup"><span data-stu-id="17b3e-149">intentCount</span></span>|<span data-ttu-id="17b3e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="17b3e-150">Int32</span></span>|<span data-ttu-id="17b3e-151">Número de tentativas criadas a partir deste modelo.</span><span class="sxs-lookup"><span data-stu-id="17b3e-151">Number of Intents created from this template.</span></span> <span data-ttu-id="17b3e-152">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="17b3e-152">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="17b3e-153">templateType</span><span class="sxs-lookup"><span data-stu-id="17b3e-153">templateType</span></span>|[<span data-ttu-id="17b3e-154">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="17b3e-154">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="17b3e-155">O tipo do modelo.</span><span class="sxs-lookup"><span data-stu-id="17b3e-155">The template's type.</span></span> <span data-ttu-id="17b3e-156">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="17b3e-156">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="17b3e-157">Os valores possíveis são: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`.</span><span class="sxs-lookup"><span data-stu-id="17b3e-157">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`.</span></span>|
|<span data-ttu-id="17b3e-158">platformType</span><span class="sxs-lookup"><span data-stu-id="17b3e-158">platformType</span></span>|[<span data-ttu-id="17b3e-159">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="17b3e-159">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="17b3e-160">A plataforma do modelo.</span><span class="sxs-lookup"><span data-stu-id="17b3e-160">The template's platform.</span></span> <span data-ttu-id="17b3e-161">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="17b3e-161">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="17b3e-162">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="17b3e-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="17b3e-163">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="17b3e-163">publishedDateTime</span></span>|<span data-ttu-id="17b3e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17b3e-164">DateTimeOffset</span></span>|<span data-ttu-id="17b3e-165">Quando o modelo foi publicado herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="17b3e-165">When the template was published Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="17b3e-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="17b3e-166">Response</span></span>
<span data-ttu-id="17b3e-167">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17b3e-167">If successful, this method returns a `201 Created` response code and a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17b3e-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17b3e-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="17b3e-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17b3e-169">Request</span></span>
<span data-ttu-id="17b3e-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17b3e-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "platformType": "androidForWork",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a><span data-ttu-id="17b3e-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="17b3e-171">Response</span></span>
<span data-ttu-id="17b3e-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17b3e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 420

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
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```





