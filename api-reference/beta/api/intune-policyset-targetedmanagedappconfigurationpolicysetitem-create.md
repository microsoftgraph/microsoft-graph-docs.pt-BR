---
title: Criar targetedManagedAppConfigurationPolicySetItem
description: Criar um novo objeto targetedManagedAppConfigurationPolicySetItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 71438a7e52f8b1fe6f316082bfa282771a182d92
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42460490"
---
# <a name="create-targetedmanagedappconfigurationpolicysetitem"></a><span data-ttu-id="00a82-103">Criar targetedManagedAppConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="00a82-103">Create targetedManagedAppConfigurationPolicySetItem</span></span>

<span data-ttu-id="00a82-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="00a82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00a82-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="00a82-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00a82-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="00a82-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00a82-107">Criar um novo objeto [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="00a82-107">Create a new [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00a82-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="00a82-108">Prerequisites</span></span>
<span data-ttu-id="00a82-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00a82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00a82-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00a82-111">Permission type</span></span>|<span data-ttu-id="00a82-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="00a82-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00a82-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00a82-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00a82-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a82-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="00a82-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00a82-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00a82-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00a82-116">Not supported.</span></span>|
|<span data-ttu-id="00a82-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00a82-117">Application</span></span>|<span data-ttu-id="00a82-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a82-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00a82-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00a82-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="00a82-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00a82-120">Request headers</span></span>
|<span data-ttu-id="00a82-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="00a82-121">Header</span></span>|<span data-ttu-id="00a82-122">Valor</span><span class="sxs-lookup"><span data-stu-id="00a82-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00a82-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="00a82-123">Authorization</span></span>|<span data-ttu-id="00a82-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00a82-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00a82-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="00a82-125">Accept</span></span>|<span data-ttu-id="00a82-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00a82-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00a82-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00a82-127">Request body</span></span>
<span data-ttu-id="00a82-128">No corpo da solicitação, forneça uma representação JSON do objeto targetedManagedAppConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="00a82-128">In the request body, supply a JSON representation for the targetedManagedAppConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="00a82-129">A tabela a seguir mostra as propriedades que são necessárias ao criar targetedManagedAppConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="00a82-129">The following table shows the properties that are required when you create the targetedManagedAppConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="00a82-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00a82-130">Property</span></span>|<span data-ttu-id="00a82-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="00a82-131">Type</span></span>|<span data-ttu-id="00a82-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="00a82-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00a82-133">id</span><span class="sxs-lookup"><span data-stu-id="00a82-133">id</span></span>|<span data-ttu-id="00a82-134">String</span><span class="sxs-lookup"><span data-stu-id="00a82-134">String</span></span>|<span data-ttu-id="00a82-135">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="00a82-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="00a82-136">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="00a82-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="00a82-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00a82-137">createdDateTime</span></span>|<span data-ttu-id="00a82-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00a82-138">DateTimeOffset</span></span>|<span data-ttu-id="00a82-139">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="00a82-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="00a82-140">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="00a82-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="00a82-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00a82-141">lastModifiedDateTime</span></span>|<span data-ttu-id="00a82-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00a82-142">DateTimeOffset</span></span>|<span data-ttu-id="00a82-143">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="00a82-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="00a82-144">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="00a82-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="00a82-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="00a82-145">payloadId</span></span>|<span data-ttu-id="00a82-146">String</span><span class="sxs-lookup"><span data-stu-id="00a82-146">String</span></span>|<span data-ttu-id="00a82-147">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="00a82-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="00a82-148">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="00a82-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="00a82-149">itemType</span><span class="sxs-lookup"><span data-stu-id="00a82-149">itemType</span></span>|<span data-ttu-id="00a82-150">String</span><span class="sxs-lookup"><span data-stu-id="00a82-150">String</span></span>|<span data-ttu-id="00a82-151">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="00a82-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="00a82-152">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="00a82-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="00a82-153">displayName</span><span class="sxs-lookup"><span data-stu-id="00a82-153">displayName</span></span>|<span data-ttu-id="00a82-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00a82-154">String</span></span>|<span data-ttu-id="00a82-155">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="00a82-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="00a82-156">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="00a82-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="00a82-157">status</span><span class="sxs-lookup"><span data-stu-id="00a82-157">status</span></span>|[<span data-ttu-id="00a82-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="00a82-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="00a82-159">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="00a82-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="00a82-160">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="00a82-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="00a82-161">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="00a82-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="00a82-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="00a82-162">errorCode</span></span>|[<span data-ttu-id="00a82-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="00a82-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="00a82-164">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="00a82-164">Error code if any occured.</span></span> <span data-ttu-id="00a82-165">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="00a82-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="00a82-166">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="00a82-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="00a82-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="00a82-167">guidedDeploymentTags</span></span>|<span data-ttu-id="00a82-168">String collection</span><span class="sxs-lookup"><span data-stu-id="00a82-168">String collection</span></span>|<span data-ttu-id="00a82-169">Marcas da implantação dirigida herdadas de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="00a82-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="00a82-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="00a82-170">Response</span></span>
<span data-ttu-id="00a82-171">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00a82-171">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00a82-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00a82-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="00a82-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00a82-173">Request</span></span>
<span data-ttu-id="00a82-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="00a82-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="00a82-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="00a82-175">Response</span></span>
<span data-ttu-id="00a82-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="00a82-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





