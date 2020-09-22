---
title: Atualizar deviceManagementTemplate
description: Atualiza as propriedades de um objeto deviceManagementTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b960e6ae36f9f55f60141ded1841c3958a23b1c6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059002"
---
# <a name="update-devicemanagementtemplate"></a><span data-ttu-id="3c71b-103">Atualizar deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="3c71b-103">Update deviceManagementTemplate</span></span>

<span data-ttu-id="3c71b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c71b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c71b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3c71b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c71b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c71b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c71b-107">Atualiza as propriedades de um objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="3c71b-107">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c71b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3c71b-108">Prerequisites</span></span>
<span data-ttu-id="3c71b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c71b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c71b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c71b-111">Permission type</span></span>|<span data-ttu-id="3c71b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3c71b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c71b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c71b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c71b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c71b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3c71b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c71b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c71b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c71b-116">Not supported.</span></span>|
|<span data-ttu-id="3c71b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c71b-117">Application</span></span>|<span data-ttu-id="3c71b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c71b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c71b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c71b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="3c71b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c71b-120">Request headers</span></span>
|<span data-ttu-id="3c71b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c71b-121">Header</span></span>|<span data-ttu-id="3c71b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3c71b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c71b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c71b-123">Authorization</span></span>|<span data-ttu-id="3c71b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c71b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c71b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3c71b-125">Accept</span></span>|<span data-ttu-id="3c71b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c71b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c71b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c71b-127">Request body</span></span>
<span data-ttu-id="3c71b-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="3c71b-128">In the request body, supply a JSON representation for the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

<span data-ttu-id="3c71b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="3c71b-129">The following table shows the properties that are required when you create the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>

|<span data-ttu-id="3c71b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c71b-130">Property</span></span>|<span data-ttu-id="3c71b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c71b-131">Type</span></span>|<span data-ttu-id="3c71b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c71b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c71b-133">id</span><span class="sxs-lookup"><span data-stu-id="3c71b-133">id</span></span>|<span data-ttu-id="3c71b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c71b-134">String</span></span>|<span data-ttu-id="3c71b-135">A ID do modelo</span><span class="sxs-lookup"><span data-stu-id="3c71b-135">The template ID</span></span>|
|<span data-ttu-id="3c71b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3c71b-136">displayName</span></span>|<span data-ttu-id="3c71b-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c71b-137">String</span></span>|<span data-ttu-id="3c71b-138">O nome de exibição do modelo</span><span class="sxs-lookup"><span data-stu-id="3c71b-138">The template's display name</span></span>|
|<span data-ttu-id="3c71b-139">description</span><span class="sxs-lookup"><span data-stu-id="3c71b-139">description</span></span>|<span data-ttu-id="3c71b-140">String</span><span class="sxs-lookup"><span data-stu-id="3c71b-140">String</span></span>|<span data-ttu-id="3c71b-141">A descrição do modelo</span><span class="sxs-lookup"><span data-stu-id="3c71b-141">The template's description</span></span>|
|<span data-ttu-id="3c71b-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="3c71b-142">versionInfo</span></span>|<span data-ttu-id="3c71b-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c71b-143">String</span></span>|<span data-ttu-id="3c71b-144">As informações de versão do modelo</span><span class="sxs-lookup"><span data-stu-id="3c71b-144">The template's version information</span></span>|
|<span data-ttu-id="3c71b-145">preterido</span><span class="sxs-lookup"><span data-stu-id="3c71b-145">isDeprecated</span></span>|<span data-ttu-id="3c71b-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="3c71b-146">Boolean</span></span>|<span data-ttu-id="3c71b-147">O modelo é preterido ou não.</span><span class="sxs-lookup"><span data-stu-id="3c71b-147">The template is deprecated or not.</span></span> <span data-ttu-id="3c71b-148">Os propósitos não podem ser criados a partir de um modelo preterido.</span><span class="sxs-lookup"><span data-stu-id="3c71b-148">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="3c71b-149">intentCount</span><span class="sxs-lookup"><span data-stu-id="3c71b-149">intentCount</span></span>|<span data-ttu-id="3c71b-150">Int32</span><span class="sxs-lookup"><span data-stu-id="3c71b-150">Int32</span></span>|<span data-ttu-id="3c71b-151">Número de tentativas criadas a partir deste modelo.</span><span class="sxs-lookup"><span data-stu-id="3c71b-151">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="3c71b-152">templateType</span><span class="sxs-lookup"><span data-stu-id="3c71b-152">templateType</span></span>|[<span data-ttu-id="3c71b-153">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="3c71b-153">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="3c71b-154">O tipo do modelo.</span><span class="sxs-lookup"><span data-stu-id="3c71b-154">The template's type.</span></span> <span data-ttu-id="3c71b-155">Os valores possíveis são: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`.</span><span class="sxs-lookup"><span data-stu-id="3c71b-155">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`.</span></span>|
|<span data-ttu-id="3c71b-156">platformType</span><span class="sxs-lookup"><span data-stu-id="3c71b-156">platformType</span></span>|[<span data-ttu-id="3c71b-157">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="3c71b-157">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="3c71b-158">A plataforma do modelo.</span><span class="sxs-lookup"><span data-stu-id="3c71b-158">The template's platform.</span></span> <span data-ttu-id="3c71b-159">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="3c71b-159">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="3c71b-160">templateSubtype</span><span class="sxs-lookup"><span data-stu-id="3c71b-160">templateSubtype</span></span>|[<span data-ttu-id="3c71b-161">deviceManagementTemplateSubtype</span><span class="sxs-lookup"><span data-stu-id="3c71b-161">deviceManagementTemplateSubtype</span></span>](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|<span data-ttu-id="3c71b-162">O subtipo do modelo.</span><span class="sxs-lookup"><span data-stu-id="3c71b-162">The template's subtype.</span></span> <span data-ttu-id="3c71b-163">Os valores possíveis são: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`.</span><span class="sxs-lookup"><span data-stu-id="3c71b-163">Possible values are: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`.</span></span>|
|<span data-ttu-id="3c71b-164">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c71b-164">publishedDateTime</span></span>|<span data-ttu-id="3c71b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c71b-165">DateTimeOffset</span></span>|<span data-ttu-id="3c71b-166">Quando o modelo foi publicado</span><span class="sxs-lookup"><span data-stu-id="3c71b-166">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="3c71b-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c71b-167">Response</span></span>
<span data-ttu-id="3c71b-168">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c71b-168">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c71b-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c71b-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c71b-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c71b-170">Request</span></span>
<span data-ttu-id="3c71b-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c71b-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
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

### <a name="response"></a><span data-ttu-id="3c71b-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c71b-172">Response</span></span>
<span data-ttu-id="3c71b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c71b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






