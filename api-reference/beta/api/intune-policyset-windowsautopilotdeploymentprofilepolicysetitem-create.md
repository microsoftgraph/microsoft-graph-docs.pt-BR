---
title: Criar windowsAutopilotDeploymentProfilePolicySetItem
description: Criar um novo objeto windowsAutopilotDeploymentProfilePolicySetItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ee70e2c0161d7af7498e0bf8eff12c39f096cdb4
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191702"
---
# <a name="create-windowsautopilotdeploymentprofilepolicysetitem"></a><span data-ttu-id="15e50-103">Criar windowsAutopilotDeploymentProfilePolicySetItem</span><span class="sxs-lookup"><span data-stu-id="15e50-103">Create windowsAutopilotDeploymentProfilePolicySetItem</span></span>

> <span data-ttu-id="15e50-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="15e50-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15e50-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15e50-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15e50-106">Criar um novo objeto [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="15e50-106">Create a new [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15e50-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15e50-107">Prerequisites</span></span>
<span data-ttu-id="15e50-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15e50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15e50-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15e50-110">Permission type</span></span>|<span data-ttu-id="15e50-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="15e50-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15e50-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15e50-112">Delegated (work or school account)</span></span>|<span data-ttu-id="15e50-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15e50-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="15e50-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15e50-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15e50-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15e50-115">Not supported.</span></span>|
|<span data-ttu-id="15e50-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15e50-116">Application</span></span>|<span data-ttu-id="15e50-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15e50-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15e50-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15e50-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="15e50-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15e50-119">Request headers</span></span>
|<span data-ttu-id="15e50-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="15e50-120">Header</span></span>|<span data-ttu-id="15e50-121">Valor</span><span class="sxs-lookup"><span data-stu-id="15e50-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15e50-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="15e50-122">Authorization</span></span>|<span data-ttu-id="15e50-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15e50-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15e50-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="15e50-124">Accept</span></span>|<span data-ttu-id="15e50-125">application/json</span><span class="sxs-lookup"><span data-stu-id="15e50-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15e50-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15e50-126">Request body</span></span>
<span data-ttu-id="15e50-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsAutopilotDeploymentProfilePolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="15e50-127">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfilePolicySetItem object.</span></span>

<span data-ttu-id="15e50-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsAutopilotDeploymentProfilePolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="15e50-128">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfilePolicySetItem.</span></span>

|<span data-ttu-id="15e50-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15e50-129">Property</span></span>|<span data-ttu-id="15e50-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="15e50-130">Type</span></span>|<span data-ttu-id="15e50-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="15e50-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15e50-132">id</span><span class="sxs-lookup"><span data-stu-id="15e50-132">id</span></span>|<span data-ttu-id="15e50-133">String</span><span class="sxs-lookup"><span data-stu-id="15e50-133">String</span></span>|<span data-ttu-id="15e50-134">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="15e50-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="15e50-135">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="15e50-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="15e50-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15e50-136">createdDateTime</span></span>|<span data-ttu-id="15e50-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15e50-137">DateTimeOffset</span></span>|<span data-ttu-id="15e50-138">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="15e50-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="15e50-139">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="15e50-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="15e50-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15e50-140">lastModifiedDateTime</span></span>|<span data-ttu-id="15e50-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15e50-141">DateTimeOffset</span></span>|<span data-ttu-id="15e50-142">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="15e50-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="15e50-143">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="15e50-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="15e50-144">payloadId</span><span class="sxs-lookup"><span data-stu-id="15e50-144">payloadId</span></span>|<span data-ttu-id="15e50-145">String</span><span class="sxs-lookup"><span data-stu-id="15e50-145">String</span></span>|<span data-ttu-id="15e50-146">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="15e50-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="15e50-147">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="15e50-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="15e50-148">itemType</span><span class="sxs-lookup"><span data-stu-id="15e50-148">itemType</span></span>|<span data-ttu-id="15e50-149">String</span><span class="sxs-lookup"><span data-stu-id="15e50-149">String</span></span>|<span data-ttu-id="15e50-150">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="15e50-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="15e50-151">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="15e50-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="15e50-152">displayName</span><span class="sxs-lookup"><span data-stu-id="15e50-152">displayName</span></span>|<span data-ttu-id="15e50-153">String</span><span class="sxs-lookup"><span data-stu-id="15e50-153">String</span></span>|<span data-ttu-id="15e50-154">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="15e50-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="15e50-155">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="15e50-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="15e50-156">status</span><span class="sxs-lookup"><span data-stu-id="15e50-156">status</span></span>|[<span data-ttu-id="15e50-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="15e50-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="15e50-158">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="15e50-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="15e50-159">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="15e50-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="15e50-160">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="15e50-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="15e50-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="15e50-161">errorCode</span></span>|[<span data-ttu-id="15e50-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="15e50-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="15e50-163">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="15e50-163">Error code if any occured.</span></span> <span data-ttu-id="15e50-164">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="15e50-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="15e50-165">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="15e50-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="15e50-166">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="15e50-166">guidedDeploymentTags</span></span>|<span data-ttu-id="15e50-167">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="15e50-167">String collection</span></span>|<span data-ttu-id="15e50-168">Marcas da implantação dirigida herdadas de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="15e50-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="15e50-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="15e50-169">Response</span></span>
<span data-ttu-id="15e50-170">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15e50-170">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15e50-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15e50-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="15e50-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15e50-172">Request</span></span>
<span data-ttu-id="15e50-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15e50-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
Content-type: application/json
Content-length: 328

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfilePolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="15e50-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="15e50-174">Response</span></span>
<span data-ttu-id="15e50-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15e50-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 500

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfilePolicySetItem",
  "id": "850e84d8-84d8-850e-d884-0e85d8840e85",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ]
}
```




