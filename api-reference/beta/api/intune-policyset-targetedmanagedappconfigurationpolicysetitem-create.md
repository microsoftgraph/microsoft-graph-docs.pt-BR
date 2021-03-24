---
title: Criar targetedManagedAppConfigurationPolicySetItem
description: Crie um novo objeto targetedManagedAppConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5e4ef91911c915545440d703e6b08aeea4abb132
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148537"
---
# <a name="create-targetedmanagedappconfigurationpolicysetitem"></a><span data-ttu-id="3b206-103">Criar targetedManagedAppConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="3b206-103">Create targetedManagedAppConfigurationPolicySetItem</span></span>

<span data-ttu-id="3b206-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b206-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b206-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3b206-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b206-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b206-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b206-107">Crie um novo [objeto targetedManagedAppConfigurationPolicySetItem.](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3b206-107">Create a new [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b206-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b206-108">Prerequisites</span></span>
<span data-ttu-id="3b206-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b206-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b206-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b206-111">Permission type</span></span>|<span data-ttu-id="3b206-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b206-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b206-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b206-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b206-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b206-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3b206-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b206-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b206-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b206-116">Not supported.</span></span>|
|<span data-ttu-id="3b206-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b206-117">Application</span></span>|<span data-ttu-id="3b206-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b206-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b206-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b206-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="3b206-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b206-120">Request headers</span></span>
|<span data-ttu-id="3b206-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b206-121">Header</span></span>|<span data-ttu-id="3b206-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3b206-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b206-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b206-123">Authorization</span></span>|<span data-ttu-id="3b206-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b206-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b206-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3b206-125">Accept</span></span>|<span data-ttu-id="3b206-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b206-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b206-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b206-127">Request body</span></span>
<span data-ttu-id="3b206-128">No corpo da solicitação, fornece uma representação JSON para o objeto targetedManagedAppConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="3b206-128">In the request body, supply a JSON representation for the targetedManagedAppConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="3b206-129">A tabela a seguir mostra as propriedades que são necessárias ao criar targetedManagedAppConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="3b206-129">The following table shows the properties that are required when you create the targetedManagedAppConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="3b206-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b206-130">Property</span></span>|<span data-ttu-id="3b206-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b206-131">Type</span></span>|<span data-ttu-id="3b206-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b206-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b206-133">id</span><span class="sxs-lookup"><span data-stu-id="3b206-133">id</span></span>|<span data-ttu-id="3b206-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b206-134">String</span></span>|<span data-ttu-id="3b206-135">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="3b206-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="3b206-136">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3b206-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3b206-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b206-137">createdDateTime</span></span>|<span data-ttu-id="3b206-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b206-138">DateTimeOffset</span></span>|<span data-ttu-id="3b206-139">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="3b206-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="3b206-140">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3b206-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3b206-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b206-141">lastModifiedDateTime</span></span>|<span data-ttu-id="3b206-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b206-142">DateTimeOffset</span></span>|<span data-ttu-id="3b206-143">Última hora modificada do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="3b206-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="3b206-144">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3b206-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3b206-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="3b206-145">payloadId</span></span>|<span data-ttu-id="3b206-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b206-146">String</span></span>|<span data-ttu-id="3b206-147">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="3b206-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="3b206-148">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3b206-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3b206-149">itemType</span><span class="sxs-lookup"><span data-stu-id="3b206-149">itemType</span></span>|<span data-ttu-id="3b206-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b206-150">String</span></span>|<span data-ttu-id="3b206-151">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="3b206-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="3b206-152">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3b206-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3b206-153">displayName</span><span class="sxs-lookup"><span data-stu-id="3b206-153">displayName</span></span>|<span data-ttu-id="3b206-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b206-154">String</span></span>|<span data-ttu-id="3b206-155">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="3b206-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="3b206-156">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3b206-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3b206-157">status</span><span class="sxs-lookup"><span data-stu-id="3b206-157">status</span></span>|[<span data-ttu-id="3b206-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="3b206-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="3b206-159">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="3b206-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="3b206-160">Herdado [de policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="3b206-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="3b206-161">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="3b206-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="3b206-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="3b206-162">errorCode</span></span>|[<span data-ttu-id="3b206-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="3b206-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="3b206-164">Código de erro se ocorrer algum.</span><span class="sxs-lookup"><span data-stu-id="3b206-164">Error code if any occured.</span></span> <span data-ttu-id="3b206-165">Herdado [de policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="3b206-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="3b206-166">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="3b206-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="3b206-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="3b206-167">guidedDeploymentTags</span></span>|<span data-ttu-id="3b206-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b206-168">String collection</span></span>|<span data-ttu-id="3b206-169">Marcas da implantação guiada Herdadas [de policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3b206-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="3b206-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b206-170">Response</span></span>
<span data-ttu-id="3b206-171">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b206-171">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b206-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b206-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b206-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b206-173">Request</span></span>
<span data-ttu-id="3b206-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b206-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
Content-type: application/json
Content-length: 326

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfigurationPolicySetItem",
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

### <a name="response"></a><span data-ttu-id="3b206-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b206-175">Response</span></span>
<span data-ttu-id="3b206-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b206-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 498

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfigurationPolicySetItem",
  "id": "f86d3112-3112-f86d-1231-6df812316df8",
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




