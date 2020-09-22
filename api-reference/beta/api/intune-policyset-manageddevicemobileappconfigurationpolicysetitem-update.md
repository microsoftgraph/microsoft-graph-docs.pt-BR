---
title: Atualizar managedDeviceMobileAppConfigurationPolicySetItem
description: Atualiza as propriedades de um objeto managedDeviceMobileAppConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 395b6c6ffc037b85445594349ea905ae93d2356c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064854"
---
# <a name="update-manageddevicemobileappconfigurationpolicysetitem"></a><span data-ttu-id="f6028-103">Atualizar managedDeviceMobileAppConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="f6028-103">Update managedDeviceMobileAppConfigurationPolicySetItem</span></span>

<span data-ttu-id="f6028-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6028-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6028-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f6028-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6028-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f6028-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6028-107">Atualiza as propriedades de um objeto [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="f6028-107">Update the properties of a [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6028-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f6028-108">Prerequisites</span></span>
<span data-ttu-id="f6028-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6028-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6028-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6028-111">Permission type</span></span>|<span data-ttu-id="f6028-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f6028-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6028-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6028-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6028-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6028-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f6028-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6028-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6028-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6028-116">Not supported.</span></span>|
|<span data-ttu-id="f6028-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6028-117">Application</span></span>|<span data-ttu-id="f6028-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6028-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6028-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6028-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="f6028-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6028-120">Request headers</span></span>
|<span data-ttu-id="f6028-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f6028-121">Header</span></span>|<span data-ttu-id="f6028-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f6028-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6028-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6028-123">Authorization</span></span>|<span data-ttu-id="f6028-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6028-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6028-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f6028-125">Accept</span></span>|<span data-ttu-id="f6028-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6028-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6028-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6028-127">Request body</span></span>
<span data-ttu-id="f6028-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="f6028-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) object.</span></span>

<span data-ttu-id="f6028-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="f6028-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md).</span></span>

|<span data-ttu-id="f6028-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6028-130">Property</span></span>|<span data-ttu-id="f6028-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6028-131">Type</span></span>|<span data-ttu-id="f6028-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6028-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6028-133">id</span><span class="sxs-lookup"><span data-stu-id="f6028-133">id</span></span>|<span data-ttu-id="f6028-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6028-134">String</span></span>|<span data-ttu-id="f6028-135">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="f6028-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="f6028-136">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="f6028-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="f6028-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6028-137">createdDateTime</span></span>|<span data-ttu-id="f6028-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6028-138">DateTimeOffset</span></span>|<span data-ttu-id="f6028-139">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="f6028-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="f6028-140">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="f6028-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="f6028-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6028-141">lastModifiedDateTime</span></span>|<span data-ttu-id="f6028-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6028-142">DateTimeOffset</span></span>|<span data-ttu-id="f6028-143">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="f6028-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="f6028-144">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="f6028-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="f6028-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="f6028-145">payloadId</span></span>|<span data-ttu-id="f6028-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6028-146">String</span></span>|<span data-ttu-id="f6028-147">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="f6028-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="f6028-148">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="f6028-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="f6028-149">itemType</span><span class="sxs-lookup"><span data-stu-id="f6028-149">itemType</span></span>|<span data-ttu-id="f6028-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6028-150">String</span></span>|<span data-ttu-id="f6028-151">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="f6028-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="f6028-152">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="f6028-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="f6028-153">displayName</span><span class="sxs-lookup"><span data-stu-id="f6028-153">displayName</span></span>|<span data-ttu-id="f6028-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6028-154">String</span></span>|<span data-ttu-id="f6028-155">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="f6028-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="f6028-156">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="f6028-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="f6028-157">status</span><span class="sxs-lookup"><span data-stu-id="f6028-157">status</span></span>|[<span data-ttu-id="f6028-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="f6028-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="f6028-159">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="f6028-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="f6028-160">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="f6028-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="f6028-161">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="f6028-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="f6028-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="f6028-162">errorCode</span></span>|[<span data-ttu-id="f6028-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="f6028-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="f6028-164">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="f6028-164">Error code if any occured.</span></span> <span data-ttu-id="f6028-165">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="f6028-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="f6028-166">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="f6028-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="f6028-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="f6028-167">guidedDeploymentTags</span></span>|<span data-ttu-id="f6028-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6028-168">String collection</span></span>|<span data-ttu-id="f6028-169">Marcas da implantação dirigida herdadas de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="f6028-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f6028-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6028-170">Response</span></span>
<span data-ttu-id="f6028-171">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6028-171">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6028-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6028-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6028-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6028-173">Request</span></span>
<span data-ttu-id="f6028-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6028-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 330

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationPolicySetItem",
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

### <a name="response"></a><span data-ttu-id="f6028-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6028-175">Response</span></span>
<span data-ttu-id="f6028-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f6028-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 502

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationPolicySetItem",
  "id": "bb065442-5442-bb06-4254-06bb425406bb",
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






