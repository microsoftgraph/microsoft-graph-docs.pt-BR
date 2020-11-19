---
title: Criar windows10EnrollmentCompletionPageConfigurationPolicySetItem
description: Criar um novo objeto windows10EnrollmentCompletionPageConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e5bfe5a7df54d5c626f4f5c209e82a4d3b493abc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49211009"
---
# <a name="create-windows10enrollmentcompletionpageconfigurationpolicysetitem"></a><span data-ttu-id="28694-103">Criar windows10EnrollmentCompletionPageConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="28694-103">Create windows10EnrollmentCompletionPageConfigurationPolicySetItem</span></span>

<span data-ttu-id="28694-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28694-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28694-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="28694-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28694-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="28694-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28694-107">Criar um novo objeto [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="28694-107">Create a new [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28694-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="28694-108">Prerequisites</span></span>
<span data-ttu-id="28694-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28694-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28694-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28694-111">Permission type</span></span>|<span data-ttu-id="28694-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="28694-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28694-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28694-113">Delegated (work or school account)</span></span>|<span data-ttu-id="28694-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28694-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="28694-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28694-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28694-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28694-116">Not supported.</span></span>|
|<span data-ttu-id="28694-117">Application</span><span class="sxs-lookup"><span data-stu-id="28694-117">Application</span></span>|<span data-ttu-id="28694-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28694-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28694-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28694-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="28694-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28694-120">Request headers</span></span>
|<span data-ttu-id="28694-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="28694-121">Header</span></span>|<span data-ttu-id="28694-122">Valor</span><span class="sxs-lookup"><span data-stu-id="28694-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28694-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="28694-123">Authorization</span></span>|<span data-ttu-id="28694-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28694-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28694-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="28694-125">Accept</span></span>|<span data-ttu-id="28694-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28694-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28694-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28694-127">Request body</span></span>
<span data-ttu-id="28694-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="28694-128">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="28694-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="28694-129">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="28694-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28694-130">Property</span></span>|<span data-ttu-id="28694-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="28694-131">Type</span></span>|<span data-ttu-id="28694-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="28694-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28694-133">id</span><span class="sxs-lookup"><span data-stu-id="28694-133">id</span></span>|<span data-ttu-id="28694-134">String</span><span class="sxs-lookup"><span data-stu-id="28694-134">String</span></span>|<span data-ttu-id="28694-135">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="28694-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="28694-136">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="28694-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="28694-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="28694-137">createdDateTime</span></span>|<span data-ttu-id="28694-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28694-138">DateTimeOffset</span></span>|<span data-ttu-id="28694-139">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="28694-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="28694-140">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="28694-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="28694-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="28694-141">lastModifiedDateTime</span></span>|<span data-ttu-id="28694-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28694-142">DateTimeOffset</span></span>|<span data-ttu-id="28694-143">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="28694-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="28694-144">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="28694-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="28694-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="28694-145">payloadId</span></span>|<span data-ttu-id="28694-146">String</span><span class="sxs-lookup"><span data-stu-id="28694-146">String</span></span>|<span data-ttu-id="28694-147">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="28694-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="28694-148">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="28694-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="28694-149">itemType</span><span class="sxs-lookup"><span data-stu-id="28694-149">itemType</span></span>|<span data-ttu-id="28694-150">String</span><span class="sxs-lookup"><span data-stu-id="28694-150">String</span></span>|<span data-ttu-id="28694-151">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="28694-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="28694-152">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="28694-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="28694-153">displayName</span><span class="sxs-lookup"><span data-stu-id="28694-153">displayName</span></span>|<span data-ttu-id="28694-154">String</span><span class="sxs-lookup"><span data-stu-id="28694-154">String</span></span>|<span data-ttu-id="28694-155">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="28694-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="28694-156">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="28694-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="28694-157">status</span><span class="sxs-lookup"><span data-stu-id="28694-157">status</span></span>|[<span data-ttu-id="28694-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="28694-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="28694-159">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="28694-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="28694-160">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="28694-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="28694-161">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="28694-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="28694-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="28694-162">errorCode</span></span>|[<span data-ttu-id="28694-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="28694-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="28694-164">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="28694-164">Error code if any occured.</span></span> <span data-ttu-id="28694-165">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="28694-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="28694-166">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="28694-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="28694-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="28694-167">guidedDeploymentTags</span></span>|<span data-ttu-id="28694-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="28694-168">String collection</span></span>|<span data-ttu-id="28694-169">Marcas da implantação dirigida herdadas de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="28694-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="28694-170">prioridade</span><span class="sxs-lookup"><span data-stu-id="28694-170">priority</span></span>|<span data-ttu-id="28694-171">Int32</span><span class="sxs-lookup"><span data-stu-id="28694-171">Int32</span></span>|<span data-ttu-id="28694-172">Prioridade do Windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="28694-172">Priority of the Windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="28694-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="28694-173">Response</span></span>
<span data-ttu-id="28694-174">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28694-174">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28694-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28694-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="28694-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28694-176">Request</span></span>
<span data-ttu-id="28694-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28694-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
Content-type: application/json
Content-length: 359

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfigurationPolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="28694-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="28694-178">Response</span></span>
<span data-ttu-id="28694-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="28694-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 531

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfigurationPolicySetItem",
  "id": "ebfb1dbb-1dbb-ebfb-bb1d-fbebbb1dfbeb",
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
  "priority": 8
}
```




