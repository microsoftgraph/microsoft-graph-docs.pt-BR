---
title: Atualizar deviceManagementScriptPolicySetItem
description: Atualize as propriedades de um objeto deviceManagementScriptPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f5deb63a7a6a0132ae3ae7cd9402d03cab2ee47d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148677"
---
# <a name="update-devicemanagementscriptpolicysetitem"></a><span data-ttu-id="0dbcc-103">Atualizar deviceManagementScriptPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="0dbcc-103">Update deviceManagementScriptPolicySetItem</span></span>

<span data-ttu-id="0dbcc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dbcc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0dbcc-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0dbcc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0dbcc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0dbcc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dbcc-107">Atualize as propriedades de [um objeto deviceManagementScriptPolicySetItem.](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0dbcc-107">Update the properties of a [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0dbcc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0dbcc-108">Prerequisites</span></span>
<span data-ttu-id="0dbcc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0dbcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0dbcc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0dbcc-111">Permission type</span></span>|<span data-ttu-id="0dbcc-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0dbcc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0dbcc-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0dbcc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0dbcc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dbcc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0dbcc-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0dbcc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0dbcc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0dbcc-116">Not supported.</span></span>|
|<span data-ttu-id="0dbcc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0dbcc-117">Application</span></span>|<span data-ttu-id="0dbcc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dbcc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0dbcc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0dbcc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="0dbcc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0dbcc-120">Request headers</span></span>
|<span data-ttu-id="0dbcc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0dbcc-121">Header</span></span>|<span data-ttu-id="0dbcc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0dbcc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0dbcc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0dbcc-123">Authorization</span></span>|<span data-ttu-id="0dbcc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0dbcc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0dbcc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0dbcc-125">Accept</span></span>|<span data-ttu-id="0dbcc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0dbcc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0dbcc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0dbcc-127">Request body</span></span>
<span data-ttu-id="0dbcc-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementScriptPolicySetItem.](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0dbcc-128">In the request body, supply a JSON representation for the [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) object.</span></span>

<span data-ttu-id="0dbcc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="0dbcc-129">The following table shows the properties that are required when you create the [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md).</span></span>

|<span data-ttu-id="0dbcc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0dbcc-130">Property</span></span>|<span data-ttu-id="0dbcc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0dbcc-131">Type</span></span>|<span data-ttu-id="0dbcc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0dbcc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dbcc-133">id</span><span class="sxs-lookup"><span data-stu-id="0dbcc-133">id</span></span>|<span data-ttu-id="0dbcc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0dbcc-134">String</span></span>|<span data-ttu-id="0dbcc-135">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="0dbcc-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="0dbcc-136">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0dbcc-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="0dbcc-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0dbcc-137">createdDateTime</span></span>|<span data-ttu-id="0dbcc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0dbcc-138">DateTimeOffset</span></span>|<span data-ttu-id="0dbcc-139">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="0dbcc-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="0dbcc-140">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0dbcc-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="0dbcc-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0dbcc-141">lastModifiedDateTime</span></span>|<span data-ttu-id="0dbcc-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0dbcc-142">DateTimeOffset</span></span>|<span data-ttu-id="0dbcc-143">Última hora modificada do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="0dbcc-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="0dbcc-144">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0dbcc-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="0dbcc-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="0dbcc-145">payloadId</span></span>|<span data-ttu-id="0dbcc-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0dbcc-146">String</span></span>|<span data-ttu-id="0dbcc-147">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="0dbcc-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="0dbcc-148">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0dbcc-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="0dbcc-149">itemType</span><span class="sxs-lookup"><span data-stu-id="0dbcc-149">itemType</span></span>|<span data-ttu-id="0dbcc-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0dbcc-150">String</span></span>|<span data-ttu-id="0dbcc-151">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="0dbcc-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="0dbcc-152">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0dbcc-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="0dbcc-153">displayName</span><span class="sxs-lookup"><span data-stu-id="0dbcc-153">displayName</span></span>|<span data-ttu-id="0dbcc-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0dbcc-154">String</span></span>|<span data-ttu-id="0dbcc-155">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="0dbcc-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="0dbcc-156">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0dbcc-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="0dbcc-157">status</span><span class="sxs-lookup"><span data-stu-id="0dbcc-157">status</span></span>|[<span data-ttu-id="0dbcc-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="0dbcc-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="0dbcc-159">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="0dbcc-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="0dbcc-160">Herdado [de policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="0dbcc-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="0dbcc-161">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="0dbcc-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="0dbcc-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="0dbcc-162">errorCode</span></span>|[<span data-ttu-id="0dbcc-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="0dbcc-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="0dbcc-164">Código de erro se ocorrer algum.</span><span class="sxs-lookup"><span data-stu-id="0dbcc-164">Error code if any occured.</span></span> <span data-ttu-id="0dbcc-165">Herdado [de policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="0dbcc-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="0dbcc-166">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="0dbcc-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="0dbcc-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="0dbcc-167">guidedDeploymentTags</span></span>|<span data-ttu-id="0dbcc-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0dbcc-168">String collection</span></span>|<span data-ttu-id="0dbcc-169">Marcas da implantação guiada Herdadas [de policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0dbcc-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0dbcc-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="0dbcc-170">Response</span></span>
<span data-ttu-id="0dbcc-171">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0dbcc-171">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0dbcc-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0dbcc-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="0dbcc-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0dbcc-173">Request</span></span>
<span data-ttu-id="0dbcc-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0dbcc-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
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

### <a name="response"></a><span data-ttu-id="0dbcc-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="0dbcc-175">Response</span></span>
<span data-ttu-id="0dbcc-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0dbcc-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




