---
title: Atualizar iosLobAppProvisioningConfigurationPolicySetItem
description: Atualiza as propriedades de um objeto iosLobAppProvisioningConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9cd1889bf8429fb3fb1b5f15b57ef9ffa28f3850
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696493"
---
# <a name="update-ioslobappprovisioningconfigurationpolicysetitem"></a><span data-ttu-id="b832c-103">Atualizar iosLobAppProvisioningConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="b832c-103">Update iosLobAppProvisioningConfigurationPolicySetItem</span></span>

<span data-ttu-id="b832c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b832c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b832c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b832c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b832c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b832c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b832c-107">Atualiza as propriedades de um objeto [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="b832c-107">Update the properties of a [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b832c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b832c-108">Prerequisites</span></span>
<span data-ttu-id="b832c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b832c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b832c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b832c-111">Permission type</span></span>|<span data-ttu-id="b832c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b832c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b832c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b832c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b832c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b832c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b832c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b832c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b832c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b832c-116">Not supported.</span></span>|
|<span data-ttu-id="b832c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b832c-117">Application</span></span>|<span data-ttu-id="b832c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b832c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b832c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b832c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="b832c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b832c-120">Request headers</span></span>
|<span data-ttu-id="b832c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b832c-121">Header</span></span>|<span data-ttu-id="b832c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b832c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b832c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b832c-123">Authorization</span></span>|<span data-ttu-id="b832c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b832c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b832c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b832c-125">Accept</span></span>|<span data-ttu-id="b832c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b832c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b832c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b832c-127">Request body</span></span>
<span data-ttu-id="b832c-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="b832c-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) object.</span></span>

<span data-ttu-id="b832c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="b832c-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md).</span></span>

|<span data-ttu-id="b832c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b832c-130">Property</span></span>|<span data-ttu-id="b832c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b832c-131">Type</span></span>|<span data-ttu-id="b832c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b832c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b832c-133">id</span><span class="sxs-lookup"><span data-stu-id="b832c-133">id</span></span>|<span data-ttu-id="b832c-134">String</span><span class="sxs-lookup"><span data-stu-id="b832c-134">String</span></span>|<span data-ttu-id="b832c-135">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b832c-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="b832c-136">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b832c-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b832c-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b832c-137">createdDateTime</span></span>|<span data-ttu-id="b832c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b832c-138">DateTimeOffset</span></span>|<span data-ttu-id="b832c-139">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b832c-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="b832c-140">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b832c-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b832c-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b832c-141">lastModifiedDateTime</span></span>|<span data-ttu-id="b832c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b832c-142">DateTimeOffset</span></span>|<span data-ttu-id="b832c-143">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b832c-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="b832c-144">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b832c-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b832c-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="b832c-145">payloadId</span></span>|<span data-ttu-id="b832c-146">String</span><span class="sxs-lookup"><span data-stu-id="b832c-146">String</span></span>|<span data-ttu-id="b832c-147">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b832c-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="b832c-148">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b832c-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b832c-149">itemType</span><span class="sxs-lookup"><span data-stu-id="b832c-149">itemType</span></span>|<span data-ttu-id="b832c-150">String</span><span class="sxs-lookup"><span data-stu-id="b832c-150">String</span></span>|<span data-ttu-id="b832c-151">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b832c-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="b832c-152">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b832c-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b832c-153">displayName</span><span class="sxs-lookup"><span data-stu-id="b832c-153">displayName</span></span>|<span data-ttu-id="b832c-154">String</span><span class="sxs-lookup"><span data-stu-id="b832c-154">String</span></span>|<span data-ttu-id="b832c-155">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b832c-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="b832c-156">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b832c-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b832c-157">status</span><span class="sxs-lookup"><span data-stu-id="b832c-157">status</span></span>|[<span data-ttu-id="b832c-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="b832c-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="b832c-159">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b832c-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="b832c-160">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="b832c-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="b832c-161">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b832c-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="b832c-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="b832c-162">errorCode</span></span>|[<span data-ttu-id="b832c-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="b832c-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="b832c-164">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="b832c-164">Error code if any occured.</span></span> <span data-ttu-id="b832c-165">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="b832c-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="b832c-166">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="b832c-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="b832c-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="b832c-167">guidedDeploymentTags</span></span>|<span data-ttu-id="b832c-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b832c-168">String collection</span></span>|<span data-ttu-id="b832c-169">Marcas da implantação dirigida herdadas de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b832c-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b832c-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="b832c-170">Response</span></span>
<span data-ttu-id="b832c-171">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b832c-171">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b832c-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b832c-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="b832c-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b832c-173">Request</span></span>
<span data-ttu-id="b832c-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b832c-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b832c-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="b832c-175">Response</span></span>
<span data-ttu-id="b832c-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b832c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





