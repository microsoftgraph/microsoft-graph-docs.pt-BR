---
title: Atualizar deviceManagementTemplate
description: Atualiza as propriedades de um objeto deviceManagementTemplate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a31fac90cf11035457c3dccdddbd6411a96bc399
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188966"
---
# <a name="update-devicemanagementtemplate"></a><span data-ttu-id="7bb62-103">Atualizar deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="7bb62-103">Update deviceManagementTemplate</span></span>

> <span data-ttu-id="7bb62-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7bb62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bb62-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7bb62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bb62-106">Atualiza as propriedades de um objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="7bb62-106">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7bb62-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7bb62-107">Prerequisites</span></span>
<span data-ttu-id="7bb62-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bb62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bb62-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7bb62-110">Permission type</span></span>|<span data-ttu-id="7bb62-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7bb62-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bb62-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7bb62-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7bb62-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bb62-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7bb62-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7bb62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bb62-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bb62-115">Not supported.</span></span>|
|<span data-ttu-id="7bb62-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bb62-116">Application</span></span>|<span data-ttu-id="7bb62-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bb62-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bb62-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7bb62-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="7bb62-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7bb62-119">Request headers</span></span>
|<span data-ttu-id="7bb62-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7bb62-120">Header</span></span>|<span data-ttu-id="7bb62-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7bb62-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7bb62-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7bb62-122">Authorization</span></span>|<span data-ttu-id="7bb62-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bb62-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7bb62-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7bb62-124">Accept</span></span>|<span data-ttu-id="7bb62-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7bb62-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bb62-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7bb62-126">Request body</span></span>
<span data-ttu-id="7bb62-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="7bb62-127">In the request body, supply a JSON representation for the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

<span data-ttu-id="7bb62-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="7bb62-128">The following table shows the properties that are required when you create the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>

|<span data-ttu-id="7bb62-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bb62-129">Property</span></span>|<span data-ttu-id="7bb62-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bb62-130">Type</span></span>|<span data-ttu-id="7bb62-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bb62-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bb62-132">id</span><span class="sxs-lookup"><span data-stu-id="7bb62-132">id</span></span>|<span data-ttu-id="7bb62-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bb62-133">String</span></span>|<span data-ttu-id="7bb62-134">A ID do modelo</span><span class="sxs-lookup"><span data-stu-id="7bb62-134">The template ID</span></span>|
|<span data-ttu-id="7bb62-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7bb62-135">displayName</span></span>|<span data-ttu-id="7bb62-136">String</span><span class="sxs-lookup"><span data-stu-id="7bb62-136">String</span></span>|<span data-ttu-id="7bb62-137">O nome de exibição do modelo</span><span class="sxs-lookup"><span data-stu-id="7bb62-137">The template's display name</span></span>|
|<span data-ttu-id="7bb62-138">descrição</span><span class="sxs-lookup"><span data-stu-id="7bb62-138">description</span></span>|<span data-ttu-id="7bb62-139">String</span><span class="sxs-lookup"><span data-stu-id="7bb62-139">String</span></span>|<span data-ttu-id="7bb62-140">A descrição do modelo</span><span class="sxs-lookup"><span data-stu-id="7bb62-140">The template's description</span></span>|
|<span data-ttu-id="7bb62-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="7bb62-141">versionInfo</span></span>|<span data-ttu-id="7bb62-142">String</span><span class="sxs-lookup"><span data-stu-id="7bb62-142">String</span></span>|<span data-ttu-id="7bb62-143">As informações de versão do modelo</span><span class="sxs-lookup"><span data-stu-id="7bb62-143">The template's version information</span></span>|
|<span data-ttu-id="7bb62-144">preterido</span><span class="sxs-lookup"><span data-stu-id="7bb62-144">isDeprecated</span></span>|<span data-ttu-id="7bb62-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="7bb62-145">Boolean</span></span>|<span data-ttu-id="7bb62-146">O modelo é preterido ou não.</span><span class="sxs-lookup"><span data-stu-id="7bb62-146">The template is deprecated or not.</span></span> <span data-ttu-id="7bb62-147">Os propósitos não podem ser criados a partir de um modelo preterido.</span><span class="sxs-lookup"><span data-stu-id="7bb62-147">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="7bb62-148">intentCount</span><span class="sxs-lookup"><span data-stu-id="7bb62-148">intentCount</span></span>|<span data-ttu-id="7bb62-149">Int32</span><span class="sxs-lookup"><span data-stu-id="7bb62-149">Int32</span></span>|<span data-ttu-id="7bb62-150">Número de tentativas criadas a partir deste modelo.</span><span class="sxs-lookup"><span data-stu-id="7bb62-150">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="7bb62-151">templateType</span><span class="sxs-lookup"><span data-stu-id="7bb62-151">templateType</span></span>|[<span data-ttu-id="7bb62-152">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="7bb62-152">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="7bb62-153">O tipo do modelo.</span><span class="sxs-lookup"><span data-stu-id="7bb62-153">The template's type.</span></span> <span data-ttu-id="7bb62-154">Os possíveis valores são: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`.</span><span class="sxs-lookup"><span data-stu-id="7bb62-154">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`.</span></span>|
|<span data-ttu-id="7bb62-155">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="7bb62-155">publishedDateTime</span></span>|<span data-ttu-id="7bb62-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bb62-156">DateTimeOffset</span></span>|<span data-ttu-id="7bb62-157">Quando o modelo foi publicado</span><span class="sxs-lookup"><span data-stu-id="7bb62-157">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="7bb62-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bb62-158">Response</span></span>
<span data-ttu-id="7bb62-159">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7bb62-159">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bb62-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7bb62-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="7bb62-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bb62-161">Request</span></span>
<span data-ttu-id="7bb62-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7bb62-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
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

### <a name="response"></a><span data-ttu-id="7bb62-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bb62-163">Response</span></span>
<span data-ttu-id="7bb62-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7bb62-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




