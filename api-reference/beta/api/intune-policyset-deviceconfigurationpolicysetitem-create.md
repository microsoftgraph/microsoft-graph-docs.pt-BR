---
title: Criar deviceConfigurationPolicySetItem
description: Criar um novo objeto deviceConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 593dfb9057144911d47f1ee450d759db532faa23
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467170"
---
# <a name="create-deviceconfigurationpolicysetitem"></a><span data-ttu-id="3e40a-103">Criar deviceConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="3e40a-103">Create deviceConfigurationPolicySetItem</span></span>

<span data-ttu-id="3e40a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e40a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e40a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3e40a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e40a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3e40a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e40a-107">Criar um novo objeto [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="3e40a-107">Create a new [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e40a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3e40a-108">Prerequisites</span></span>
<span data-ttu-id="3e40a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e40a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e40a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e40a-111">Permission type</span></span>|<span data-ttu-id="3e40a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3e40a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e40a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e40a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e40a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e40a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3e40a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e40a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e40a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e40a-116">Not supported.</span></span>|
|<span data-ttu-id="3e40a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e40a-117">Application</span></span>|<span data-ttu-id="3e40a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e40a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e40a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e40a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="3e40a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e40a-120">Request headers</span></span>
|<span data-ttu-id="3e40a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3e40a-121">Header</span></span>|<span data-ttu-id="3e40a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3e40a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e40a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e40a-123">Authorization</span></span>|<span data-ttu-id="3e40a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e40a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e40a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3e40a-125">Accept</span></span>|<span data-ttu-id="3e40a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e40a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e40a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e40a-127">Request body</span></span>
<span data-ttu-id="3e40a-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="3e40a-128">In the request body, supply a JSON representation for the deviceConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="3e40a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="3e40a-129">The following table shows the properties that are required when you create the deviceConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="3e40a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e40a-130">Property</span></span>|<span data-ttu-id="3e40a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e40a-131">Type</span></span>|<span data-ttu-id="3e40a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e40a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e40a-133">id</span><span class="sxs-lookup"><span data-stu-id="3e40a-133">id</span></span>|<span data-ttu-id="3e40a-134">String</span><span class="sxs-lookup"><span data-stu-id="3e40a-134">String</span></span>|<span data-ttu-id="3e40a-135">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="3e40a-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="3e40a-136">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3e40a-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3e40a-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e40a-137">createdDateTime</span></span>|<span data-ttu-id="3e40a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e40a-138">DateTimeOffset</span></span>|<span data-ttu-id="3e40a-139">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="3e40a-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="3e40a-140">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3e40a-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3e40a-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e40a-141">lastModifiedDateTime</span></span>|<span data-ttu-id="3e40a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e40a-142">DateTimeOffset</span></span>|<span data-ttu-id="3e40a-143">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="3e40a-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="3e40a-144">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3e40a-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3e40a-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="3e40a-145">payloadId</span></span>|<span data-ttu-id="3e40a-146">String</span><span class="sxs-lookup"><span data-stu-id="3e40a-146">String</span></span>|<span data-ttu-id="3e40a-147">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="3e40a-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="3e40a-148">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3e40a-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3e40a-149">itemType</span><span class="sxs-lookup"><span data-stu-id="3e40a-149">itemType</span></span>|<span data-ttu-id="3e40a-150">String</span><span class="sxs-lookup"><span data-stu-id="3e40a-150">String</span></span>|<span data-ttu-id="3e40a-151">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="3e40a-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="3e40a-152">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3e40a-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3e40a-153">displayName</span><span class="sxs-lookup"><span data-stu-id="3e40a-153">displayName</span></span>|<span data-ttu-id="3e40a-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e40a-154">String</span></span>|<span data-ttu-id="3e40a-155">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="3e40a-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="3e40a-156">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3e40a-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3e40a-157">status</span><span class="sxs-lookup"><span data-stu-id="3e40a-157">status</span></span>|[<span data-ttu-id="3e40a-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="3e40a-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="3e40a-159">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="3e40a-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="3e40a-160">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="3e40a-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="3e40a-161">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="3e40a-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="3e40a-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="3e40a-162">errorCode</span></span>|[<span data-ttu-id="3e40a-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="3e40a-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="3e40a-164">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="3e40a-164">Error code if any occured.</span></span> <span data-ttu-id="3e40a-165">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="3e40a-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="3e40a-166">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="3e40a-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="3e40a-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="3e40a-167">guidedDeploymentTags</span></span>|<span data-ttu-id="3e40a-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e40a-168">String collection</span></span>|<span data-ttu-id="3e40a-169">Marcas da implantação dirigida herdadas de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3e40a-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="3e40a-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e40a-170">Response</span></span>
<span data-ttu-id="3e40a-171">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e40a-171">If successful, this method returns a `201 Created` response code and a [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e40a-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e40a-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e40a-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e40a-173">Request</span></span>
<span data-ttu-id="3e40a-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e40a-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
Content-type: application/json
Content-length: 314

{
  "@odata.type": "#microsoft.graph.deviceConfigurationPolicySetItem",
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

### <a name="response"></a><span data-ttu-id="3e40a-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e40a-175">Response</span></span>
<span data-ttu-id="3e40a-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e40a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 486

{
  "@odata.type": "#microsoft.graph.deviceConfigurationPolicySetItem",
  "id": "00b1197c-197c-00b1-7c19-b1007c19b100",
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



