---
title: Criar deviceManagementTemplate
description: Criar um novo objeto deviceManagementTemplate.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 01f3c719e0f5ad2b77c48f223dd198aa7b92e96b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43381435"
---
# <a name="create-devicemanagementtemplate"></a><span data-ttu-id="75b7d-103">Criar deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="75b7d-103">Create deviceManagementTemplate</span></span>

<span data-ttu-id="75b7d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75b7d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75b7d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="75b7d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75b7d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75b7d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75b7d-107">Criar um novo objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="75b7d-107">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75b7d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="75b7d-108">Prerequisites</span></span>
<span data-ttu-id="75b7d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75b7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75b7d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75b7d-111">Permission type</span></span>|<span data-ttu-id="75b7d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="75b7d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75b7d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75b7d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75b7d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75b7d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75b7d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75b7d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75b7d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75b7d-116">Not supported.</span></span>|
|<span data-ttu-id="75b7d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75b7d-117">Application</span></span>|<span data-ttu-id="75b7d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75b7d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75b7d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75b7d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="75b7d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75b7d-120">Request headers</span></span>
|<span data-ttu-id="75b7d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="75b7d-121">Header</span></span>|<span data-ttu-id="75b7d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="75b7d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75b7d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="75b7d-123">Authorization</span></span>|<span data-ttu-id="75b7d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75b7d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75b7d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="75b7d-125">Accept</span></span>|<span data-ttu-id="75b7d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75b7d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75b7d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75b7d-127">Request body</span></span>
<span data-ttu-id="75b7d-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementTemplate.</span><span class="sxs-lookup"><span data-stu-id="75b7d-128">In the request body, supply a JSON representation for the deviceManagementTemplate object.</span></span>

<span data-ttu-id="75b7d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementTemplate.</span><span class="sxs-lookup"><span data-stu-id="75b7d-129">The following table shows the properties that are required when you create the deviceManagementTemplate.</span></span>

|<span data-ttu-id="75b7d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75b7d-130">Property</span></span>|<span data-ttu-id="75b7d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="75b7d-131">Type</span></span>|<span data-ttu-id="75b7d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="75b7d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75b7d-133">id</span><span class="sxs-lookup"><span data-stu-id="75b7d-133">id</span></span>|<span data-ttu-id="75b7d-134">String</span><span class="sxs-lookup"><span data-stu-id="75b7d-134">String</span></span>|<span data-ttu-id="75b7d-135">A ID do modelo</span><span class="sxs-lookup"><span data-stu-id="75b7d-135">The template ID</span></span>|
|<span data-ttu-id="75b7d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="75b7d-136">displayName</span></span>|<span data-ttu-id="75b7d-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75b7d-137">String</span></span>|<span data-ttu-id="75b7d-138">O nome de exibição do modelo</span><span class="sxs-lookup"><span data-stu-id="75b7d-138">The template's display name</span></span>|
|<span data-ttu-id="75b7d-139">description</span><span class="sxs-lookup"><span data-stu-id="75b7d-139">description</span></span>|<span data-ttu-id="75b7d-140">String</span><span class="sxs-lookup"><span data-stu-id="75b7d-140">String</span></span>|<span data-ttu-id="75b7d-141">A descrição do modelo</span><span class="sxs-lookup"><span data-stu-id="75b7d-141">The template's description</span></span>|
|<span data-ttu-id="75b7d-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="75b7d-142">versionInfo</span></span>|<span data-ttu-id="75b7d-143">String</span><span class="sxs-lookup"><span data-stu-id="75b7d-143">String</span></span>|<span data-ttu-id="75b7d-144">As informações de versão do modelo</span><span class="sxs-lookup"><span data-stu-id="75b7d-144">The template's version information</span></span>|
|<span data-ttu-id="75b7d-145">preterido</span><span class="sxs-lookup"><span data-stu-id="75b7d-145">isDeprecated</span></span>|<span data-ttu-id="75b7d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="75b7d-146">Boolean</span></span>|<span data-ttu-id="75b7d-147">O modelo é preterido ou não.</span><span class="sxs-lookup"><span data-stu-id="75b7d-147">The template is deprecated or not.</span></span> <span data-ttu-id="75b7d-148">Os propósitos não podem ser criados a partir de um modelo preterido.</span><span class="sxs-lookup"><span data-stu-id="75b7d-148">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="75b7d-149">intentCount</span><span class="sxs-lookup"><span data-stu-id="75b7d-149">intentCount</span></span>|<span data-ttu-id="75b7d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="75b7d-150">Int32</span></span>|<span data-ttu-id="75b7d-151">Número de tentativas criadas a partir deste modelo.</span><span class="sxs-lookup"><span data-stu-id="75b7d-151">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="75b7d-152">templateType</span><span class="sxs-lookup"><span data-stu-id="75b7d-152">templateType</span></span>|[<span data-ttu-id="75b7d-153">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="75b7d-153">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="75b7d-154">O tipo do modelo.</span><span class="sxs-lookup"><span data-stu-id="75b7d-154">The template's type.</span></span> <span data-ttu-id="75b7d-155">Os valores possíveis são: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`.</span><span class="sxs-lookup"><span data-stu-id="75b7d-155">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`.</span></span>|
|<span data-ttu-id="75b7d-156">platformType</span><span class="sxs-lookup"><span data-stu-id="75b7d-156">platformType</span></span>|[<span data-ttu-id="75b7d-157">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="75b7d-157">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="75b7d-158">A plataforma do modelo.</span><span class="sxs-lookup"><span data-stu-id="75b7d-158">The template's platform.</span></span> <span data-ttu-id="75b7d-159">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="75b7d-159">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="75b7d-160">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="75b7d-160">publishedDateTime</span></span>|<span data-ttu-id="75b7d-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75b7d-161">DateTimeOffset</span></span>|<span data-ttu-id="75b7d-162">Quando o modelo foi publicado</span><span class="sxs-lookup"><span data-stu-id="75b7d-162">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="75b7d-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="75b7d-163">Response</span></span>
<span data-ttu-id="75b7d-164">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75b7d-164">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75b7d-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75b7d-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="75b7d-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75b7d-166">Request</span></span>
<span data-ttu-id="75b7d-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75b7d-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
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

### <a name="response"></a><span data-ttu-id="75b7d-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="75b7d-168">Response</span></span>
<span data-ttu-id="75b7d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75b7d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 420

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
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```



