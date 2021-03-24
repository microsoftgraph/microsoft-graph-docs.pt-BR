---
title: Criar managedDeviceMobileAppConfigurationPolicySetItem
description: Crie um novo objeto managedDeviceMobileAppConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d957acf8e738f4b1ab470cecf9d9b753c56a226e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141726"
---
# <a name="create-manageddevicemobileappconfigurationpolicysetitem"></a><span data-ttu-id="278ce-103">Criar managedDeviceMobileAppConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="278ce-103">Create managedDeviceMobileAppConfigurationPolicySetItem</span></span>

<span data-ttu-id="278ce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="278ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="278ce-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="278ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="278ce-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="278ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="278ce-107">Crie um novo [objeto managedDeviceMobileAppConfigurationPolicySetItem.](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="278ce-107">Create a new [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="278ce-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="278ce-108">Prerequisites</span></span>
<span data-ttu-id="278ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="278ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="278ce-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="278ce-111">Permission type</span></span>|<span data-ttu-id="278ce-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="278ce-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="278ce-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="278ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="278ce-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="278ce-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="278ce-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="278ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="278ce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="278ce-116">Not supported.</span></span>|
|<span data-ttu-id="278ce-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="278ce-117">Application</span></span>|<span data-ttu-id="278ce-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="278ce-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="278ce-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="278ce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="278ce-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="278ce-120">Request headers</span></span>
|<span data-ttu-id="278ce-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="278ce-121">Header</span></span>|<span data-ttu-id="278ce-122">Valor</span><span class="sxs-lookup"><span data-stu-id="278ce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="278ce-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="278ce-123">Authorization</span></span>|<span data-ttu-id="278ce-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="278ce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="278ce-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="278ce-125">Accept</span></span>|<span data-ttu-id="278ce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="278ce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="278ce-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="278ce-127">Request body</span></span>
<span data-ttu-id="278ce-128">No corpo da solicitação, fornece uma representação JSON para o objeto managedDeviceMobileAppConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="278ce-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="278ce-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceMobileAppConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="278ce-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="278ce-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="278ce-130">Property</span></span>|<span data-ttu-id="278ce-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="278ce-131">Type</span></span>|<span data-ttu-id="278ce-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="278ce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="278ce-133">id</span><span class="sxs-lookup"><span data-stu-id="278ce-133">id</span></span>|<span data-ttu-id="278ce-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="278ce-134">String</span></span>|<span data-ttu-id="278ce-135">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="278ce-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="278ce-136">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="278ce-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="278ce-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="278ce-137">createdDateTime</span></span>|<span data-ttu-id="278ce-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="278ce-138">DateTimeOffset</span></span>|<span data-ttu-id="278ce-139">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="278ce-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="278ce-140">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="278ce-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="278ce-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="278ce-141">lastModifiedDateTime</span></span>|<span data-ttu-id="278ce-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="278ce-142">DateTimeOffset</span></span>|<span data-ttu-id="278ce-143">Última hora modificada do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="278ce-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="278ce-144">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="278ce-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="278ce-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="278ce-145">payloadId</span></span>|<span data-ttu-id="278ce-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="278ce-146">String</span></span>|<span data-ttu-id="278ce-147">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="278ce-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="278ce-148">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="278ce-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="278ce-149">itemType</span><span class="sxs-lookup"><span data-stu-id="278ce-149">itemType</span></span>|<span data-ttu-id="278ce-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="278ce-150">String</span></span>|<span data-ttu-id="278ce-151">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="278ce-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="278ce-152">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="278ce-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="278ce-153">displayName</span><span class="sxs-lookup"><span data-stu-id="278ce-153">displayName</span></span>|<span data-ttu-id="278ce-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="278ce-154">String</span></span>|<span data-ttu-id="278ce-155">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="278ce-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="278ce-156">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="278ce-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="278ce-157">status</span><span class="sxs-lookup"><span data-stu-id="278ce-157">status</span></span>|[<span data-ttu-id="278ce-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="278ce-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="278ce-159">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="278ce-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="278ce-160">Herdado [de policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="278ce-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="278ce-161">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="278ce-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="278ce-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="278ce-162">errorCode</span></span>|[<span data-ttu-id="278ce-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="278ce-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="278ce-164">Código de erro se ocorrer algum.</span><span class="sxs-lookup"><span data-stu-id="278ce-164">Error code if any occured.</span></span> <span data-ttu-id="278ce-165">Herdado [de policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="278ce-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="278ce-166">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="278ce-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="278ce-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="278ce-167">guidedDeploymentTags</span></span>|<span data-ttu-id="278ce-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="278ce-168">String collection</span></span>|<span data-ttu-id="278ce-169">Marcas da implantação guiada Herdadas [de policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="278ce-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="278ce-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="278ce-170">Response</span></span>
<span data-ttu-id="278ce-171">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="278ce-171">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="278ce-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="278ce-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="278ce-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="278ce-173">Request</span></span>
<span data-ttu-id="278ce-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="278ce-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="278ce-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="278ce-175">Response</span></span>
<span data-ttu-id="278ce-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="278ce-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




