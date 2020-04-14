---
title: Atualizar windowsAutopilotDeploymentProfilePolicySetItem
description: Atualiza as propriedades de um objeto windowsAutopilotDeploymentProfilePolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bf52e7b5819fa12b0b4b40962f86bc8bef1e2b1b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437888"
---
# <a name="update-windowsautopilotdeploymentprofilepolicysetitem"></a><span data-ttu-id="75650-103">Atualizar windowsAutopilotDeploymentProfilePolicySetItem</span><span class="sxs-lookup"><span data-stu-id="75650-103">Update windowsAutopilotDeploymentProfilePolicySetItem</span></span>

<span data-ttu-id="75650-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75650-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75650-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="75650-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75650-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75650-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75650-107">Atualiza as propriedades de um objeto [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="75650-107">Update the properties of a [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75650-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="75650-108">Prerequisites</span></span>
<span data-ttu-id="75650-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75650-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75650-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75650-111">Permission type</span></span>|<span data-ttu-id="75650-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="75650-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75650-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75650-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75650-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75650-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75650-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75650-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75650-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75650-116">Not supported.</span></span>|
|<span data-ttu-id="75650-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75650-117">Application</span></span>|<span data-ttu-id="75650-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75650-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75650-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75650-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="75650-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75650-120">Request headers</span></span>
|<span data-ttu-id="75650-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="75650-121">Header</span></span>|<span data-ttu-id="75650-122">Valor</span><span class="sxs-lookup"><span data-stu-id="75650-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75650-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="75650-123">Authorization</span></span>|<span data-ttu-id="75650-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75650-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75650-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="75650-125">Accept</span></span>|<span data-ttu-id="75650-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75650-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75650-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75650-127">Request body</span></span>
<span data-ttu-id="75650-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="75650-128">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object.</span></span>

<span data-ttu-id="75650-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="75650-129">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md).</span></span>

|<span data-ttu-id="75650-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75650-130">Property</span></span>|<span data-ttu-id="75650-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="75650-131">Type</span></span>|<span data-ttu-id="75650-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="75650-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75650-133">id</span><span class="sxs-lookup"><span data-stu-id="75650-133">id</span></span>|<span data-ttu-id="75650-134">String</span><span class="sxs-lookup"><span data-stu-id="75650-134">String</span></span>|<span data-ttu-id="75650-135">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="75650-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="75650-136">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="75650-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="75650-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75650-137">createdDateTime</span></span>|<span data-ttu-id="75650-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75650-138">DateTimeOffset</span></span>|<span data-ttu-id="75650-139">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="75650-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="75650-140">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="75650-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="75650-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75650-141">lastModifiedDateTime</span></span>|<span data-ttu-id="75650-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75650-142">DateTimeOffset</span></span>|<span data-ttu-id="75650-143">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="75650-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="75650-144">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="75650-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="75650-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="75650-145">payloadId</span></span>|<span data-ttu-id="75650-146">String</span><span class="sxs-lookup"><span data-stu-id="75650-146">String</span></span>|<span data-ttu-id="75650-147">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="75650-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="75650-148">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="75650-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="75650-149">itemType</span><span class="sxs-lookup"><span data-stu-id="75650-149">itemType</span></span>|<span data-ttu-id="75650-150">String</span><span class="sxs-lookup"><span data-stu-id="75650-150">String</span></span>|<span data-ttu-id="75650-151">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="75650-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="75650-152">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="75650-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="75650-153">displayName</span><span class="sxs-lookup"><span data-stu-id="75650-153">displayName</span></span>|<span data-ttu-id="75650-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75650-154">String</span></span>|<span data-ttu-id="75650-155">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="75650-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="75650-156">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="75650-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="75650-157">status</span><span class="sxs-lookup"><span data-stu-id="75650-157">status</span></span>|[<span data-ttu-id="75650-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="75650-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="75650-159">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="75650-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="75650-160">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="75650-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="75650-161">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="75650-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="75650-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="75650-162">errorCode</span></span>|[<span data-ttu-id="75650-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="75650-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="75650-164">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="75650-164">Error code if any occured.</span></span> <span data-ttu-id="75650-165">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="75650-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="75650-166">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="75650-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="75650-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="75650-167">guidedDeploymentTags</span></span>|<span data-ttu-id="75650-168">Coleção String</span><span class="sxs-lookup"><span data-stu-id="75650-168">String collection</span></span>|<span data-ttu-id="75650-169">Marcas da implantação dirigida herdadas de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="75650-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="75650-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="75650-170">Response</span></span>
<span data-ttu-id="75650-171">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75650-171">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75650-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75650-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="75650-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75650-173">Request</span></span>
<span data-ttu-id="75650-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75650-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
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

### <a name="response"></a><span data-ttu-id="75650-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="75650-175">Response</span></span>
<span data-ttu-id="75650-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75650-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



