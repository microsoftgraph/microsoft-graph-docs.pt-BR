---
title: Criar securityBaselineTemplate
description: Criar um novo objeto securityBaselineTemplate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0d36c5da772bf5b0eeab711ffa156567d0a243db
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33914454"
---
# <a name="create-securitybaselinetemplate"></a><span data-ttu-id="02fab-103">Criar securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="02fab-103">Create securityBaselineTemplate</span></span>

> <span data-ttu-id="02fab-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="02fab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02fab-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02fab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02fab-106">Criar um novo objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="02fab-106">Create a new [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02fab-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02fab-107">Prerequisites</span></span>
<span data-ttu-id="02fab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02fab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02fab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02fab-110">Permission type</span></span>|<span data-ttu-id="02fab-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02fab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02fab-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02fab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="02fab-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02fab-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="02fab-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02fab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02fab-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02fab-115">Not supported.</span></span>|
|<span data-ttu-id="02fab-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02fab-116">Application</span></span>|<span data-ttu-id="02fab-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02fab-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02fab-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02fab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="02fab-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02fab-119">Request headers</span></span>
|<span data-ttu-id="02fab-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02fab-120">Header</span></span>|<span data-ttu-id="02fab-121">Valor</span><span class="sxs-lookup"><span data-stu-id="02fab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02fab-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="02fab-122">Authorization</span></span>|<span data-ttu-id="02fab-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02fab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02fab-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02fab-124">Accept</span></span>|<span data-ttu-id="02fab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="02fab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02fab-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02fab-126">Request body</span></span>
<span data-ttu-id="02fab-127">No corpo da solicitação, forneça uma representação JSON do objeto securityBaselineTemplate.</span><span class="sxs-lookup"><span data-stu-id="02fab-127">In the request body, supply a JSON representation for the securityBaselineTemplate object.</span></span>

<span data-ttu-id="02fab-128">A tabela a seguir mostra as propriedades que são necessárias ao criar securityBaselineTemplate.</span><span class="sxs-lookup"><span data-stu-id="02fab-128">The following table shows the properties that are required when you create the securityBaselineTemplate.</span></span>

|<span data-ttu-id="02fab-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02fab-129">Property</span></span>|<span data-ttu-id="02fab-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="02fab-130">Type</span></span>|<span data-ttu-id="02fab-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="02fab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02fab-132">id</span><span class="sxs-lookup"><span data-stu-id="02fab-132">id</span></span>|<span data-ttu-id="02fab-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02fab-133">String</span></span>|<span data-ttu-id="02fab-134">A ID do modelo herdada de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="02fab-134">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="02fab-135">displayName</span><span class="sxs-lookup"><span data-stu-id="02fab-135">displayName</span></span>|<span data-ttu-id="02fab-136">String</span><span class="sxs-lookup"><span data-stu-id="02fab-136">String</span></span>|<span data-ttu-id="02fab-137">O nome de exibição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="02fab-137">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="02fab-138">description</span><span class="sxs-lookup"><span data-stu-id="02fab-138">description</span></span>|<span data-ttu-id="02fab-139">String</span><span class="sxs-lookup"><span data-stu-id="02fab-139">String</span></span>|<span data-ttu-id="02fab-140">A descrição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="02fab-140">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="02fab-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="02fab-141">versionInfo</span></span>|<span data-ttu-id="02fab-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02fab-142">String</span></span>|<span data-ttu-id="02fab-143">As informações de versão do modelo herdadas de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="02fab-143">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="02fab-144">preterido</span><span class="sxs-lookup"><span data-stu-id="02fab-144">isDeprecated</span></span>|<span data-ttu-id="02fab-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="02fab-145">Boolean</span></span>|<span data-ttu-id="02fab-146">O modelo é preterido ou não.</span><span class="sxs-lookup"><span data-stu-id="02fab-146">The template is deprecated or not.</span></span> <span data-ttu-id="02fab-147">Os propósitos não podem ser criados a partir de um modelo preterido.</span><span class="sxs-lookup"><span data-stu-id="02fab-147">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="02fab-148">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="02fab-148">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="02fab-149">intentCount</span><span class="sxs-lookup"><span data-stu-id="02fab-149">intentCount</span></span>|<span data-ttu-id="02fab-150">Int32</span><span class="sxs-lookup"><span data-stu-id="02fab-150">Int32</span></span>|<span data-ttu-id="02fab-151">Número de tentativas criadas a partir deste modelo.</span><span class="sxs-lookup"><span data-stu-id="02fab-151">Number of Intents created from this template.</span></span> <span data-ttu-id="02fab-152">Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="02fab-152">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="02fab-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="02fab-153">Response</span></span>
<span data-ttu-id="02fab-154">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02fab-154">If successful, this method returns a `201 Created` response code and a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02fab-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02fab-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="02fab-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02fab-156">Request</span></span>
<span data-ttu-id="02fab-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02fab-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 232

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11
}
```

### <a name="response"></a><span data-ttu-id="02fab-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="02fab-158">Response</span></span>
<span data-ttu-id="02fab-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02fab-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 281

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11
}
```




