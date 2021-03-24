---
title: Atualizar iosLobAppProvisioningConfigurationPolicySetItem
description: Atualize as propriedades de um objeto iosLobAppProvisioningConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: da31a610291d64666fa41c2265bc60952e4c6003
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141733"
---
# <a name="update-ioslobappprovisioningconfigurationpolicysetitem"></a><span data-ttu-id="a58eb-103">Atualizar iosLobAppProvisioningConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="a58eb-103">Update iosLobAppProvisioningConfigurationPolicySetItem</span></span>

<span data-ttu-id="a58eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a58eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a58eb-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a58eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a58eb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a58eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a58eb-107">Atualize as propriedades de [um objeto iosLobAppProvisioningConfigurationPolicySetItem.](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="a58eb-107">Update the properties of a [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a58eb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a58eb-108">Prerequisites</span></span>
<span data-ttu-id="a58eb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a58eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a58eb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a58eb-111">Permission type</span></span>|<span data-ttu-id="a58eb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a58eb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a58eb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a58eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a58eb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a58eb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a58eb-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a58eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a58eb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a58eb-116">Not supported.</span></span>|
|<span data-ttu-id="a58eb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a58eb-117">Application</span></span>|<span data-ttu-id="a58eb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a58eb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a58eb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a58eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="a58eb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a58eb-120">Request headers</span></span>
|<span data-ttu-id="a58eb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a58eb-121">Header</span></span>|<span data-ttu-id="a58eb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a58eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a58eb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a58eb-123">Authorization</span></span>|<span data-ttu-id="a58eb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a58eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a58eb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a58eb-125">Accept</span></span>|<span data-ttu-id="a58eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a58eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a58eb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a58eb-127">Request body</span></span>
<span data-ttu-id="a58eb-128">No corpo da solicitação, fornece uma representação JSON para o objeto [iosLobAppProvisioningConfigurationPolicySetItem.](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="a58eb-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) object.</span></span>

<span data-ttu-id="a58eb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="a58eb-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md).</span></span>

|<span data-ttu-id="a58eb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a58eb-130">Property</span></span>|<span data-ttu-id="a58eb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a58eb-131">Type</span></span>|<span data-ttu-id="a58eb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a58eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a58eb-133">id</span><span class="sxs-lookup"><span data-stu-id="a58eb-133">id</span></span>|<span data-ttu-id="a58eb-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a58eb-134">String</span></span>|<span data-ttu-id="a58eb-135">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="a58eb-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="a58eb-136">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="a58eb-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="a58eb-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a58eb-137">createdDateTime</span></span>|<span data-ttu-id="a58eb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a58eb-138">DateTimeOffset</span></span>|<span data-ttu-id="a58eb-139">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="a58eb-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="a58eb-140">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="a58eb-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="a58eb-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a58eb-141">lastModifiedDateTime</span></span>|<span data-ttu-id="a58eb-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a58eb-142">DateTimeOffset</span></span>|<span data-ttu-id="a58eb-143">Última hora modificada do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="a58eb-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="a58eb-144">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="a58eb-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="a58eb-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="a58eb-145">payloadId</span></span>|<span data-ttu-id="a58eb-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a58eb-146">String</span></span>|<span data-ttu-id="a58eb-147">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="a58eb-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="a58eb-148">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="a58eb-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="a58eb-149">itemType</span><span class="sxs-lookup"><span data-stu-id="a58eb-149">itemType</span></span>|<span data-ttu-id="a58eb-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a58eb-150">String</span></span>|<span data-ttu-id="a58eb-151">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="a58eb-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="a58eb-152">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="a58eb-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="a58eb-153">displayName</span><span class="sxs-lookup"><span data-stu-id="a58eb-153">displayName</span></span>|<span data-ttu-id="a58eb-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a58eb-154">String</span></span>|<span data-ttu-id="a58eb-155">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="a58eb-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="a58eb-156">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="a58eb-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="a58eb-157">status</span><span class="sxs-lookup"><span data-stu-id="a58eb-157">status</span></span>|[<span data-ttu-id="a58eb-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="a58eb-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="a58eb-159">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="a58eb-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="a58eb-160">Herdado [de policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="a58eb-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="a58eb-161">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a58eb-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="a58eb-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="a58eb-162">errorCode</span></span>|[<span data-ttu-id="a58eb-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="a58eb-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="a58eb-164">Código de erro se ocorrer algum.</span><span class="sxs-lookup"><span data-stu-id="a58eb-164">Error code if any occured.</span></span> <span data-ttu-id="a58eb-165">Herdado [de policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="a58eb-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="a58eb-166">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="a58eb-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="a58eb-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="a58eb-167">guidedDeploymentTags</span></span>|<span data-ttu-id="a58eb-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a58eb-168">String collection</span></span>|<span data-ttu-id="a58eb-169">Marcas da implantação guiada Herdadas [de policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="a58eb-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a58eb-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="a58eb-170">Response</span></span>
<span data-ttu-id="a58eb-171">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a58eb-171">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a58eb-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a58eb-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="a58eb-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a58eb-173">Request</span></span>
<span data-ttu-id="a58eb-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a58eb-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 329

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationPolicySetItem",
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

### <a name="response"></a><span data-ttu-id="a58eb-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="a58eb-175">Response</span></span>
<span data-ttu-id="a58eb-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a58eb-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 501

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationPolicySetItem",
  "id": "6a978d58-8d58-6a97-588d-976a588d976a",
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




