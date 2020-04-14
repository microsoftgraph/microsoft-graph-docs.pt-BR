---
title: Atualizar managedAppProtectionPolicySetItem
description: Atualiza as propriedades de um objeto managedAppProtectionPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e6e4bc9cc9164d9c0d3751f5e8ac43bfc2e23cf6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449948"
---
# <a name="update-managedappprotectionpolicysetitem"></a><span data-ttu-id="dae5d-103">Atualizar managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="dae5d-103">Update managedAppProtectionPolicySetItem</span></span>

<span data-ttu-id="dae5d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dae5d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dae5d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dae5d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dae5d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dae5d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dae5d-107">Atualiza as propriedades de um objeto [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="dae5d-107">Update the properties of a [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dae5d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dae5d-108">Prerequisites</span></span>
<span data-ttu-id="dae5d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dae5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dae5d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dae5d-111">Permission type</span></span>|<span data-ttu-id="dae5d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dae5d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dae5d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dae5d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dae5d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dae5d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dae5d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dae5d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dae5d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dae5d-116">Not supported.</span></span>|
|<span data-ttu-id="dae5d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dae5d-117">Application</span></span>|<span data-ttu-id="dae5d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dae5d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dae5d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dae5d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="dae5d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dae5d-120">Request headers</span></span>
|<span data-ttu-id="dae5d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dae5d-121">Header</span></span>|<span data-ttu-id="dae5d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dae5d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dae5d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dae5d-123">Authorization</span></span>|<span data-ttu-id="dae5d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dae5d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dae5d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dae5d-125">Accept</span></span>|<span data-ttu-id="dae5d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dae5d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dae5d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dae5d-127">Request body</span></span>
<span data-ttu-id="dae5d-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="dae5d-128">In the request body, supply a JSON representation for the [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>

<span data-ttu-id="dae5d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="dae5d-129">The following table shows the properties that are required when you create the [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md).</span></span>

|<span data-ttu-id="dae5d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dae5d-130">Property</span></span>|<span data-ttu-id="dae5d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dae5d-131">Type</span></span>|<span data-ttu-id="dae5d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dae5d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dae5d-133">id</span><span class="sxs-lookup"><span data-stu-id="dae5d-133">id</span></span>|<span data-ttu-id="dae5d-134">String</span><span class="sxs-lookup"><span data-stu-id="dae5d-134">String</span></span>|<span data-ttu-id="dae5d-135">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="dae5d-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="dae5d-136">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="dae5d-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="dae5d-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dae5d-137">createdDateTime</span></span>|<span data-ttu-id="dae5d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dae5d-138">DateTimeOffset</span></span>|<span data-ttu-id="dae5d-139">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="dae5d-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="dae5d-140">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="dae5d-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="dae5d-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dae5d-141">lastModifiedDateTime</span></span>|<span data-ttu-id="dae5d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dae5d-142">DateTimeOffset</span></span>|<span data-ttu-id="dae5d-143">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="dae5d-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="dae5d-144">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="dae5d-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="dae5d-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="dae5d-145">payloadId</span></span>|<span data-ttu-id="dae5d-146">String</span><span class="sxs-lookup"><span data-stu-id="dae5d-146">String</span></span>|<span data-ttu-id="dae5d-147">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="dae5d-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="dae5d-148">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="dae5d-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="dae5d-149">itemType</span><span class="sxs-lookup"><span data-stu-id="dae5d-149">itemType</span></span>|<span data-ttu-id="dae5d-150">String</span><span class="sxs-lookup"><span data-stu-id="dae5d-150">String</span></span>|<span data-ttu-id="dae5d-151">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="dae5d-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="dae5d-152">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="dae5d-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="dae5d-153">displayName</span><span class="sxs-lookup"><span data-stu-id="dae5d-153">displayName</span></span>|<span data-ttu-id="dae5d-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dae5d-154">String</span></span>|<span data-ttu-id="dae5d-155">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="dae5d-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="dae5d-156">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="dae5d-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="dae5d-157">status</span><span class="sxs-lookup"><span data-stu-id="dae5d-157">status</span></span>|[<span data-ttu-id="dae5d-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="dae5d-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="dae5d-159">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="dae5d-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="dae5d-160">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="dae5d-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="dae5d-161">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="dae5d-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="dae5d-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="dae5d-162">errorCode</span></span>|[<span data-ttu-id="dae5d-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="dae5d-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="dae5d-164">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="dae5d-164">Error code if any occured.</span></span> <span data-ttu-id="dae5d-165">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="dae5d-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="dae5d-166">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="dae5d-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="dae5d-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="dae5d-167">guidedDeploymentTags</span></span>|<span data-ttu-id="dae5d-168">Coleção String</span><span class="sxs-lookup"><span data-stu-id="dae5d-168">String collection</span></span>|<span data-ttu-id="dae5d-169">Marcas da implantação dirigida herdadas de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="dae5d-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="dae5d-170">targetedAppManagementLevels</span><span class="sxs-lookup"><span data-stu-id="dae5d-170">targetedAppManagementLevels</span></span>|<span data-ttu-id="dae5d-171">String</span><span class="sxs-lookup"><span data-stu-id="dae5d-171">String</span></span>|<span data-ttu-id="dae5d-172">TargetedAppManagementLevels do ManagedAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="dae5d-172">TargetedAppManagementLevels of the ManagedAppPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="dae5d-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="dae5d-173">Response</span></span>
<span data-ttu-id="dae5d-174">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dae5d-174">If successful, this method returns a `200 OK` response code and an updated [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dae5d-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dae5d-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="dae5d-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dae5d-176">Request</span></span>
<span data-ttu-id="dae5d-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dae5d-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
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

### <a name="response"></a><span data-ttu-id="dae5d-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="dae5d-178">Response</span></span>
<span data-ttu-id="dae5d-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dae5d-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



