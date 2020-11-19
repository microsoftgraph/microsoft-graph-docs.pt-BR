---
title: Criar deviceManagementScriptPolicySetItem
description: Criar um novo objeto deviceManagementScriptPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2dfe0a88bb22160a5037fb8e202f016c34302333
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49233128"
---
# <a name="create-devicemanagementscriptpolicysetitem"></a><span data-ttu-id="d3056-103">Criar deviceManagementScriptPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="d3056-103">Create deviceManagementScriptPolicySetItem</span></span>

<span data-ttu-id="d3056-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3056-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3056-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d3056-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3056-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3056-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3056-107">Criar um novo objeto [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="d3056-107">Create a new [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3056-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3056-108">Prerequisites</span></span>
<span data-ttu-id="d3056-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3056-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3056-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3056-111">Permission type</span></span>|<span data-ttu-id="d3056-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3056-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3056-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3056-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3056-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3056-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d3056-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3056-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3056-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3056-116">Not supported.</span></span>|
|<span data-ttu-id="d3056-117">Application</span><span class="sxs-lookup"><span data-stu-id="d3056-117">Application</span></span>|<span data-ttu-id="d3056-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3056-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3056-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3056-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="d3056-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3056-120">Request headers</span></span>
|<span data-ttu-id="d3056-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3056-121">Header</span></span>|<span data-ttu-id="d3056-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d3056-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3056-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3056-123">Authorization</span></span>|<span data-ttu-id="d3056-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3056-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3056-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d3056-125">Accept</span></span>|<span data-ttu-id="d3056-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3056-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3056-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3056-127">Request body</span></span>
<span data-ttu-id="d3056-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementScriptPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="d3056-128">In the request body, supply a JSON representation for the deviceManagementScriptPolicySetItem object.</span></span>

<span data-ttu-id="d3056-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScriptPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="d3056-129">The following table shows the properties that are required when you create the deviceManagementScriptPolicySetItem.</span></span>

|<span data-ttu-id="d3056-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3056-130">Property</span></span>|<span data-ttu-id="d3056-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3056-131">Type</span></span>|<span data-ttu-id="d3056-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3056-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3056-133">id</span><span class="sxs-lookup"><span data-stu-id="d3056-133">id</span></span>|<span data-ttu-id="d3056-134">String</span><span class="sxs-lookup"><span data-stu-id="d3056-134">String</span></span>|<span data-ttu-id="d3056-135">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="d3056-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="d3056-136">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d3056-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d3056-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d3056-137">createdDateTime</span></span>|<span data-ttu-id="d3056-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3056-138">DateTimeOffset</span></span>|<span data-ttu-id="d3056-139">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="d3056-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="d3056-140">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d3056-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d3056-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3056-141">lastModifiedDateTime</span></span>|<span data-ttu-id="d3056-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3056-142">DateTimeOffset</span></span>|<span data-ttu-id="d3056-143">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="d3056-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="d3056-144">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d3056-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d3056-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="d3056-145">payloadId</span></span>|<span data-ttu-id="d3056-146">String</span><span class="sxs-lookup"><span data-stu-id="d3056-146">String</span></span>|<span data-ttu-id="d3056-147">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="d3056-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="d3056-148">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d3056-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d3056-149">itemType</span><span class="sxs-lookup"><span data-stu-id="d3056-149">itemType</span></span>|<span data-ttu-id="d3056-150">String</span><span class="sxs-lookup"><span data-stu-id="d3056-150">String</span></span>|<span data-ttu-id="d3056-151">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="d3056-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="d3056-152">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d3056-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d3056-153">displayName</span><span class="sxs-lookup"><span data-stu-id="d3056-153">displayName</span></span>|<span data-ttu-id="d3056-154">String</span><span class="sxs-lookup"><span data-stu-id="d3056-154">String</span></span>|<span data-ttu-id="d3056-155">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="d3056-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="d3056-156">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d3056-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d3056-157">status</span><span class="sxs-lookup"><span data-stu-id="d3056-157">status</span></span>|[<span data-ttu-id="d3056-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="d3056-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="d3056-159">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="d3056-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="d3056-160">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="d3056-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="d3056-161">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="d3056-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="d3056-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="d3056-162">errorCode</span></span>|[<span data-ttu-id="d3056-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="d3056-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="d3056-164">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="d3056-164">Error code if any occured.</span></span> <span data-ttu-id="d3056-165">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="d3056-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="d3056-166">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="d3056-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="d3056-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="d3056-167">guidedDeploymentTags</span></span>|<span data-ttu-id="d3056-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3056-168">String collection</span></span>|<span data-ttu-id="d3056-169">Marcas da implantação dirigida herdadas de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d3056-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d3056-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3056-170">Response</span></span>
<span data-ttu-id="d3056-171">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3056-171">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3056-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3056-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3056-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3056-173">Request</span></span>
<span data-ttu-id="d3056-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3056-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
Content-type: application/json
Content-length: 317

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptPolicySetItem",
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

### <a name="response"></a><span data-ttu-id="d3056-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3056-175">Response</span></span>
<span data-ttu-id="d3056-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3056-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptPolicySetItem",
  "id": "b6b82c18-2c18-b6b8-182c-b8b6182cb8b6",
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




