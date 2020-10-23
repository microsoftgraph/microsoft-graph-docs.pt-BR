---
title: Criar mdmWindowsInformationProtectionPolicyPolicySetItem
description: Criar um novo objeto mdmWindowsInformationProtectionPolicyPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f964723e56da8b67e4aae16e59d0677121ef17e0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695303"
---
# <a name="create-mdmwindowsinformationprotectionpolicypolicysetitem"></a><span data-ttu-id="93c0b-103">Criar mdmWindowsInformationProtectionPolicyPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="93c0b-103">Create mdmWindowsInformationProtectionPolicyPolicySetItem</span></span>

<span data-ttu-id="93c0b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93c0b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93c0b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="93c0b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93c0b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="93c0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93c0b-107">Criar um novo objeto [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="93c0b-107">Create a new [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93c0b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="93c0b-108">Prerequisites</span></span>
<span data-ttu-id="93c0b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93c0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93c0b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93c0b-111">Permission type</span></span>|<span data-ttu-id="93c0b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="93c0b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93c0b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93c0b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93c0b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93c0b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="93c0b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93c0b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93c0b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93c0b-116">Not supported.</span></span>|
|<span data-ttu-id="93c0b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93c0b-117">Application</span></span>|<span data-ttu-id="93c0b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93c0b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="93c0b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93c0b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="93c0b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93c0b-120">Request headers</span></span>
|<span data-ttu-id="93c0b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="93c0b-121">Header</span></span>|<span data-ttu-id="93c0b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="93c0b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93c0b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="93c0b-123">Authorization</span></span>|<span data-ttu-id="93c0b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93c0b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93c0b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="93c0b-125">Accept</span></span>|<span data-ttu-id="93c0b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93c0b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93c0b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93c0b-127">Request body</span></span>
<span data-ttu-id="93c0b-128">No corpo da solicitação, forneça uma representação JSON do objeto mdmWindowsInformationProtectionPolicyPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="93c0b-128">In the request body, supply a JSON representation for the mdmWindowsInformationProtectionPolicyPolicySetItem object.</span></span>

<span data-ttu-id="93c0b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar mdmWindowsInformationProtectionPolicyPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="93c0b-129">The following table shows the properties that are required when you create the mdmWindowsInformationProtectionPolicyPolicySetItem.</span></span>

|<span data-ttu-id="93c0b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93c0b-130">Property</span></span>|<span data-ttu-id="93c0b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="93c0b-131">Type</span></span>|<span data-ttu-id="93c0b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="93c0b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93c0b-133">id</span><span class="sxs-lookup"><span data-stu-id="93c0b-133">id</span></span>|<span data-ttu-id="93c0b-134">String</span><span class="sxs-lookup"><span data-stu-id="93c0b-134">String</span></span>|<span data-ttu-id="93c0b-135">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="93c0b-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="93c0b-136">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="93c0b-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="93c0b-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93c0b-137">createdDateTime</span></span>|<span data-ttu-id="93c0b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93c0b-138">DateTimeOffset</span></span>|<span data-ttu-id="93c0b-139">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="93c0b-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="93c0b-140">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="93c0b-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="93c0b-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93c0b-141">lastModifiedDateTime</span></span>|<span data-ttu-id="93c0b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93c0b-142">DateTimeOffset</span></span>|<span data-ttu-id="93c0b-143">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="93c0b-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="93c0b-144">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="93c0b-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="93c0b-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="93c0b-145">payloadId</span></span>|<span data-ttu-id="93c0b-146">String</span><span class="sxs-lookup"><span data-stu-id="93c0b-146">String</span></span>|<span data-ttu-id="93c0b-147">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="93c0b-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="93c0b-148">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="93c0b-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="93c0b-149">itemType</span><span class="sxs-lookup"><span data-stu-id="93c0b-149">itemType</span></span>|<span data-ttu-id="93c0b-150">String</span><span class="sxs-lookup"><span data-stu-id="93c0b-150">String</span></span>|<span data-ttu-id="93c0b-151">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="93c0b-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="93c0b-152">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="93c0b-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="93c0b-153">displayName</span><span class="sxs-lookup"><span data-stu-id="93c0b-153">displayName</span></span>|<span data-ttu-id="93c0b-154">String</span><span class="sxs-lookup"><span data-stu-id="93c0b-154">String</span></span>|<span data-ttu-id="93c0b-155">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="93c0b-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="93c0b-156">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="93c0b-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="93c0b-157">status</span><span class="sxs-lookup"><span data-stu-id="93c0b-157">status</span></span>|[<span data-ttu-id="93c0b-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="93c0b-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="93c0b-159">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="93c0b-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="93c0b-160">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="93c0b-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="93c0b-161">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="93c0b-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="93c0b-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="93c0b-162">errorCode</span></span>|[<span data-ttu-id="93c0b-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="93c0b-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="93c0b-164">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="93c0b-164">Error code if any occured.</span></span> <span data-ttu-id="93c0b-165">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="93c0b-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="93c0b-166">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="93c0b-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="93c0b-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="93c0b-167">guidedDeploymentTags</span></span>|<span data-ttu-id="93c0b-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="93c0b-168">String collection</span></span>|<span data-ttu-id="93c0b-169">Marcas da implantação dirigida herdadas de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="93c0b-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="93c0b-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="93c0b-170">Response</span></span>
<span data-ttu-id="93c0b-171">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93c0b-171">If successful, this method returns a `201 Created` response code and a [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93c0b-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93c0b-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="93c0b-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93c0b-173">Request</span></span>
<span data-ttu-id="93c0b-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93c0b-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
Content-type: application/json
Content-length: 332

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicyPolicySetItem",
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

### <a name="response"></a><span data-ttu-id="93c0b-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="93c0b-175">Response</span></span>
<span data-ttu-id="93c0b-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93c0b-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 504

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicyPolicySetItem",
  "id": "4ac5be70-be70-4ac5-70be-c54a70bec54a",
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





