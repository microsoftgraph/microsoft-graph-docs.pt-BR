---
title: Criar windowsAutopilotDeploymentProfilePolicySetItem
description: Criar um novo objeto windowsAutopilotDeploymentProfilePolicySetItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9c505f86c3643d26fe81eb1890d9537c1a818126
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42460294"
---
# <a name="create-windowsautopilotdeploymentprofilepolicysetitem"></a><span data-ttu-id="29e6c-103">Criar windowsAutopilotDeploymentProfilePolicySetItem</span><span class="sxs-lookup"><span data-stu-id="29e6c-103">Create windowsAutopilotDeploymentProfilePolicySetItem</span></span>

<span data-ttu-id="29e6c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="29e6c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29e6c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="29e6c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29e6c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="29e6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29e6c-107">Criar um novo objeto [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="29e6c-107">Create a new [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29e6c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="29e6c-108">Prerequisites</span></span>
<span data-ttu-id="29e6c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29e6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29e6c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29e6c-111">Permission type</span></span>|<span data-ttu-id="29e6c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="29e6c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29e6c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29e6c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29e6c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29e6c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="29e6c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29e6c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29e6c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29e6c-116">Not supported.</span></span>|
|<span data-ttu-id="29e6c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29e6c-117">Application</span></span>|<span data-ttu-id="29e6c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29e6c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29e6c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29e6c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="29e6c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29e6c-120">Request headers</span></span>
|<span data-ttu-id="29e6c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29e6c-121">Header</span></span>|<span data-ttu-id="29e6c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="29e6c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29e6c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="29e6c-123">Authorization</span></span>|<span data-ttu-id="29e6c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29e6c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29e6c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="29e6c-125">Accept</span></span>|<span data-ttu-id="29e6c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29e6c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29e6c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29e6c-127">Request body</span></span>
<span data-ttu-id="29e6c-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsAutopilotDeploymentProfilePolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="29e6c-128">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfilePolicySetItem object.</span></span>

<span data-ttu-id="29e6c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsAutopilotDeploymentProfilePolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="29e6c-129">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfilePolicySetItem.</span></span>

|<span data-ttu-id="29e6c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29e6c-130">Property</span></span>|<span data-ttu-id="29e6c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="29e6c-131">Type</span></span>|<span data-ttu-id="29e6c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="29e6c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29e6c-133">id</span><span class="sxs-lookup"><span data-stu-id="29e6c-133">id</span></span>|<span data-ttu-id="29e6c-134">String</span><span class="sxs-lookup"><span data-stu-id="29e6c-134">String</span></span>|<span data-ttu-id="29e6c-135">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="29e6c-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="29e6c-136">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="29e6c-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="29e6c-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29e6c-137">createdDateTime</span></span>|<span data-ttu-id="29e6c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29e6c-138">DateTimeOffset</span></span>|<span data-ttu-id="29e6c-139">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="29e6c-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="29e6c-140">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="29e6c-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="29e6c-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29e6c-141">lastModifiedDateTime</span></span>|<span data-ttu-id="29e6c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29e6c-142">DateTimeOffset</span></span>|<span data-ttu-id="29e6c-143">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="29e6c-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="29e6c-144">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="29e6c-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="29e6c-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="29e6c-145">payloadId</span></span>|<span data-ttu-id="29e6c-146">String</span><span class="sxs-lookup"><span data-stu-id="29e6c-146">String</span></span>|<span data-ttu-id="29e6c-147">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="29e6c-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="29e6c-148">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="29e6c-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="29e6c-149">itemType</span><span class="sxs-lookup"><span data-stu-id="29e6c-149">itemType</span></span>|<span data-ttu-id="29e6c-150">String</span><span class="sxs-lookup"><span data-stu-id="29e6c-150">String</span></span>|<span data-ttu-id="29e6c-151">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="29e6c-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="29e6c-152">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="29e6c-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="29e6c-153">displayName</span><span class="sxs-lookup"><span data-stu-id="29e6c-153">displayName</span></span>|<span data-ttu-id="29e6c-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29e6c-154">String</span></span>|<span data-ttu-id="29e6c-155">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="29e6c-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="29e6c-156">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="29e6c-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="29e6c-157">status</span><span class="sxs-lookup"><span data-stu-id="29e6c-157">status</span></span>|[<span data-ttu-id="29e6c-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="29e6c-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="29e6c-159">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="29e6c-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="29e6c-160">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="29e6c-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="29e6c-161">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="29e6c-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="29e6c-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="29e6c-162">errorCode</span></span>|[<span data-ttu-id="29e6c-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="29e6c-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="29e6c-164">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="29e6c-164">Error code if any occured.</span></span> <span data-ttu-id="29e6c-165">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="29e6c-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="29e6c-166">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="29e6c-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="29e6c-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="29e6c-167">guidedDeploymentTags</span></span>|<span data-ttu-id="29e6c-168">String collection</span><span class="sxs-lookup"><span data-stu-id="29e6c-168">String collection</span></span>|<span data-ttu-id="29e6c-169">Marcas da implantação dirigida herdadas de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="29e6c-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="29e6c-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="29e6c-170">Response</span></span>
<span data-ttu-id="29e6c-171">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29e6c-171">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29e6c-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29e6c-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="29e6c-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29e6c-173">Request</span></span>
<span data-ttu-id="29e6c-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29e6c-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="29e6c-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="29e6c-175">Response</span></span>
<span data-ttu-id="29e6c-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29e6c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





