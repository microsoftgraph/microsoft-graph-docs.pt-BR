---
title: Atualizar deviceCompliancePolicyPolicySetItem
description: Atualiza as propriedades de um objeto deviceCompliancePolicyPolicySetItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e8e11e8ae9b8e64b16fa83ff1b42b91a7fedc368
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42461294"
---
# <a name="update-devicecompliancepolicypolicysetitem"></a><span data-ttu-id="457df-103">Atualizar deviceCompliancePolicyPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="457df-103">Update deviceCompliancePolicyPolicySetItem</span></span>

<span data-ttu-id="457df-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="457df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="457df-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="457df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="457df-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="457df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="457df-107">Atualiza as propriedades de um objeto [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="457df-107">Update the properties of a [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="457df-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="457df-108">Prerequisites</span></span>
<span data-ttu-id="457df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="457df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="457df-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="457df-111">Permission type</span></span>|<span data-ttu-id="457df-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="457df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="457df-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="457df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="457df-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="457df-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="457df-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="457df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="457df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="457df-116">Not supported.</span></span>|
|<span data-ttu-id="457df-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="457df-117">Application</span></span>|<span data-ttu-id="457df-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="457df-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="457df-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="457df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="457df-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="457df-120">Request headers</span></span>
|<span data-ttu-id="457df-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="457df-121">Header</span></span>|<span data-ttu-id="457df-122">Valor</span><span class="sxs-lookup"><span data-stu-id="457df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="457df-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="457df-123">Authorization</span></span>|<span data-ttu-id="457df-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="457df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="457df-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="457df-125">Accept</span></span>|<span data-ttu-id="457df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="457df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="457df-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="457df-127">Request body</span></span>
<span data-ttu-id="457df-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="457df-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object.</span></span>

<span data-ttu-id="457df-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="457df-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md).</span></span>

|<span data-ttu-id="457df-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="457df-130">Property</span></span>|<span data-ttu-id="457df-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="457df-131">Type</span></span>|<span data-ttu-id="457df-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="457df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="457df-133">id</span><span class="sxs-lookup"><span data-stu-id="457df-133">id</span></span>|<span data-ttu-id="457df-134">String</span><span class="sxs-lookup"><span data-stu-id="457df-134">String</span></span>|<span data-ttu-id="457df-135">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="457df-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="457df-136">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="457df-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="457df-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="457df-137">createdDateTime</span></span>|<span data-ttu-id="457df-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="457df-138">DateTimeOffset</span></span>|<span data-ttu-id="457df-139">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="457df-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="457df-140">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="457df-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="457df-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="457df-141">lastModifiedDateTime</span></span>|<span data-ttu-id="457df-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="457df-142">DateTimeOffset</span></span>|<span data-ttu-id="457df-143">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="457df-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="457df-144">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="457df-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="457df-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="457df-145">payloadId</span></span>|<span data-ttu-id="457df-146">String</span><span class="sxs-lookup"><span data-stu-id="457df-146">String</span></span>|<span data-ttu-id="457df-147">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="457df-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="457df-148">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="457df-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="457df-149">itemType</span><span class="sxs-lookup"><span data-stu-id="457df-149">itemType</span></span>|<span data-ttu-id="457df-150">String</span><span class="sxs-lookup"><span data-stu-id="457df-150">String</span></span>|<span data-ttu-id="457df-151">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="457df-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="457df-152">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="457df-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="457df-153">displayName</span><span class="sxs-lookup"><span data-stu-id="457df-153">displayName</span></span>|<span data-ttu-id="457df-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="457df-154">String</span></span>|<span data-ttu-id="457df-155">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="457df-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="457df-156">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="457df-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="457df-157">status</span><span class="sxs-lookup"><span data-stu-id="457df-157">status</span></span>|[<span data-ttu-id="457df-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="457df-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="457df-159">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="457df-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="457df-160">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="457df-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="457df-161">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="457df-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="457df-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="457df-162">errorCode</span></span>|[<span data-ttu-id="457df-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="457df-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="457df-164">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="457df-164">Error code if any occured.</span></span> <span data-ttu-id="457df-165">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="457df-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="457df-166">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="457df-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="457df-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="457df-167">guidedDeploymentTags</span></span>|<span data-ttu-id="457df-168">String collection</span><span class="sxs-lookup"><span data-stu-id="457df-168">String collection</span></span>|<span data-ttu-id="457df-169">Marcas da implantação dirigida herdadas de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="457df-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="457df-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="457df-170">Response</span></span>
<span data-ttu-id="457df-171">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="457df-171">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="457df-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="457df-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="457df-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="457df-173">Request</span></span>
<span data-ttu-id="457df-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="457df-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 317

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyPolicySetItem",
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

### <a name="response"></a><span data-ttu-id="457df-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="457df-175">Response</span></span>
<span data-ttu-id="457df-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="457df-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyPolicySetItem",
  "id": "5c0bc827-c827-5c0b-27c8-0b5c27c80b5c",
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





