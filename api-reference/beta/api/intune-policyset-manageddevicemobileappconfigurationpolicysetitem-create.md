---
title: Criar managedDeviceMobileAppConfigurationPolicySetItem
description: Criar um novo objeto managedDeviceMobileAppConfigurationPolicySetItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 71bd4c91727aff9c74b4f318e7df39d4be0f9890
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941082"
---
# <a name="create-manageddevicemobileappconfigurationpolicysetitem"></a><span data-ttu-id="abaf8-103">Criar managedDeviceMobileAppConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="abaf8-103">Create managedDeviceMobileAppConfigurationPolicySetItem</span></span>

> <span data-ttu-id="abaf8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="abaf8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abaf8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="abaf8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abaf8-106">Criar um novo objeto [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="abaf8-106">Create a new [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abaf8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="abaf8-107">Prerequisites</span></span>
<span data-ttu-id="abaf8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abaf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abaf8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abaf8-110">Permission type</span></span>|<span data-ttu-id="abaf8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="abaf8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abaf8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abaf8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="abaf8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abaf8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="abaf8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abaf8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abaf8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abaf8-115">Not supported.</span></span>|
|<span data-ttu-id="abaf8-116">Application</span><span class="sxs-lookup"><span data-stu-id="abaf8-116">Application</span></span>|<span data-ttu-id="abaf8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abaf8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="abaf8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abaf8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="abaf8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abaf8-119">Request headers</span></span>
|<span data-ttu-id="abaf8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="abaf8-120">Header</span></span>|<span data-ttu-id="abaf8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="abaf8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abaf8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="abaf8-122">Authorization</span></span>|<span data-ttu-id="abaf8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abaf8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abaf8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="abaf8-124">Accept</span></span>|<span data-ttu-id="abaf8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="abaf8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abaf8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abaf8-126">Request body</span></span>
<span data-ttu-id="abaf8-127">No corpo da solicitação, forneça uma representação JSON do objeto managedDeviceMobileAppConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="abaf8-127">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="abaf8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceMobileAppConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="abaf8-128">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="abaf8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abaf8-129">Property</span></span>|<span data-ttu-id="abaf8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="abaf8-130">Type</span></span>|<span data-ttu-id="abaf8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="abaf8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abaf8-132">id</span><span class="sxs-lookup"><span data-stu-id="abaf8-132">id</span></span>|<span data-ttu-id="abaf8-133">String</span><span class="sxs-lookup"><span data-stu-id="abaf8-133">String</span></span>|<span data-ttu-id="abaf8-134">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="abaf8-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="abaf8-135">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="abaf8-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="abaf8-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="abaf8-136">createdDateTime</span></span>|<span data-ttu-id="abaf8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abaf8-137">DateTimeOffset</span></span>|<span data-ttu-id="abaf8-138">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="abaf8-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="abaf8-139">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="abaf8-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="abaf8-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="abaf8-140">lastModifiedDateTime</span></span>|<span data-ttu-id="abaf8-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abaf8-141">DateTimeOffset</span></span>|<span data-ttu-id="abaf8-142">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="abaf8-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="abaf8-143">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="abaf8-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="abaf8-144">payloadId</span><span class="sxs-lookup"><span data-stu-id="abaf8-144">payloadId</span></span>|<span data-ttu-id="abaf8-145">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="abaf8-145">String</span></span>|<span data-ttu-id="abaf8-146">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="abaf8-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="abaf8-147">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="abaf8-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="abaf8-148">itemType</span><span class="sxs-lookup"><span data-stu-id="abaf8-148">itemType</span></span>|<span data-ttu-id="abaf8-149">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="abaf8-149">String</span></span>|<span data-ttu-id="abaf8-150">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="abaf8-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="abaf8-151">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="abaf8-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="abaf8-152">displayName</span><span class="sxs-lookup"><span data-stu-id="abaf8-152">displayName</span></span>|<span data-ttu-id="abaf8-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abaf8-153">String</span></span>|<span data-ttu-id="abaf8-154">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="abaf8-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="abaf8-155">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="abaf8-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="abaf8-156">status</span><span class="sxs-lookup"><span data-stu-id="abaf8-156">status</span></span>|[<span data-ttu-id="abaf8-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="abaf8-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="abaf8-158">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="abaf8-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="abaf8-159">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="abaf8-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="abaf8-160">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="abaf8-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="abaf8-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="abaf8-161">errorCode</span></span>|[<span data-ttu-id="abaf8-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="abaf8-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="abaf8-163">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="abaf8-163">Error code if any occured.</span></span> <span data-ttu-id="abaf8-164">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="abaf8-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="abaf8-165">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="abaf8-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="abaf8-166">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="abaf8-166">guidedDeploymentTags</span></span>|<span data-ttu-id="abaf8-167">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="abaf8-167">String collection</span></span>|<span data-ttu-id="abaf8-168">Marcas da implantação dirigida herdadas de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="abaf8-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="abaf8-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="abaf8-169">Response</span></span>
<span data-ttu-id="abaf8-170">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abaf8-170">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abaf8-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abaf8-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="abaf8-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abaf8-172">Request</span></span>
<span data-ttu-id="abaf8-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abaf8-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
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

### <a name="response"></a><span data-ttu-id="abaf8-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="abaf8-174">Response</span></span>
<span data-ttu-id="abaf8-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="abaf8-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





