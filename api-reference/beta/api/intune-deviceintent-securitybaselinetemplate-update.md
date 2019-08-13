---
title: Atualizar securityBaselineTemplate
description: Atualiza as propriedades de um objeto securityBaselineTemplate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1b1d79b93e63c64365aeba6e026c99ad79cd6c68
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36348946"
---
# <a name="update-securitybaselinetemplate"></a><span data-ttu-id="98f4d-103">Atualizar securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="98f4d-103">Update securityBaselineTemplate</span></span>

> <span data-ttu-id="98f4d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="98f4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98f4d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="98f4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98f4d-106">Atualiza as propriedades de um objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="98f4d-106">Update the properties of a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98f4d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="98f4d-107">Prerequisites</span></span>
<span data-ttu-id="98f4d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98f4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98f4d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98f4d-110">Permission type</span></span>|<span data-ttu-id="98f4d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="98f4d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98f4d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98f4d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="98f4d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98f4d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="98f4d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98f4d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98f4d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98f4d-115">Not supported.</span></span>|
|<span data-ttu-id="98f4d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98f4d-116">Application</span></span>|<span data-ttu-id="98f4d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98f4d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="98f4d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98f4d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="98f4d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98f4d-119">Request headers</span></span>
|<span data-ttu-id="98f4d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="98f4d-120">Header</span></span>|<span data-ttu-id="98f4d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="98f4d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98f4d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="98f4d-122">Authorization</span></span>|<span data-ttu-id="98f4d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98f4d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98f4d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="98f4d-124">Accept</span></span>|<span data-ttu-id="98f4d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="98f4d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98f4d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98f4d-126">Request body</span></span>
<span data-ttu-id="98f4d-127">No corpo da solicitação, forneça uma representação JSON do objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="98f4d-127">In the request body, supply a JSON representation for the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

<span data-ttu-id="98f4d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="98f4d-128">The following table shows the properties that are required when you create the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span></span>

|<span data-ttu-id="98f4d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98f4d-129">Property</span></span>|<span data-ttu-id="98f4d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="98f4d-130">Type</span></span>|<span data-ttu-id="98f4d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="98f4d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98f4d-132">id</span><span class="sxs-lookup"><span data-stu-id="98f4d-132">id</span></span>|<span data-ttu-id="98f4d-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98f4d-133">String</span></span>|<span data-ttu-id="98f4d-134">A ID do modelo herdada de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="98f4d-134">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="98f4d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="98f4d-135">displayName</span></span>|<span data-ttu-id="98f4d-136">String</span><span class="sxs-lookup"><span data-stu-id="98f4d-136">String</span></span>|<span data-ttu-id="98f4d-137">O nome de exibição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="98f4d-137">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="98f4d-138">descrição</span><span class="sxs-lookup"><span data-stu-id="98f4d-138">description</span></span>|<span data-ttu-id="98f4d-139">String</span><span class="sxs-lookup"><span data-stu-id="98f4d-139">String</span></span>|<span data-ttu-id="98f4d-140">A descrição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="98f4d-140">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="98f4d-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="98f4d-141">versionInfo</span></span>|<span data-ttu-id="98f4d-142">String</span><span class="sxs-lookup"><span data-stu-id="98f4d-142">String</span></span>|<span data-ttu-id="98f4d-143">As informações de versão do modelo herdadas de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="98f4d-143">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="98f4d-144">preterido</span><span class="sxs-lookup"><span data-stu-id="98f4d-144">isDeprecated</span></span>|<span data-ttu-id="98f4d-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="98f4d-145">Boolean</span></span>|<span data-ttu-id="98f4d-146">O modelo é preterido ou não.</span><span class="sxs-lookup"><span data-stu-id="98f4d-146">The template is deprecated or not.</span></span> <span data-ttu-id="98f4d-147">Os propósitos não podem ser criados a partir de um modelo preterido.</span><span class="sxs-lookup"><span data-stu-id="98f4d-147">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="98f4d-148">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="98f4d-148">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="98f4d-149">intentCount</span><span class="sxs-lookup"><span data-stu-id="98f4d-149">intentCount</span></span>|<span data-ttu-id="98f4d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="98f4d-150">Int32</span></span>|<span data-ttu-id="98f4d-151">Número de tentativas criadas a partir deste modelo.</span><span class="sxs-lookup"><span data-stu-id="98f4d-151">Number of Intents created from this template.</span></span> <span data-ttu-id="98f4d-152">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="98f4d-152">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="98f4d-153">templateType</span><span class="sxs-lookup"><span data-stu-id="98f4d-153">templateType</span></span>|[<span data-ttu-id="98f4d-154">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="98f4d-154">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="98f4d-155">O tipo do modelo.</span><span class="sxs-lookup"><span data-stu-id="98f4d-155">The template's type.</span></span> <span data-ttu-id="98f4d-156">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="98f4d-156">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="98f4d-157">Os valores possíveis são: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="98f4d-157">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`.</span></span>|
|<span data-ttu-id="98f4d-158">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="98f4d-158">publishedDateTime</span></span>|<span data-ttu-id="98f4d-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98f4d-159">DateTimeOffset</span></span>|<span data-ttu-id="98f4d-160">Quando o modelo foi publicado herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="98f4d-160">When the template was published Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="98f4d-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="98f4d-161">Response</span></span>
<span data-ttu-id="98f4d-162">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98f4d-162">If successful, this method returns a `200 OK` response code and an updated [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98f4d-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98f4d-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="98f4d-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98f4d-164">Request</span></span>
<span data-ttu-id="98f4d-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98f4d-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
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

### <a name="response"></a><span data-ttu-id="98f4d-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="98f4d-166">Response</span></span>
<span data-ttu-id="98f4d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98f4d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






