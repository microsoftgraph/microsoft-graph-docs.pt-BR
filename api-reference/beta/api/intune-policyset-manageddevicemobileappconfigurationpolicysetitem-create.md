---
title: Criar managedDeviceMobileAppConfigurationPolicySetItem
description: Criar um novo objeto managedDeviceMobileAppConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 62279a04bb08ee542f65095497455f4e53c65693
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49211163"
---
# <a name="create-manageddevicemobileappconfigurationpolicysetitem"></a><span data-ttu-id="d7ef1-103">Criar managedDeviceMobileAppConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="d7ef1-103">Create managedDeviceMobileAppConfigurationPolicySetItem</span></span>

<span data-ttu-id="d7ef1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7ef1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7ef1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d7ef1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7ef1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d7ef1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7ef1-107">Criar um novo objeto [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="d7ef1-107">Create a new [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7ef1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d7ef1-108">Prerequisites</span></span>
<span data-ttu-id="d7ef1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7ef1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7ef1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7ef1-111">Permission type</span></span>|<span data-ttu-id="d7ef1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d7ef1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7ef1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7ef1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d7ef1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7ef1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7ef1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7ef1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7ef1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7ef1-116">Not supported.</span></span>|
|<span data-ttu-id="d7ef1-117">Application</span><span class="sxs-lookup"><span data-stu-id="d7ef1-117">Application</span></span>|<span data-ttu-id="d7ef1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7ef1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7ef1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7ef1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="d7ef1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7ef1-120">Request headers</span></span>
|<span data-ttu-id="d7ef1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d7ef1-121">Header</span></span>|<span data-ttu-id="d7ef1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d7ef1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7ef1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7ef1-123">Authorization</span></span>|<span data-ttu-id="d7ef1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7ef1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7ef1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d7ef1-125">Accept</span></span>|<span data-ttu-id="d7ef1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d7ef1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7ef1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7ef1-127">Request body</span></span>
<span data-ttu-id="d7ef1-128">No corpo da solicitação, forneça uma representação JSON do objeto managedDeviceMobileAppConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="d7ef1-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="d7ef1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceMobileAppConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="d7ef1-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="d7ef1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7ef1-130">Property</span></span>|<span data-ttu-id="d7ef1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7ef1-131">Type</span></span>|<span data-ttu-id="d7ef1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7ef1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7ef1-133">id</span><span class="sxs-lookup"><span data-stu-id="d7ef1-133">id</span></span>|<span data-ttu-id="d7ef1-134">String</span><span class="sxs-lookup"><span data-stu-id="d7ef1-134">String</span></span>|<span data-ttu-id="d7ef1-135">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="d7ef1-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="d7ef1-136">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d7ef1-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d7ef1-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7ef1-137">createdDateTime</span></span>|<span data-ttu-id="d7ef1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7ef1-138">DateTimeOffset</span></span>|<span data-ttu-id="d7ef1-139">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="d7ef1-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="d7ef1-140">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d7ef1-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d7ef1-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7ef1-141">lastModifiedDateTime</span></span>|<span data-ttu-id="d7ef1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7ef1-142">DateTimeOffset</span></span>|<span data-ttu-id="d7ef1-143">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="d7ef1-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="d7ef1-144">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d7ef1-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d7ef1-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="d7ef1-145">payloadId</span></span>|<span data-ttu-id="d7ef1-146">String</span><span class="sxs-lookup"><span data-stu-id="d7ef1-146">String</span></span>|<span data-ttu-id="d7ef1-147">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="d7ef1-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="d7ef1-148">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d7ef1-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d7ef1-149">itemType</span><span class="sxs-lookup"><span data-stu-id="d7ef1-149">itemType</span></span>|<span data-ttu-id="d7ef1-150">String</span><span class="sxs-lookup"><span data-stu-id="d7ef1-150">String</span></span>|<span data-ttu-id="d7ef1-151">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="d7ef1-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="d7ef1-152">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d7ef1-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d7ef1-153">displayName</span><span class="sxs-lookup"><span data-stu-id="d7ef1-153">displayName</span></span>|<span data-ttu-id="d7ef1-154">String</span><span class="sxs-lookup"><span data-stu-id="d7ef1-154">String</span></span>|<span data-ttu-id="d7ef1-155">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="d7ef1-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="d7ef1-156">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d7ef1-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d7ef1-157">status</span><span class="sxs-lookup"><span data-stu-id="d7ef1-157">status</span></span>|[<span data-ttu-id="d7ef1-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="d7ef1-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="d7ef1-159">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="d7ef1-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="d7ef1-160">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="d7ef1-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="d7ef1-161">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="d7ef1-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="d7ef1-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="d7ef1-162">errorCode</span></span>|[<span data-ttu-id="d7ef1-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="d7ef1-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="d7ef1-164">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="d7ef1-164">Error code if any occured.</span></span> <span data-ttu-id="d7ef1-165">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="d7ef1-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="d7ef1-166">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="d7ef1-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="d7ef1-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="d7ef1-167">guidedDeploymentTags</span></span>|<span data-ttu-id="d7ef1-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7ef1-168">String collection</span></span>|<span data-ttu-id="d7ef1-169">Marcas da implantação dirigida herdadas de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d7ef1-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d7ef1-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7ef1-170">Response</span></span>
<span data-ttu-id="d7ef1-171">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7ef1-171">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7ef1-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7ef1-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7ef1-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7ef1-173">Request</span></span>
<span data-ttu-id="d7ef1-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7ef1-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d7ef1-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7ef1-175">Response</span></span>
<span data-ttu-id="d7ef1-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7ef1-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




