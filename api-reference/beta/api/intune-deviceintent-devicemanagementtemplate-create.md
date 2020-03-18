---
title: Criar deviceManagementTemplate
description: Criar um novo objeto deviceManagementTemplate.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0873e16f719d27b5f8288ee2209aa61f282917b4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42765248"
---
# <a name="create-devicemanagementtemplate"></a><span data-ttu-id="91cba-103">Criar deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="91cba-103">Create deviceManagementTemplate</span></span>

> <span data-ttu-id="91cba-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="91cba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91cba-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91cba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91cba-106">Criar um novo objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="91cba-106">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91cba-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="91cba-107">Prerequisites</span></span>
<span data-ttu-id="91cba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91cba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91cba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91cba-110">Permission type</span></span>|<span data-ttu-id="91cba-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="91cba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91cba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91cba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="91cba-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91cba-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="91cba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91cba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91cba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91cba-115">Not supported.</span></span>|
|<span data-ttu-id="91cba-116">Application</span><span class="sxs-lookup"><span data-stu-id="91cba-116">Application</span></span>|<span data-ttu-id="91cba-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91cba-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91cba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91cba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="91cba-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91cba-119">Request headers</span></span>
|<span data-ttu-id="91cba-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91cba-120">Header</span></span>|<span data-ttu-id="91cba-121">Valor</span><span class="sxs-lookup"><span data-stu-id="91cba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91cba-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="91cba-122">Authorization</span></span>|<span data-ttu-id="91cba-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91cba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91cba-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="91cba-124">Accept</span></span>|<span data-ttu-id="91cba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="91cba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91cba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91cba-126">Request body</span></span>
<span data-ttu-id="91cba-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementTemplate.</span><span class="sxs-lookup"><span data-stu-id="91cba-127">In the request body, supply a JSON representation for the deviceManagementTemplate object.</span></span>

<span data-ttu-id="91cba-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementTemplate.</span><span class="sxs-lookup"><span data-stu-id="91cba-128">The following table shows the properties that are required when you create the deviceManagementTemplate.</span></span>

|<span data-ttu-id="91cba-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91cba-129">Property</span></span>|<span data-ttu-id="91cba-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="91cba-130">Type</span></span>|<span data-ttu-id="91cba-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="91cba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91cba-132">id</span><span class="sxs-lookup"><span data-stu-id="91cba-132">id</span></span>|<span data-ttu-id="91cba-133">String</span><span class="sxs-lookup"><span data-stu-id="91cba-133">String</span></span>|<span data-ttu-id="91cba-134">A ID do modelo</span><span class="sxs-lookup"><span data-stu-id="91cba-134">The template ID</span></span>|
|<span data-ttu-id="91cba-135">displayName</span><span class="sxs-lookup"><span data-stu-id="91cba-135">displayName</span></span>|<span data-ttu-id="91cba-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91cba-136">String</span></span>|<span data-ttu-id="91cba-137">O nome de exibição do modelo</span><span class="sxs-lookup"><span data-stu-id="91cba-137">The template's display name</span></span>|
|<span data-ttu-id="91cba-138">description</span><span class="sxs-lookup"><span data-stu-id="91cba-138">description</span></span>|<span data-ttu-id="91cba-139">String</span><span class="sxs-lookup"><span data-stu-id="91cba-139">String</span></span>|<span data-ttu-id="91cba-140">A descrição do modelo</span><span class="sxs-lookup"><span data-stu-id="91cba-140">The template's description</span></span>|
|<span data-ttu-id="91cba-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="91cba-141">versionInfo</span></span>|<span data-ttu-id="91cba-142">String</span><span class="sxs-lookup"><span data-stu-id="91cba-142">String</span></span>|<span data-ttu-id="91cba-143">As informações de versão do modelo</span><span class="sxs-lookup"><span data-stu-id="91cba-143">The template's version information</span></span>|
|<span data-ttu-id="91cba-144">preterido</span><span class="sxs-lookup"><span data-stu-id="91cba-144">isDeprecated</span></span>|<span data-ttu-id="91cba-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="91cba-145">Boolean</span></span>|<span data-ttu-id="91cba-146">O modelo é preterido ou não.</span><span class="sxs-lookup"><span data-stu-id="91cba-146">The template is deprecated or not.</span></span> <span data-ttu-id="91cba-147">Os propósitos não podem ser criados a partir de um modelo preterido.</span><span class="sxs-lookup"><span data-stu-id="91cba-147">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="91cba-148">intentCount</span><span class="sxs-lookup"><span data-stu-id="91cba-148">intentCount</span></span>|<span data-ttu-id="91cba-149">Int32</span><span class="sxs-lookup"><span data-stu-id="91cba-149">Int32</span></span>|<span data-ttu-id="91cba-150">Número de tentativas criadas a partir deste modelo.</span><span class="sxs-lookup"><span data-stu-id="91cba-150">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="91cba-151">templateType</span><span class="sxs-lookup"><span data-stu-id="91cba-151">templateType</span></span>|[<span data-ttu-id="91cba-152">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="91cba-152">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="91cba-153">O tipo do modelo.</span><span class="sxs-lookup"><span data-stu-id="91cba-153">The template's type.</span></span> <span data-ttu-id="91cba-154">Os valores possíveis são: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`.</span><span class="sxs-lookup"><span data-stu-id="91cba-154">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`.</span></span>|
|<span data-ttu-id="91cba-155">platformType</span><span class="sxs-lookup"><span data-stu-id="91cba-155">platformType</span></span>|[<span data-ttu-id="91cba-156">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="91cba-156">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="91cba-157">A plataforma do modelo.</span><span class="sxs-lookup"><span data-stu-id="91cba-157">The template's platform.</span></span> <span data-ttu-id="91cba-158">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="91cba-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="91cba-159">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="91cba-159">publishedDateTime</span></span>|<span data-ttu-id="91cba-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91cba-160">DateTimeOffset</span></span>|<span data-ttu-id="91cba-161">Quando o modelo foi publicado</span><span class="sxs-lookup"><span data-stu-id="91cba-161">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="91cba-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="91cba-162">Response</span></span>
<span data-ttu-id="91cba-163">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91cba-163">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91cba-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91cba-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="91cba-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91cba-165">Request</span></span>
<span data-ttu-id="91cba-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91cba-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="91cba-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="91cba-167">Response</span></span>
<span data-ttu-id="91cba-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91cba-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




