---
title: Criar deviceManagementTemplate
description: Criar um novo objeto deviceManagementTemplate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f0298ba9d99bd00db8e10e7b5b2afb79a0c7e3ec
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959765"
---
# <a name="create-devicemanagementtemplate"></a><span data-ttu-id="e9ea0-103">Criar deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="e9ea0-103">Create deviceManagementTemplate</span></span>

> <span data-ttu-id="e9ea0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e9ea0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9ea0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e9ea0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9ea0-106">Criar um novo objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="e9ea0-106">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9ea0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e9ea0-107">Prerequisites</span></span>
<span data-ttu-id="e9ea0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9ea0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9ea0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9ea0-110">Permission type</span></span>|<span data-ttu-id="e9ea0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e9ea0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9ea0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9ea0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e9ea0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9ea0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e9ea0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9ea0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9ea0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9ea0-115">Not supported.</span></span>|
|<span data-ttu-id="e9ea0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9ea0-116">Application</span></span>|<span data-ttu-id="e9ea0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9ea0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9ea0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9ea0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="e9ea0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9ea0-119">Request headers</span></span>
|<span data-ttu-id="e9ea0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9ea0-120">Header</span></span>|<span data-ttu-id="e9ea0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e9ea0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9ea0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9ea0-122">Authorization</span></span>|<span data-ttu-id="e9ea0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9ea0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9ea0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e9ea0-124">Accept</span></span>|<span data-ttu-id="e9ea0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e9ea0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9ea0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9ea0-126">Request body</span></span>
<span data-ttu-id="e9ea0-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementTemplate.</span><span class="sxs-lookup"><span data-stu-id="e9ea0-127">In the request body, supply a JSON representation for the deviceManagementTemplate object.</span></span>

<span data-ttu-id="e9ea0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementTemplate.</span><span class="sxs-lookup"><span data-stu-id="e9ea0-128">The following table shows the properties that are required when you create the deviceManagementTemplate.</span></span>

|<span data-ttu-id="e9ea0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9ea0-129">Property</span></span>|<span data-ttu-id="e9ea0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9ea0-130">Type</span></span>|<span data-ttu-id="e9ea0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9ea0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9ea0-132">id</span><span class="sxs-lookup"><span data-stu-id="e9ea0-132">id</span></span>|<span data-ttu-id="e9ea0-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9ea0-133">String</span></span>|<span data-ttu-id="e9ea0-134">A ID do modelo</span><span class="sxs-lookup"><span data-stu-id="e9ea0-134">The template ID</span></span>|
|<span data-ttu-id="e9ea0-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e9ea0-135">displayName</span></span>|<span data-ttu-id="e9ea0-136">String</span><span class="sxs-lookup"><span data-stu-id="e9ea0-136">String</span></span>|<span data-ttu-id="e9ea0-137">O nome de exibição do modelo</span><span class="sxs-lookup"><span data-stu-id="e9ea0-137">The template's display name</span></span>|
|<span data-ttu-id="e9ea0-138">descrição</span><span class="sxs-lookup"><span data-stu-id="e9ea0-138">description</span></span>|<span data-ttu-id="e9ea0-139">String</span><span class="sxs-lookup"><span data-stu-id="e9ea0-139">String</span></span>|<span data-ttu-id="e9ea0-140">A descrição do modelo</span><span class="sxs-lookup"><span data-stu-id="e9ea0-140">The template's description</span></span>|
|<span data-ttu-id="e9ea0-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="e9ea0-141">versionInfo</span></span>|<span data-ttu-id="e9ea0-142">String</span><span class="sxs-lookup"><span data-stu-id="e9ea0-142">String</span></span>|<span data-ttu-id="e9ea0-143">As informações de versão do modelo</span><span class="sxs-lookup"><span data-stu-id="e9ea0-143">The template's version information</span></span>|
|<span data-ttu-id="e9ea0-144">preterido</span><span class="sxs-lookup"><span data-stu-id="e9ea0-144">isDeprecated</span></span>|<span data-ttu-id="e9ea0-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="e9ea0-145">Boolean</span></span>|<span data-ttu-id="e9ea0-146">O modelo é preterido ou não.</span><span class="sxs-lookup"><span data-stu-id="e9ea0-146">The template is deprecated or not.</span></span> <span data-ttu-id="e9ea0-147">Os propósitos não podem ser criados a partir de um modelo preterido.</span><span class="sxs-lookup"><span data-stu-id="e9ea0-147">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="e9ea0-148">intentCount</span><span class="sxs-lookup"><span data-stu-id="e9ea0-148">intentCount</span></span>|<span data-ttu-id="e9ea0-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e9ea0-149">Int32</span></span>|<span data-ttu-id="e9ea0-150">Número de tentativas criadas a partir deste modelo.</span><span class="sxs-lookup"><span data-stu-id="e9ea0-150">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="e9ea0-151">templateType</span><span class="sxs-lookup"><span data-stu-id="e9ea0-151">templateType</span></span>|[<span data-ttu-id="e9ea0-152">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="e9ea0-152">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="e9ea0-153">O tipo do modelo.</span><span class="sxs-lookup"><span data-stu-id="e9ea0-153">The template's type.</span></span> <span data-ttu-id="e9ea0-154">Os valores possíveis são: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="e9ea0-154">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`.</span></span>|
|<span data-ttu-id="e9ea0-155">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="e9ea0-155">publishedDateTime</span></span>|<span data-ttu-id="e9ea0-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9ea0-156">DateTimeOffset</span></span>|<span data-ttu-id="e9ea0-157">Quando o modelo foi publicado</span><span class="sxs-lookup"><span data-stu-id="e9ea0-157">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="e9ea0-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9ea0-158">Response</span></span>
<span data-ttu-id="e9ea0-159">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9ea0-159">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9ea0-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9ea0-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9ea0-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9ea0-161">Request</span></span>
<span data-ttu-id="e9ea0-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9ea0-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 334

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a><span data-ttu-id="e9ea0-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9ea0-163">Response</span></span>
<span data-ttu-id="e9ea0-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9ea0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 383

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```





