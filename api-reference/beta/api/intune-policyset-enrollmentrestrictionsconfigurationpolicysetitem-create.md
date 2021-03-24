---
title: Criar enrollmentRestrictionsConfigurationPolicySetItem
description: Crie um novo objeto enrollmentRestrictionsConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cf64846d9e80fce3b8300386ce0ce1bdc2085949
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148628"
---
# <a name="create-enrollmentrestrictionsconfigurationpolicysetitem"></a><span data-ttu-id="1f5b9-103">Criar enrollmentRestrictionsConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="1f5b9-103">Create enrollmentRestrictionsConfigurationPolicySetItem</span></span>

<span data-ttu-id="1f5b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f5b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f5b9-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f5b9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f5b9-107">Crie um novo [objeto enrollmentRestrictionsConfigurationPolicySetItem.](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1f5b9-107">Create a new [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f5b9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1f5b9-108">Prerequisites</span></span>
<span data-ttu-id="1f5b9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f5b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f5b9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f5b9-111">Permission type</span></span>|<span data-ttu-id="1f5b9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f5b9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f5b9-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f5b9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f5b9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f5b9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1f5b9-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f5b9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f5b9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-116">Not supported.</span></span>|
|<span data-ttu-id="1f5b9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f5b9-117">Application</span></span>|<span data-ttu-id="1f5b9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f5b9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f5b9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f5b9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="1f5b9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f5b9-120">Request headers</span></span>
|<span data-ttu-id="1f5b9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1f5b9-121">Header</span></span>|<span data-ttu-id="1f5b9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1f5b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f5b9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f5b9-123">Authorization</span></span>|<span data-ttu-id="1f5b9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f5b9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1f5b9-125">Accept</span></span>|<span data-ttu-id="1f5b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1f5b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f5b9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f5b9-127">Request body</span></span>
<span data-ttu-id="1f5b9-128">No corpo da solicitação, fornece uma representação JSON para o objeto enrollmentRestrictionsConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-128">In the request body, supply a JSON representation for the enrollmentRestrictionsConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="1f5b9-129">A tabela a seguir mostra as propriedades que são necessárias ao criar enrollmentRestrictionsConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-129">The following table shows the properties that are required when you create the enrollmentRestrictionsConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="1f5b9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f5b9-130">Property</span></span>|<span data-ttu-id="1f5b9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f5b9-131">Type</span></span>|<span data-ttu-id="1f5b9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f5b9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f5b9-133">id</span><span class="sxs-lookup"><span data-stu-id="1f5b9-133">id</span></span>|<span data-ttu-id="1f5b9-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f5b9-134">String</span></span>|<span data-ttu-id="1f5b9-135">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="1f5b9-136">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1f5b9-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1f5b9-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f5b9-137">createdDateTime</span></span>|<span data-ttu-id="1f5b9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f5b9-138">DateTimeOffset</span></span>|<span data-ttu-id="1f5b9-139">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="1f5b9-140">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1f5b9-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1f5b9-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f5b9-141">lastModifiedDateTime</span></span>|<span data-ttu-id="1f5b9-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f5b9-142">DateTimeOffset</span></span>|<span data-ttu-id="1f5b9-143">Última hora modificada do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="1f5b9-144">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1f5b9-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1f5b9-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="1f5b9-145">payloadId</span></span>|<span data-ttu-id="1f5b9-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f5b9-146">String</span></span>|<span data-ttu-id="1f5b9-147">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="1f5b9-148">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1f5b9-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1f5b9-149">itemType</span><span class="sxs-lookup"><span data-stu-id="1f5b9-149">itemType</span></span>|<span data-ttu-id="1f5b9-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f5b9-150">String</span></span>|<span data-ttu-id="1f5b9-151">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="1f5b9-152">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1f5b9-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1f5b9-153">displayName</span><span class="sxs-lookup"><span data-stu-id="1f5b9-153">displayName</span></span>|<span data-ttu-id="1f5b9-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f5b9-154">String</span></span>|<span data-ttu-id="1f5b9-155">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="1f5b9-156">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1f5b9-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1f5b9-157">status</span><span class="sxs-lookup"><span data-stu-id="1f5b9-157">status</span></span>|[<span data-ttu-id="1f5b9-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="1f5b9-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="1f5b9-159">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="1f5b9-160">Herdado [de policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="1f5b9-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="1f5b9-161">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="1f5b9-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="1f5b9-162">errorCode</span></span>|[<span data-ttu-id="1f5b9-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="1f5b9-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="1f5b9-164">Código de erro se ocorrer algum.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-164">Error code if any occured.</span></span> <span data-ttu-id="1f5b9-165">Herdado [de policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="1f5b9-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="1f5b9-166">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="1f5b9-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="1f5b9-167">guidedDeploymentTags</span></span>|<span data-ttu-id="1f5b9-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f5b9-168">String collection</span></span>|<span data-ttu-id="1f5b9-169">Marcas da implantação guiada Herdadas [de policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1f5b9-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1f5b9-170">prioridade</span><span class="sxs-lookup"><span data-stu-id="1f5b9-170">priority</span></span>|<span data-ttu-id="1f5b9-171">Int32</span><span class="sxs-lookup"><span data-stu-id="1f5b9-171">Int32</span></span>|<span data-ttu-id="1f5b9-172">Prioridade do EnrollmentRestrictionsConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-172">Priority of the EnrollmentRestrictionsConfigurationPolicySetItem.</span></span>|
|<span data-ttu-id="1f5b9-173">limite</span><span class="sxs-lookup"><span data-stu-id="1f5b9-173">limit</span></span>|<span data-ttu-id="1f5b9-174">Int32</span><span class="sxs-lookup"><span data-stu-id="1f5b9-174">Int32</span></span>|<span data-ttu-id="1f5b9-175">Limite do EnrollmentRestrictionsConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-175">Limit of the EnrollmentRestrictionsConfigurationPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="1f5b9-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f5b9-176">Response</span></span>
<span data-ttu-id="1f5b9-177">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-177">If successful, this method returns a `201 Created` response code and a [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f5b9-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f5b9-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f5b9-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f5b9-179">Request</span></span>
<span data-ttu-id="1f5b9-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
Content-type: application/json
Content-length: 363

{
  "@odata.type": "#microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "priority": 8,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="1f5b9-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f5b9-181">Response</span></span>
<span data-ttu-id="1f5b9-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f5b9-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 535

{
  "@odata.type": "#microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem",
  "id": "08c4f0b1-f0b1-08c4-b1f0-c408b1f0c408",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "priority": 8,
  "limit": 5
}
```




