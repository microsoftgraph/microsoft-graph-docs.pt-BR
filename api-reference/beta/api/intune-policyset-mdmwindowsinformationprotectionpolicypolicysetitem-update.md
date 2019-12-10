---
title: Atualizar mdmWindowsInformationProtectionPolicyPolicySetItem
description: Atualiza as propriedades de um objeto mdmWindowsInformationProtectionPolicyPolicySetItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 92a13d8fc7fc01a4576d4f1ace96f822ba04e4af
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941019"
---
# <a name="update-mdmwindowsinformationprotectionpolicypolicysetitem"></a><span data-ttu-id="a96e0-103">Atualizar mdmWindowsInformationProtectionPolicyPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="a96e0-103">Update mdmWindowsInformationProtectionPolicyPolicySetItem</span></span>

> <span data-ttu-id="a96e0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a96e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a96e0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a96e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a96e0-106">Atualiza as propriedades de um objeto [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="a96e0-106">Update the properties of a [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a96e0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a96e0-107">Prerequisites</span></span>
<span data-ttu-id="a96e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a96e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a96e0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a96e0-110">Permission type</span></span>|<span data-ttu-id="a96e0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a96e0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a96e0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a96e0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a96e0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a96e0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a96e0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a96e0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a96e0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a96e0-115">Not supported.</span></span>|
|<span data-ttu-id="a96e0-116">Application</span><span class="sxs-lookup"><span data-stu-id="a96e0-116">Application</span></span>|<span data-ttu-id="a96e0-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a96e0-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a96e0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a96e0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="a96e0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a96e0-119">Request headers</span></span>
|<span data-ttu-id="a96e0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a96e0-120">Header</span></span>|<span data-ttu-id="a96e0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a96e0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a96e0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a96e0-122">Authorization</span></span>|<span data-ttu-id="a96e0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a96e0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a96e0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a96e0-124">Accept</span></span>|<span data-ttu-id="a96e0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a96e0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a96e0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a96e0-126">Request body</span></span>
<span data-ttu-id="a96e0-127">No corpo da solicitação, forneça uma representação JSON do objeto [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="a96e0-127">In the request body, supply a JSON representation for the [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) object.</span></span>

<span data-ttu-id="a96e0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="a96e0-128">The following table shows the properties that are required when you create the [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md).</span></span>

|<span data-ttu-id="a96e0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a96e0-129">Property</span></span>|<span data-ttu-id="a96e0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a96e0-130">Type</span></span>|<span data-ttu-id="a96e0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a96e0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a96e0-132">id</span><span class="sxs-lookup"><span data-stu-id="a96e0-132">id</span></span>|<span data-ttu-id="a96e0-133">String</span><span class="sxs-lookup"><span data-stu-id="a96e0-133">String</span></span>|<span data-ttu-id="a96e0-134">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="a96e0-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="a96e0-135">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="a96e0-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="a96e0-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a96e0-136">createdDateTime</span></span>|<span data-ttu-id="a96e0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a96e0-137">DateTimeOffset</span></span>|<span data-ttu-id="a96e0-138">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="a96e0-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="a96e0-139">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="a96e0-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="a96e0-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a96e0-140">lastModifiedDateTime</span></span>|<span data-ttu-id="a96e0-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a96e0-141">DateTimeOffset</span></span>|<span data-ttu-id="a96e0-142">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="a96e0-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="a96e0-143">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="a96e0-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="a96e0-144">payloadId</span><span class="sxs-lookup"><span data-stu-id="a96e0-144">payloadId</span></span>|<span data-ttu-id="a96e0-145">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a96e0-145">String</span></span>|<span data-ttu-id="a96e0-146">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="a96e0-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="a96e0-147">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="a96e0-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="a96e0-148">itemType</span><span class="sxs-lookup"><span data-stu-id="a96e0-148">itemType</span></span>|<span data-ttu-id="a96e0-149">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a96e0-149">String</span></span>|<span data-ttu-id="a96e0-150">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="a96e0-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="a96e0-151">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="a96e0-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="a96e0-152">displayName</span><span class="sxs-lookup"><span data-stu-id="a96e0-152">displayName</span></span>|<span data-ttu-id="a96e0-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a96e0-153">String</span></span>|<span data-ttu-id="a96e0-154">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="a96e0-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="a96e0-155">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="a96e0-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="a96e0-156">status</span><span class="sxs-lookup"><span data-stu-id="a96e0-156">status</span></span>|[<span data-ttu-id="a96e0-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="a96e0-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="a96e0-158">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="a96e0-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="a96e0-159">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="a96e0-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="a96e0-160">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a96e0-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="a96e0-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="a96e0-161">errorCode</span></span>|[<span data-ttu-id="a96e0-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="a96e0-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="a96e0-163">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="a96e0-163">Error code if any occured.</span></span> <span data-ttu-id="a96e0-164">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="a96e0-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="a96e0-165">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="a96e0-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="a96e0-166">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="a96e0-166">guidedDeploymentTags</span></span>|<span data-ttu-id="a96e0-167">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a96e0-167">String collection</span></span>|<span data-ttu-id="a96e0-168">Marcas da implantação dirigida herdadas de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="a96e0-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a96e0-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="a96e0-169">Response</span></span>
<span data-ttu-id="a96e0-170">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a96e0-170">If successful, this method returns a `200 OK` response code and an updated [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a96e0-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a96e0-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="a96e0-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a96e0-172">Request</span></span>
<span data-ttu-id="a96e0-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a96e0-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
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

### <a name="response"></a><span data-ttu-id="a96e0-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="a96e0-174">Response</span></span>
<span data-ttu-id="a96e0-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a96e0-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





