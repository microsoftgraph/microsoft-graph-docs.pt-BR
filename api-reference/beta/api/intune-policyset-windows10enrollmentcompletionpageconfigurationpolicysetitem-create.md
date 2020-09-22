---
title: Criar windows10EnrollmentCompletionPageConfigurationPolicySetItem
description: Criar um novo objeto windows10EnrollmentCompletionPageConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 078a1d677a7ccaa29877c0a8a83ba1792e1ebd77
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972046"
---
# <a name="create-windows10enrollmentcompletionpageconfigurationpolicysetitem"></a><span data-ttu-id="fea34-103">Criar windows10EnrollmentCompletionPageConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="fea34-103">Create windows10EnrollmentCompletionPageConfigurationPolicySetItem</span></span>

<span data-ttu-id="fea34-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fea34-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fea34-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fea34-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fea34-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fea34-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fea34-107">Criar um novo objeto [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="fea34-107">Create a new [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fea34-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fea34-108">Prerequisites</span></span>
<span data-ttu-id="fea34-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fea34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fea34-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fea34-111">Permission type</span></span>|<span data-ttu-id="fea34-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fea34-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fea34-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fea34-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fea34-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fea34-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fea34-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fea34-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fea34-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fea34-116">Not supported.</span></span>|
|<span data-ttu-id="fea34-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fea34-117">Application</span></span>|<span data-ttu-id="fea34-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fea34-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fea34-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fea34-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="fea34-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fea34-120">Request headers</span></span>
|<span data-ttu-id="fea34-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fea34-121">Header</span></span>|<span data-ttu-id="fea34-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fea34-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fea34-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fea34-123">Authorization</span></span>|<span data-ttu-id="fea34-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fea34-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fea34-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fea34-125">Accept</span></span>|<span data-ttu-id="fea34-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fea34-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fea34-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fea34-127">Request body</span></span>
<span data-ttu-id="fea34-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="fea34-128">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="fea34-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="fea34-129">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="fea34-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fea34-130">Property</span></span>|<span data-ttu-id="fea34-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fea34-131">Type</span></span>|<span data-ttu-id="fea34-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fea34-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fea34-133">id</span><span class="sxs-lookup"><span data-stu-id="fea34-133">id</span></span>|<span data-ttu-id="fea34-134">String</span><span class="sxs-lookup"><span data-stu-id="fea34-134">String</span></span>|<span data-ttu-id="fea34-135">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="fea34-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="fea34-136">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="fea34-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="fea34-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fea34-137">createdDateTime</span></span>|<span data-ttu-id="fea34-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fea34-138">DateTimeOffset</span></span>|<span data-ttu-id="fea34-139">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="fea34-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="fea34-140">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="fea34-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="fea34-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fea34-141">lastModifiedDateTime</span></span>|<span data-ttu-id="fea34-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fea34-142">DateTimeOffset</span></span>|<span data-ttu-id="fea34-143">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="fea34-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="fea34-144">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="fea34-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="fea34-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="fea34-145">payloadId</span></span>|<span data-ttu-id="fea34-146">String</span><span class="sxs-lookup"><span data-stu-id="fea34-146">String</span></span>|<span data-ttu-id="fea34-147">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="fea34-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="fea34-148">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="fea34-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="fea34-149">itemType</span><span class="sxs-lookup"><span data-stu-id="fea34-149">itemType</span></span>|<span data-ttu-id="fea34-150">String</span><span class="sxs-lookup"><span data-stu-id="fea34-150">String</span></span>|<span data-ttu-id="fea34-151">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="fea34-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="fea34-152">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="fea34-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="fea34-153">displayName</span><span class="sxs-lookup"><span data-stu-id="fea34-153">displayName</span></span>|<span data-ttu-id="fea34-154">String</span><span class="sxs-lookup"><span data-stu-id="fea34-154">String</span></span>|<span data-ttu-id="fea34-155">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="fea34-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="fea34-156">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="fea34-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="fea34-157">status</span><span class="sxs-lookup"><span data-stu-id="fea34-157">status</span></span>|[<span data-ttu-id="fea34-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="fea34-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="fea34-159">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="fea34-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="fea34-160">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="fea34-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="fea34-161">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="fea34-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="fea34-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="fea34-162">errorCode</span></span>|[<span data-ttu-id="fea34-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="fea34-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="fea34-164">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="fea34-164">Error code if any occured.</span></span> <span data-ttu-id="fea34-165">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="fea34-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="fea34-166">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="fea34-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="fea34-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="fea34-167">guidedDeploymentTags</span></span>|<span data-ttu-id="fea34-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fea34-168">String collection</span></span>|<span data-ttu-id="fea34-169">Marcas da implantação dirigida herdadas de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="fea34-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="fea34-170">prioridade</span><span class="sxs-lookup"><span data-stu-id="fea34-170">priority</span></span>|<span data-ttu-id="fea34-171">Int32</span><span class="sxs-lookup"><span data-stu-id="fea34-171">Int32</span></span>|<span data-ttu-id="fea34-172">Prioridade do Windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="fea34-172">Priority of the Windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="fea34-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="fea34-173">Response</span></span>
<span data-ttu-id="fea34-174">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fea34-174">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fea34-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fea34-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="fea34-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fea34-176">Request</span></span>
<span data-ttu-id="fea34-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fea34-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fea34-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="fea34-178">Response</span></span>
<span data-ttu-id="fea34-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fea34-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






