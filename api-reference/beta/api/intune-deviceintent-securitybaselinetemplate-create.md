---
title: Criar securityBaselineTemplate
description: Criar um novo objeto securityBaselineTemplate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9337b5e9a5108c8dd26cb08287d42406c5a68794
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188826"
---
# <a name="create-securitybaselinetemplate"></a><span data-ttu-id="15f79-103">Criar securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="15f79-103">Create securityBaselineTemplate</span></span>

> <span data-ttu-id="15f79-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="15f79-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15f79-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15f79-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15f79-106">Criar um novo objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="15f79-106">Create a new [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15f79-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15f79-107">Prerequisites</span></span>
<span data-ttu-id="15f79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15f79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15f79-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15f79-110">Permission type</span></span>|<span data-ttu-id="15f79-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="15f79-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15f79-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15f79-112">Delegated (work or school account)</span></span>|<span data-ttu-id="15f79-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15f79-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="15f79-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15f79-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15f79-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15f79-115">Not supported.</span></span>|
|<span data-ttu-id="15f79-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15f79-116">Application</span></span>|<span data-ttu-id="15f79-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15f79-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15f79-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15f79-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="15f79-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15f79-119">Request headers</span></span>
|<span data-ttu-id="15f79-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="15f79-120">Header</span></span>|<span data-ttu-id="15f79-121">Valor</span><span class="sxs-lookup"><span data-stu-id="15f79-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15f79-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="15f79-122">Authorization</span></span>|<span data-ttu-id="15f79-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15f79-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15f79-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="15f79-124">Accept</span></span>|<span data-ttu-id="15f79-125">application/json</span><span class="sxs-lookup"><span data-stu-id="15f79-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15f79-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15f79-126">Request body</span></span>
<span data-ttu-id="15f79-127">No corpo da solicitação, forneça uma representação JSON do objeto securityBaselineTemplate.</span><span class="sxs-lookup"><span data-stu-id="15f79-127">In the request body, supply a JSON representation for the securityBaselineTemplate object.</span></span>

<span data-ttu-id="15f79-128">A tabela a seguir mostra as propriedades que são necessárias ao criar securityBaselineTemplate.</span><span class="sxs-lookup"><span data-stu-id="15f79-128">The following table shows the properties that are required when you create the securityBaselineTemplate.</span></span>

|<span data-ttu-id="15f79-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15f79-129">Property</span></span>|<span data-ttu-id="15f79-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="15f79-130">Type</span></span>|<span data-ttu-id="15f79-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="15f79-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15f79-132">id</span><span class="sxs-lookup"><span data-stu-id="15f79-132">id</span></span>|<span data-ttu-id="15f79-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15f79-133">String</span></span>|<span data-ttu-id="15f79-134">A ID do modelo herdada de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="15f79-134">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="15f79-135">displayName</span><span class="sxs-lookup"><span data-stu-id="15f79-135">displayName</span></span>|<span data-ttu-id="15f79-136">String</span><span class="sxs-lookup"><span data-stu-id="15f79-136">String</span></span>|<span data-ttu-id="15f79-137">O nome de exibição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="15f79-137">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="15f79-138">descrição</span><span class="sxs-lookup"><span data-stu-id="15f79-138">description</span></span>|<span data-ttu-id="15f79-139">String</span><span class="sxs-lookup"><span data-stu-id="15f79-139">String</span></span>|<span data-ttu-id="15f79-140">A descrição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="15f79-140">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="15f79-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="15f79-141">versionInfo</span></span>|<span data-ttu-id="15f79-142">String</span><span class="sxs-lookup"><span data-stu-id="15f79-142">String</span></span>|<span data-ttu-id="15f79-143">As informações de versão do modelo herdadas de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="15f79-143">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="15f79-144">preterido</span><span class="sxs-lookup"><span data-stu-id="15f79-144">isDeprecated</span></span>|<span data-ttu-id="15f79-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="15f79-145">Boolean</span></span>|<span data-ttu-id="15f79-146">O modelo é preterido ou não.</span><span class="sxs-lookup"><span data-stu-id="15f79-146">The template is deprecated or not.</span></span> <span data-ttu-id="15f79-147">Os propósitos não podem ser criados a partir de um modelo preterido.</span><span class="sxs-lookup"><span data-stu-id="15f79-147">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="15f79-148">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="15f79-148">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="15f79-149">intentCount</span><span class="sxs-lookup"><span data-stu-id="15f79-149">intentCount</span></span>|<span data-ttu-id="15f79-150">Int32</span><span class="sxs-lookup"><span data-stu-id="15f79-150">Int32</span></span>|<span data-ttu-id="15f79-151">Número de tentativas criadas a partir deste modelo.</span><span class="sxs-lookup"><span data-stu-id="15f79-151">Number of Intents created from this template.</span></span> <span data-ttu-id="15f79-152">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="15f79-152">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="15f79-153">templateType</span><span class="sxs-lookup"><span data-stu-id="15f79-153">templateType</span></span>|[<span data-ttu-id="15f79-154">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="15f79-154">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="15f79-155">O tipo do modelo.</span><span class="sxs-lookup"><span data-stu-id="15f79-155">The template's type.</span></span> <span data-ttu-id="15f79-156">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="15f79-156">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="15f79-157">Os possíveis valores são: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`.</span><span class="sxs-lookup"><span data-stu-id="15f79-157">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`.</span></span>|
|<span data-ttu-id="15f79-158">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="15f79-158">publishedDateTime</span></span>|<span data-ttu-id="15f79-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15f79-159">DateTimeOffset</span></span>|<span data-ttu-id="15f79-160">Quando o modelo foi publicado herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="15f79-160">When the template was published Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="15f79-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="15f79-161">Response</span></span>
<span data-ttu-id="15f79-162">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15f79-162">If successful, this method returns a `201 Created` response code and a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15f79-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15f79-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="15f79-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15f79-164">Request</span></span>
<span data-ttu-id="15f79-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15f79-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 334

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a><span data-ttu-id="15f79-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="15f79-166">Response</span></span>
<span data-ttu-id="15f79-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15f79-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 383

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```




