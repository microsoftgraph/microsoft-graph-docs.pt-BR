---
title: Criar securityBaselineTemplate
description: Criar um novo objeto securityBaselineTemplate.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4e1156255a9c936a7440091040443ace8d7bfd0b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43427238"
---
# <a name="create-securitybaselinetemplate"></a><span data-ttu-id="e1815-103">Criar securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="e1815-103">Create securityBaselineTemplate</span></span>

<span data-ttu-id="e1815-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1815-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1815-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e1815-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1815-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1815-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1815-107">Criar um novo objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="e1815-107">Create a new [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1815-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1815-108">Prerequisites</span></span>
<span data-ttu-id="e1815-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1815-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1815-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1815-111">Permission type</span></span>|<span data-ttu-id="e1815-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1815-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1815-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1815-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1815-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1815-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e1815-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1815-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1815-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1815-116">Not supported.</span></span>|
|<span data-ttu-id="e1815-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1815-117">Application</span></span>|<span data-ttu-id="e1815-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1815-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1815-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1815-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="e1815-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1815-120">Request headers</span></span>
|<span data-ttu-id="e1815-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1815-121">Header</span></span>|<span data-ttu-id="e1815-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e1815-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1815-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1815-123">Authorization</span></span>|<span data-ttu-id="e1815-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1815-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1815-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1815-125">Accept</span></span>|<span data-ttu-id="e1815-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1815-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1815-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1815-127">Request body</span></span>
<span data-ttu-id="e1815-128">No corpo da solicitação, forneça uma representação JSON do objeto securityBaselineTemplate.</span><span class="sxs-lookup"><span data-stu-id="e1815-128">In the request body, supply a JSON representation for the securityBaselineTemplate object.</span></span>

<span data-ttu-id="e1815-129">A tabela a seguir mostra as propriedades que são necessárias ao criar securityBaselineTemplate.</span><span class="sxs-lookup"><span data-stu-id="e1815-129">The following table shows the properties that are required when you create the securityBaselineTemplate.</span></span>

|<span data-ttu-id="e1815-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1815-130">Property</span></span>|<span data-ttu-id="e1815-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1815-131">Type</span></span>|<span data-ttu-id="e1815-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1815-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1815-133">id</span><span class="sxs-lookup"><span data-stu-id="e1815-133">id</span></span>|<span data-ttu-id="e1815-134">String</span><span class="sxs-lookup"><span data-stu-id="e1815-134">String</span></span>|<span data-ttu-id="e1815-135">A ID do modelo herdada de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e1815-135">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="e1815-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e1815-136">displayName</span></span>|<span data-ttu-id="e1815-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1815-137">String</span></span>|<span data-ttu-id="e1815-138">O nome de exibição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e1815-138">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="e1815-139">description</span><span class="sxs-lookup"><span data-stu-id="e1815-139">description</span></span>|<span data-ttu-id="e1815-140">String</span><span class="sxs-lookup"><span data-stu-id="e1815-140">String</span></span>|<span data-ttu-id="e1815-141">A descrição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e1815-141">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="e1815-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="e1815-142">versionInfo</span></span>|<span data-ttu-id="e1815-143">String</span><span class="sxs-lookup"><span data-stu-id="e1815-143">String</span></span>|<span data-ttu-id="e1815-144">As informações de versão do modelo herdadas de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e1815-144">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="e1815-145">preterido</span><span class="sxs-lookup"><span data-stu-id="e1815-145">isDeprecated</span></span>|<span data-ttu-id="e1815-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1815-146">Boolean</span></span>|<span data-ttu-id="e1815-147">O modelo é preterido ou não.</span><span class="sxs-lookup"><span data-stu-id="e1815-147">The template is deprecated or not.</span></span> <span data-ttu-id="e1815-148">Os propósitos não podem ser criados a partir de um modelo preterido.</span><span class="sxs-lookup"><span data-stu-id="e1815-148">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="e1815-149">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e1815-149">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="e1815-150">intentCount</span><span class="sxs-lookup"><span data-stu-id="e1815-150">intentCount</span></span>|<span data-ttu-id="e1815-151">Int32</span><span class="sxs-lookup"><span data-stu-id="e1815-151">Int32</span></span>|<span data-ttu-id="e1815-152">Número de tentativas criadas a partir deste modelo.</span><span class="sxs-lookup"><span data-stu-id="e1815-152">Number of Intents created from this template.</span></span> <span data-ttu-id="e1815-153">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e1815-153">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="e1815-154">templateType</span><span class="sxs-lookup"><span data-stu-id="e1815-154">templateType</span></span>|[<span data-ttu-id="e1815-155">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="e1815-155">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="e1815-156">O tipo do modelo.</span><span class="sxs-lookup"><span data-stu-id="e1815-156">The template's type.</span></span> <span data-ttu-id="e1815-157">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="e1815-157">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="e1815-158">Os valores possíveis são: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`.</span><span class="sxs-lookup"><span data-stu-id="e1815-158">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`.</span></span>|
|<span data-ttu-id="e1815-159">platformType</span><span class="sxs-lookup"><span data-stu-id="e1815-159">platformType</span></span>|[<span data-ttu-id="e1815-160">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="e1815-160">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="e1815-161">A plataforma do modelo.</span><span class="sxs-lookup"><span data-stu-id="e1815-161">The template's platform.</span></span> <span data-ttu-id="e1815-162">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="e1815-162">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="e1815-163">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="e1815-163">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="e1815-164">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1815-164">publishedDateTime</span></span>|<span data-ttu-id="e1815-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1815-165">DateTimeOffset</span></span>|<span data-ttu-id="e1815-166">Quando o modelo foi publicado herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e1815-166">When the template was published Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e1815-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1815-167">Response</span></span>
<span data-ttu-id="e1815-168">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1815-168">If successful, this method returns a `201 Created` response code and a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1815-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1815-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1815-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1815-170">Request</span></span>
<span data-ttu-id="e1815-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1815-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e1815-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1815-172">Response</span></span>
<span data-ttu-id="e1815-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1815-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



