---
title: Atualizar deviceManagementTemplate
description: Atualize as propriedades de um objeto deviceManagementTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1134dc4a8c519d6c56ed1c2ad490a30fd72bc223
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130858"
---
# <a name="update-devicemanagementtemplate"></a><span data-ttu-id="8ede7-103">Atualizar deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="8ede7-103">Update deviceManagementTemplate</span></span>

<span data-ttu-id="8ede7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ede7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ede7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8ede7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ede7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8ede7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ede7-107">Atualize as propriedades de [um objeto deviceManagementTemplate.](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="8ede7-107">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ede7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8ede7-108">Prerequisites</span></span>
<span data-ttu-id="8ede7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ede7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ede7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ede7-111">Permission type</span></span>|<span data-ttu-id="8ede7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ede7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ede7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ede7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ede7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ede7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ede7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ede7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ede7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ede7-116">Not supported.</span></span>|
|<span data-ttu-id="8ede7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ede7-117">Application</span></span>|<span data-ttu-id="8ede7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ede7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ede7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ede7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="8ede7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ede7-120">Request headers</span></span>
|<span data-ttu-id="8ede7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8ede7-121">Header</span></span>|<span data-ttu-id="8ede7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8ede7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ede7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ede7-123">Authorization</span></span>|<span data-ttu-id="8ede7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ede7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ede7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8ede7-125">Accept</span></span>|<span data-ttu-id="8ede7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ede7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ede7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ede7-127">Request body</span></span>
<span data-ttu-id="8ede7-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementTemplate.](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="8ede7-128">In the request body, supply a JSON representation for the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

<span data-ttu-id="8ede7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="8ede7-129">The following table shows the properties that are required when you create the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>

|<span data-ttu-id="8ede7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ede7-130">Property</span></span>|<span data-ttu-id="8ede7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ede7-131">Type</span></span>|<span data-ttu-id="8ede7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ede7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ede7-133">id</span><span class="sxs-lookup"><span data-stu-id="8ede7-133">id</span></span>|<span data-ttu-id="8ede7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ede7-134">String</span></span>|<span data-ttu-id="8ede7-135">A ID do modelo</span><span class="sxs-lookup"><span data-stu-id="8ede7-135">The template ID</span></span>|
|<span data-ttu-id="8ede7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8ede7-136">displayName</span></span>|<span data-ttu-id="8ede7-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ede7-137">String</span></span>|<span data-ttu-id="8ede7-138">O nome de exibição do modelo</span><span class="sxs-lookup"><span data-stu-id="8ede7-138">The template's display name</span></span>|
|<span data-ttu-id="8ede7-139">descrição</span><span class="sxs-lookup"><span data-stu-id="8ede7-139">description</span></span>|<span data-ttu-id="8ede7-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ede7-140">String</span></span>|<span data-ttu-id="8ede7-141">A descrição do modelo</span><span class="sxs-lookup"><span data-stu-id="8ede7-141">The template's description</span></span>|
|<span data-ttu-id="8ede7-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="8ede7-142">versionInfo</span></span>|<span data-ttu-id="8ede7-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ede7-143">String</span></span>|<span data-ttu-id="8ede7-144">Informações de versão do modelo</span><span class="sxs-lookup"><span data-stu-id="8ede7-144">The template's version information</span></span>|
|<span data-ttu-id="8ede7-145">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="8ede7-145">isDeprecated</span></span>|<span data-ttu-id="8ede7-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="8ede7-146">Boolean</span></span>|<span data-ttu-id="8ede7-147">O modelo está preterido ou não.</span><span class="sxs-lookup"><span data-stu-id="8ede7-147">The template is deprecated or not.</span></span> <span data-ttu-id="8ede7-148">As intenções não podem ser criadas a partir de um modelo preterido.</span><span class="sxs-lookup"><span data-stu-id="8ede7-148">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="8ede7-149">intentCount</span><span class="sxs-lookup"><span data-stu-id="8ede7-149">intentCount</span></span>|<span data-ttu-id="8ede7-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8ede7-150">Int32</span></span>|<span data-ttu-id="8ede7-151">Número de Intenções criadas a partir deste modelo.</span><span class="sxs-lookup"><span data-stu-id="8ede7-151">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="8ede7-152">templateType</span><span class="sxs-lookup"><span data-stu-id="8ede7-152">templateType</span></span>|[<span data-ttu-id="8ede7-153">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="8ede7-153">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="8ede7-154">O tipo do modelo.</span><span class="sxs-lookup"><span data-stu-id="8ede7-154">The template's type.</span></span> <span data-ttu-id="8ede7-155">Os valores possíveis são: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.</span><span class="sxs-lookup"><span data-stu-id="8ede7-155">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.</span></span>|
|<span data-ttu-id="8ede7-156">platformType</span><span class="sxs-lookup"><span data-stu-id="8ede7-156">platformType</span></span>|[<span data-ttu-id="8ede7-157">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="8ede7-157">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="8ede7-158">A plataforma do modelo.</span><span class="sxs-lookup"><span data-stu-id="8ede7-158">The template's platform.</span></span> <span data-ttu-id="8ede7-159">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="8ede7-159">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="8ede7-160">templateSubtype</span><span class="sxs-lookup"><span data-stu-id="8ede7-160">templateSubtype</span></span>|[<span data-ttu-id="8ede7-161">deviceManagementTemplateSubtype</span><span class="sxs-lookup"><span data-stu-id="8ede7-161">deviceManagementTemplateSubtype</span></span>](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|<span data-ttu-id="8ede7-162">O subtipo do modelo.</span><span class="sxs-lookup"><span data-stu-id="8ede7-162">The template's subtype.</span></span> <span data-ttu-id="8ede7-163">Os valores possíveis são: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.</span><span class="sxs-lookup"><span data-stu-id="8ede7-163">Possible values are: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.</span></span>|
|<span data-ttu-id="8ede7-164">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ede7-164">publishedDateTime</span></span>|<span data-ttu-id="8ede7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ede7-165">DateTimeOffset</span></span>|<span data-ttu-id="8ede7-166">Quando o modelo foi publicado</span><span class="sxs-lookup"><span data-stu-id="8ede7-166">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="8ede7-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ede7-167">Response</span></span>
<span data-ttu-id="8ede7-168">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ede7-168">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ede7-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ede7-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ede7-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ede7-170">Request</span></span>
<span data-ttu-id="8ede7-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ede7-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8ede7-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ede7-172">Response</span></span>
<span data-ttu-id="8ede7-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ede7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




