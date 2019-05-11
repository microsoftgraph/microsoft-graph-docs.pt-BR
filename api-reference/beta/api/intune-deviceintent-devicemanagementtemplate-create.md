---
title: Criar deviceManagementTemplate
description: Criar um novo objeto deviceManagementTemplate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 102fa662dd9cf6eef9a4949f8dc9250e69cfadbf
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33915983"
---
# <a name="create-devicemanagementtemplate"></a><span data-ttu-id="7a792-103">Criar deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="7a792-103">Create deviceManagementTemplate</span></span>

> <span data-ttu-id="7a792-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7a792-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a792-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7a792-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a792-106">Criar um novo objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="7a792-106">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a792-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7a792-107">Prerequisites</span></span>
<span data-ttu-id="7a792-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a792-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a792-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a792-110">Permission type</span></span>|<span data-ttu-id="7a792-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7a792-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a792-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a792-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7a792-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a792-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7a792-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a792-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a792-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a792-115">Not supported.</span></span>|
|<span data-ttu-id="7a792-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a792-116">Application</span></span>|<span data-ttu-id="7a792-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a792-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a792-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a792-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="7a792-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a792-119">Request headers</span></span>
|<span data-ttu-id="7a792-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7a792-120">Header</span></span>|<span data-ttu-id="7a792-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7a792-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a792-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a792-122">Authorization</span></span>|<span data-ttu-id="7a792-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a792-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a792-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7a792-124">Accept</span></span>|<span data-ttu-id="7a792-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7a792-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a792-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a792-126">Request body</span></span>
<span data-ttu-id="7a792-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementTemplate.</span><span class="sxs-lookup"><span data-stu-id="7a792-127">In the request body, supply a JSON representation for the deviceManagementTemplate object.</span></span>

<span data-ttu-id="7a792-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementTemplate.</span><span class="sxs-lookup"><span data-stu-id="7a792-128">The following table shows the properties that are required when you create the deviceManagementTemplate.</span></span>

|<span data-ttu-id="7a792-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a792-129">Property</span></span>|<span data-ttu-id="7a792-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a792-130">Type</span></span>|<span data-ttu-id="7a792-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a792-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a792-132">id</span><span class="sxs-lookup"><span data-stu-id="7a792-132">id</span></span>|<span data-ttu-id="7a792-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a792-133">String</span></span>|<span data-ttu-id="7a792-134">A ID do modelo</span><span class="sxs-lookup"><span data-stu-id="7a792-134">The template ID</span></span>|
|<span data-ttu-id="7a792-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7a792-135">displayName</span></span>|<span data-ttu-id="7a792-136">String</span><span class="sxs-lookup"><span data-stu-id="7a792-136">String</span></span>|<span data-ttu-id="7a792-137">O nome de exibição do modelo</span><span class="sxs-lookup"><span data-stu-id="7a792-137">The template's display name</span></span>|
|<span data-ttu-id="7a792-138">description</span><span class="sxs-lookup"><span data-stu-id="7a792-138">description</span></span>|<span data-ttu-id="7a792-139">String</span><span class="sxs-lookup"><span data-stu-id="7a792-139">String</span></span>|<span data-ttu-id="7a792-140">A descrição do modelo</span><span class="sxs-lookup"><span data-stu-id="7a792-140">The template's description</span></span>|
|<span data-ttu-id="7a792-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="7a792-141">versionInfo</span></span>|<span data-ttu-id="7a792-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a792-142">String</span></span>|<span data-ttu-id="7a792-143">As informações de versão do modelo</span><span class="sxs-lookup"><span data-stu-id="7a792-143">The template's version information</span></span>|
|<span data-ttu-id="7a792-144">preterido</span><span class="sxs-lookup"><span data-stu-id="7a792-144">isDeprecated</span></span>|<span data-ttu-id="7a792-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="7a792-145">Boolean</span></span>|<span data-ttu-id="7a792-146">O modelo é preterido ou não.</span><span class="sxs-lookup"><span data-stu-id="7a792-146">The template is deprecated or not.</span></span> <span data-ttu-id="7a792-147">Os propósitos não podem ser criados a partir de um modelo preterido.</span><span class="sxs-lookup"><span data-stu-id="7a792-147">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="7a792-148">intentCount</span><span class="sxs-lookup"><span data-stu-id="7a792-148">intentCount</span></span>|<span data-ttu-id="7a792-149">Int32</span><span class="sxs-lookup"><span data-stu-id="7a792-149">Int32</span></span>|<span data-ttu-id="7a792-150">Número de tentativas criadas a partir deste modelo.</span><span class="sxs-lookup"><span data-stu-id="7a792-150">Number of Intents created from this template.</span></span>|



## <a name="response"></a><span data-ttu-id="7a792-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a792-151">Response</span></span>
<span data-ttu-id="7a792-152">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a792-152">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a792-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a792-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a792-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a792-154">Request</span></span>
<span data-ttu-id="7a792-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a792-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 232

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11
}
```

### <a name="response"></a><span data-ttu-id="7a792-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a792-156">Response</span></span>
<span data-ttu-id="7a792-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a792-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 281

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11
}
```




