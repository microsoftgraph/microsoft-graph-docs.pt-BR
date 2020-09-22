---
title: Criar managedAppProtectionPolicySetItem
description: Criar um novo objeto managedAppProtectionPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c509323ecc26ea1cd08d358ac64c7d6c0ad4b176
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093445"
---
# <a name="create-managedappprotectionpolicysetitem"></a><span data-ttu-id="0771f-103">Criar managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="0771f-103">Create managedAppProtectionPolicySetItem</span></span>

<span data-ttu-id="0771f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0771f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0771f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0771f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0771f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0771f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0771f-107">Criar um novo objeto [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="0771f-107">Create a new [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0771f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0771f-108">Prerequisites</span></span>
<span data-ttu-id="0771f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0771f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0771f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0771f-111">Permission type</span></span>|<span data-ttu-id="0771f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0771f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0771f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0771f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0771f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0771f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0771f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0771f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0771f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0771f-116">Not supported.</span></span>|
|<span data-ttu-id="0771f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0771f-117">Application</span></span>|<span data-ttu-id="0771f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0771f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0771f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0771f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="0771f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0771f-120">Request headers</span></span>
|<span data-ttu-id="0771f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0771f-121">Header</span></span>|<span data-ttu-id="0771f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0771f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0771f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0771f-123">Authorization</span></span>|<span data-ttu-id="0771f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0771f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0771f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0771f-125">Accept</span></span>|<span data-ttu-id="0771f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0771f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0771f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0771f-127">Request body</span></span>
<span data-ttu-id="0771f-128">No corpo da solicitação, forneça uma representação JSON do objeto managedAppProtectionPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="0771f-128">In the request body, supply a JSON representation for the managedAppProtectionPolicySetItem object.</span></span>

<span data-ttu-id="0771f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedAppProtectionPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="0771f-129">The following table shows the properties that are required when you create the managedAppProtectionPolicySetItem.</span></span>

|<span data-ttu-id="0771f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0771f-130">Property</span></span>|<span data-ttu-id="0771f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0771f-131">Type</span></span>|<span data-ttu-id="0771f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0771f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0771f-133">id</span><span class="sxs-lookup"><span data-stu-id="0771f-133">id</span></span>|<span data-ttu-id="0771f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0771f-134">String</span></span>|<span data-ttu-id="0771f-135">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="0771f-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="0771f-136">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0771f-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="0771f-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0771f-137">createdDateTime</span></span>|<span data-ttu-id="0771f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0771f-138">DateTimeOffset</span></span>|<span data-ttu-id="0771f-139">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="0771f-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="0771f-140">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0771f-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="0771f-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0771f-141">lastModifiedDateTime</span></span>|<span data-ttu-id="0771f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0771f-142">DateTimeOffset</span></span>|<span data-ttu-id="0771f-143">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="0771f-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="0771f-144">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0771f-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="0771f-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="0771f-145">payloadId</span></span>|<span data-ttu-id="0771f-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0771f-146">String</span></span>|<span data-ttu-id="0771f-147">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="0771f-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="0771f-148">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0771f-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="0771f-149">itemType</span><span class="sxs-lookup"><span data-stu-id="0771f-149">itemType</span></span>|<span data-ttu-id="0771f-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0771f-150">String</span></span>|<span data-ttu-id="0771f-151">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="0771f-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="0771f-152">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0771f-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="0771f-153">displayName</span><span class="sxs-lookup"><span data-stu-id="0771f-153">displayName</span></span>|<span data-ttu-id="0771f-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0771f-154">String</span></span>|<span data-ttu-id="0771f-155">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="0771f-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="0771f-156">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0771f-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="0771f-157">status</span><span class="sxs-lookup"><span data-stu-id="0771f-157">status</span></span>|[<span data-ttu-id="0771f-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="0771f-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="0771f-159">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="0771f-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="0771f-160">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="0771f-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="0771f-161">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="0771f-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="0771f-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="0771f-162">errorCode</span></span>|[<span data-ttu-id="0771f-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="0771f-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="0771f-164">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="0771f-164">Error code if any occured.</span></span> <span data-ttu-id="0771f-165">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="0771f-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="0771f-166">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="0771f-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="0771f-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="0771f-167">guidedDeploymentTags</span></span>|<span data-ttu-id="0771f-168">Coleção String</span><span class="sxs-lookup"><span data-stu-id="0771f-168">String collection</span></span>|<span data-ttu-id="0771f-169">Marcas da implantação dirigida herdadas de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0771f-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="0771f-170">targetedAppManagementLevels</span><span class="sxs-lookup"><span data-stu-id="0771f-170">targetedAppManagementLevels</span></span>|<span data-ttu-id="0771f-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0771f-171">String</span></span>|<span data-ttu-id="0771f-172">TargetedAppManagementLevels do ManagedAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="0771f-172">TargetedAppManagementLevels of the ManagedAppPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="0771f-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="0771f-173">Response</span></span>
<span data-ttu-id="0771f-174">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0771f-174">If successful, this method returns a `201 Created` response code and a [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0771f-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0771f-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="0771f-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0771f-176">Request</span></span>
<span data-ttu-id="0771f-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0771f-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
Content-type: application/json
Content-length: 389

{
  "@odata.type": "#microsoft.graph.managedAppProtectionPolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "targetedAppManagementLevels": "Targeted App Management Levels value"
}
```

### <a name="response"></a><span data-ttu-id="0771f-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="0771f-178">Response</span></span>
<span data-ttu-id="0771f-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0771f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 561

{
  "@odata.type": "#microsoft.graph.managedAppProtectionPolicySetItem",
  "id": "e10d79c9-79c9-e10d-c979-0de1c9790de1",
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
  "targetedAppManagementLevels": "Targeted App Management Levels value"
}
```






