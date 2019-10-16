---
title: Atualizar deviceManagementTemplate
description: Atualiza as propriedades de um objeto deviceManagementTemplate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f05999d160b2fd947f4c44f3130c95aa34756e07
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37532054"
---
# <a name="update-devicemanagementtemplate"></a><span data-ttu-id="fd0c5-103">Atualizar deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="fd0c5-103">Update deviceManagementTemplate</span></span>

> <span data-ttu-id="fd0c5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fd0c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd0c5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fd0c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd0c5-106">Atualiza as propriedades de um objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="fd0c5-106">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd0c5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fd0c5-107">Prerequisites</span></span>
<span data-ttu-id="fd0c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd0c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd0c5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd0c5-110">Permission type</span></span>|<span data-ttu-id="fd0c5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fd0c5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd0c5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd0c5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fd0c5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd0c5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fd0c5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd0c5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd0c5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd0c5-115">Not supported.</span></span>|
|<span data-ttu-id="fd0c5-116">Application</span><span class="sxs-lookup"><span data-stu-id="fd0c5-116">Application</span></span>|<span data-ttu-id="fd0c5-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd0c5-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd0c5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd0c5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="fd0c5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd0c5-119">Request headers</span></span>
|<span data-ttu-id="fd0c5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fd0c5-120">Header</span></span>|<span data-ttu-id="fd0c5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fd0c5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd0c5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd0c5-122">Authorization</span></span>|<span data-ttu-id="fd0c5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd0c5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd0c5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fd0c5-124">Accept</span></span>|<span data-ttu-id="fd0c5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fd0c5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd0c5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd0c5-126">Request body</span></span>
<span data-ttu-id="fd0c5-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="fd0c5-127">In the request body, supply a JSON representation for the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

<span data-ttu-id="fd0c5-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="fd0c5-128">The following table shows the properties that are required when you create the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>

|<span data-ttu-id="fd0c5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd0c5-129">Property</span></span>|<span data-ttu-id="fd0c5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd0c5-130">Type</span></span>|<span data-ttu-id="fd0c5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd0c5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd0c5-132">id</span><span class="sxs-lookup"><span data-stu-id="fd0c5-132">id</span></span>|<span data-ttu-id="fd0c5-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd0c5-133">String</span></span>|<span data-ttu-id="fd0c5-134">A ID do modelo</span><span class="sxs-lookup"><span data-stu-id="fd0c5-134">The template ID</span></span>|
|<span data-ttu-id="fd0c5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="fd0c5-135">displayName</span></span>|<span data-ttu-id="fd0c5-136">String</span><span class="sxs-lookup"><span data-stu-id="fd0c5-136">String</span></span>|<span data-ttu-id="fd0c5-137">O nome de exibição do modelo</span><span class="sxs-lookup"><span data-stu-id="fd0c5-137">The template's display name</span></span>|
|<span data-ttu-id="fd0c5-138">description</span><span class="sxs-lookup"><span data-stu-id="fd0c5-138">description</span></span>|<span data-ttu-id="fd0c5-139">String</span><span class="sxs-lookup"><span data-stu-id="fd0c5-139">String</span></span>|<span data-ttu-id="fd0c5-140">A descrição do modelo</span><span class="sxs-lookup"><span data-stu-id="fd0c5-140">The template's description</span></span>|
|<span data-ttu-id="fd0c5-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="fd0c5-141">versionInfo</span></span>|<span data-ttu-id="fd0c5-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd0c5-142">String</span></span>|<span data-ttu-id="fd0c5-143">As informações de versão do modelo</span><span class="sxs-lookup"><span data-stu-id="fd0c5-143">The template's version information</span></span>|
|<span data-ttu-id="fd0c5-144">preterido</span><span class="sxs-lookup"><span data-stu-id="fd0c5-144">isDeprecated</span></span>|<span data-ttu-id="fd0c5-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="fd0c5-145">Boolean</span></span>|<span data-ttu-id="fd0c5-146">O modelo é preterido ou não.</span><span class="sxs-lookup"><span data-stu-id="fd0c5-146">The template is deprecated or not.</span></span> <span data-ttu-id="fd0c5-147">Os propósitos não podem ser criados a partir de um modelo preterido.</span><span class="sxs-lookup"><span data-stu-id="fd0c5-147">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="fd0c5-148">intentCount</span><span class="sxs-lookup"><span data-stu-id="fd0c5-148">intentCount</span></span>|<span data-ttu-id="fd0c5-149">Int32</span><span class="sxs-lookup"><span data-stu-id="fd0c5-149">Int32</span></span>|<span data-ttu-id="fd0c5-150">Número de tentativas criadas a partir deste modelo.</span><span class="sxs-lookup"><span data-stu-id="fd0c5-150">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="fd0c5-151">templateType</span><span class="sxs-lookup"><span data-stu-id="fd0c5-151">templateType</span></span>|[<span data-ttu-id="fd0c5-152">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="fd0c5-152">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="fd0c5-153">O tipo do modelo.</span><span class="sxs-lookup"><span data-stu-id="fd0c5-153">The template's type.</span></span> <span data-ttu-id="fd0c5-154">Os valores possíveis são: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`.</span><span class="sxs-lookup"><span data-stu-id="fd0c5-154">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`.</span></span>|
|<span data-ttu-id="fd0c5-155">platformType</span><span class="sxs-lookup"><span data-stu-id="fd0c5-155">platformType</span></span>|[<span data-ttu-id="fd0c5-156">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="fd0c5-156">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="fd0c5-157">A plataforma do modelo.</span><span class="sxs-lookup"><span data-stu-id="fd0c5-157">The template's platform.</span></span> <span data-ttu-id="fd0c5-158">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="fd0c5-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="fd0c5-159">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd0c5-159">publishedDateTime</span></span>|<span data-ttu-id="fd0c5-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd0c5-160">DateTimeOffset</span></span>|<span data-ttu-id="fd0c5-161">Quando o modelo foi publicado</span><span class="sxs-lookup"><span data-stu-id="fd0c5-161">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="fd0c5-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd0c5-162">Response</span></span>
<span data-ttu-id="fd0c5-163">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd0c5-163">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd0c5-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd0c5-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd0c5-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd0c5-165">Request</span></span>
<span data-ttu-id="fd0c5-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd0c5-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
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

### <a name="response"></a><span data-ttu-id="fd0c5-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd0c5-167">Response</span></span>
<span data-ttu-id="fd0c5-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd0c5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






