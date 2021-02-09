---
title: Criar mobileAppPolicySetItem
description: Crie um novo objeto mobileAppPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2db884dfec7bf2460b80c30f3fc96155f22e1111
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159315"
---
# <a name="create-mobileapppolicysetitem"></a><span data-ttu-id="af43b-103">Criar mobileAppPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="af43b-103">Create mobileAppPolicySetItem</span></span>

<span data-ttu-id="af43b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af43b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af43b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="af43b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af43b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="af43b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af43b-107">Crie um novo [objeto mobileAppPolicySetItem.](../resources/intune-policyset-mobileapppolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="af43b-107">Create a new [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af43b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="af43b-108">Prerequisites</span></span>
<span data-ttu-id="af43b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af43b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af43b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af43b-111">Permission type</span></span>|<span data-ttu-id="af43b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="af43b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af43b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af43b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af43b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af43b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="af43b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af43b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af43b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af43b-116">Not supported.</span></span>|
|<span data-ttu-id="af43b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af43b-117">Application</span></span>|<span data-ttu-id="af43b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af43b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af43b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af43b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="af43b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af43b-120">Request headers</span></span>
|<span data-ttu-id="af43b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="af43b-121">Header</span></span>|<span data-ttu-id="af43b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="af43b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af43b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="af43b-123">Authorization</span></span>|<span data-ttu-id="af43b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af43b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af43b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="af43b-125">Accept</span></span>|<span data-ttu-id="af43b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af43b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af43b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af43b-127">Request body</span></span>
<span data-ttu-id="af43b-128">No corpo da solicitação, fornece uma representação JSON do objeto mobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="af43b-128">In the request body, supply a JSON representation for the mobileAppPolicySetItem object.</span></span>

<span data-ttu-id="af43b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="af43b-129">The following table shows the properties that are required when you create the mobileAppPolicySetItem.</span></span>

|<span data-ttu-id="af43b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af43b-130">Property</span></span>|<span data-ttu-id="af43b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="af43b-131">Type</span></span>|<span data-ttu-id="af43b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="af43b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af43b-133">id</span><span class="sxs-lookup"><span data-stu-id="af43b-133">id</span></span>|<span data-ttu-id="af43b-134">String</span><span class="sxs-lookup"><span data-stu-id="af43b-134">String</span></span>|<span data-ttu-id="af43b-135">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="af43b-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="af43b-136">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="af43b-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="af43b-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af43b-137">createdDateTime</span></span>|<span data-ttu-id="af43b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af43b-138">DateTimeOffset</span></span>|<span data-ttu-id="af43b-139">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="af43b-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="af43b-140">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="af43b-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="af43b-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af43b-141">lastModifiedDateTime</span></span>|<span data-ttu-id="af43b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af43b-142">DateTimeOffset</span></span>|<span data-ttu-id="af43b-143">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="af43b-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="af43b-144">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="af43b-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="af43b-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="af43b-145">payloadId</span></span>|<span data-ttu-id="af43b-146">String</span><span class="sxs-lookup"><span data-stu-id="af43b-146">String</span></span>|<span data-ttu-id="af43b-147">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="af43b-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="af43b-148">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="af43b-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="af43b-149">itemType</span><span class="sxs-lookup"><span data-stu-id="af43b-149">itemType</span></span>|<span data-ttu-id="af43b-150">String</span><span class="sxs-lookup"><span data-stu-id="af43b-150">String</span></span>|<span data-ttu-id="af43b-151">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="af43b-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="af43b-152">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="af43b-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="af43b-153">displayName</span><span class="sxs-lookup"><span data-stu-id="af43b-153">displayName</span></span>|<span data-ttu-id="af43b-154">String</span><span class="sxs-lookup"><span data-stu-id="af43b-154">String</span></span>|<span data-ttu-id="af43b-155">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="af43b-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="af43b-156">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="af43b-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="af43b-157">status</span><span class="sxs-lookup"><span data-stu-id="af43b-157">status</span></span>|[<span data-ttu-id="af43b-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="af43b-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="af43b-159">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="af43b-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="af43b-160">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="af43b-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="af43b-161">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="af43b-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="af43b-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="af43b-162">errorCode</span></span>|[<span data-ttu-id="af43b-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="af43b-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="af43b-164">Código de erro se ocorreu.</span><span class="sxs-lookup"><span data-stu-id="af43b-164">Error code if any occured.</span></span> <span data-ttu-id="af43b-165">Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="af43b-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="af43b-166">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="af43b-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="af43b-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="af43b-167">guidedDeploymentTags</span></span>|<span data-ttu-id="af43b-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="af43b-168">String collection</span></span>|<span data-ttu-id="af43b-169">Marcas da implantação guiada Herdada [de policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="af43b-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="af43b-170">finalidade</span><span class="sxs-lookup"><span data-stu-id="af43b-170">intent</span></span>|[<span data-ttu-id="af43b-171">installIntent</span><span class="sxs-lookup"><span data-stu-id="af43b-171">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="af43b-172">Intenção de instalação do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="af43b-172">Install intent of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="af43b-173">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="af43b-173">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="af43b-174">configurações</span><span class="sxs-lookup"><span data-stu-id="af43b-174">settings</span></span>|[<span data-ttu-id="af43b-175">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="af43b-175">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="af43b-176">Configurações do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="af43b-176">Settings of the MobileAppPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="af43b-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="af43b-177">Response</span></span>
<span data-ttu-id="af43b-178">Se tiver êxito, este método retornará um código de resposta e um objeto `201 Created` [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af43b-178">If successful, this method returns a `201 Created` response code and a [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af43b-179">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af43b-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="af43b-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af43b-180">Request</span></span>
<span data-ttu-id="af43b-181">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af43b-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
Content-type: application/json
Content-length: 540

{
  "@odata.type": "#microsoft.graph.mobileAppPolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "intent": "required",
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "Vpn Configuration Id value",
    "uninstallOnDeviceRemoval": true,
    "isRemovable": true
  }
}
```

### <a name="response"></a><span data-ttu-id="af43b-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="af43b-182">Response</span></span>
<span data-ttu-id="af43b-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af43b-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 712

{
  "@odata.type": "#microsoft.graph.mobileAppPolicySetItem",
  "id": "b6ffe6cf-e6cf-b6ff-cfe6-ffb6cfe6ffb6",
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
  "intent": "required",
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "Vpn Configuration Id value",
    "uninstallOnDeviceRemoval": true,
    "isRemovable": true
  }
}
```




