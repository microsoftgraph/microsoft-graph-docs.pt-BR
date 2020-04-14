---
title: Criar windowsOfficeClientSecurityConfiguration
description: Criar um novo objeto windowsOfficeClientSecurityConfiguration.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8ff00202f0b24fd953ca19064c64d4c270809191
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436681"
---
# <a name="create-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="df425-103">Criar windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="df425-103">Create windowsOfficeClientSecurityConfiguration</span></span>

<span data-ttu-id="df425-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df425-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df425-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="df425-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df425-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="df425-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df425-107">Criar um novo objeto [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="df425-107">Create a new [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df425-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="df425-108">Prerequisites</span></span>
<span data-ttu-id="df425-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df425-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df425-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df425-111">Permission type</span></span>|<span data-ttu-id="df425-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="df425-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df425-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df425-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df425-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df425-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="df425-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df425-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df425-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df425-116">Not supported.</span></span>|
|<span data-ttu-id="df425-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df425-117">Application</span></span>|<span data-ttu-id="df425-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df425-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df425-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df425-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="df425-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df425-120">Request headers</span></span>
|<span data-ttu-id="df425-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df425-121">Header</span></span>|<span data-ttu-id="df425-122">Valor</span><span class="sxs-lookup"><span data-stu-id="df425-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df425-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="df425-123">Authorization</span></span>|<span data-ttu-id="df425-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df425-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df425-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="df425-125">Accept</span></span>|<span data-ttu-id="df425-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df425-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df425-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df425-127">Request body</span></span>
<span data-ttu-id="df425-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="df425-128">In the request body, supply a JSON representation for the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

<span data-ttu-id="df425-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df425-129">The following table shows the properties that are required when you create the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

|<span data-ttu-id="df425-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df425-130">Property</span></span>|<span data-ttu-id="df425-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="df425-131">Type</span></span>|<span data-ttu-id="df425-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="df425-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df425-133">id</span><span class="sxs-lookup"><span data-stu-id="df425-133">id</span></span>|<span data-ttu-id="df425-134">String</span><span class="sxs-lookup"><span data-stu-id="df425-134">String</span></span>|<span data-ttu-id="df425-135">ID da política de configuração de cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="df425-135">Id of the office client configuration policy.</span></span> <span data-ttu-id="df425-136">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df425-136">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="df425-137">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="df425-137">userPreferencePayload</span></span>|<span data-ttu-id="df425-138">Stream</span><span class="sxs-lookup"><span data-stu-id="df425-138">Stream</span></span>|<span data-ttu-id="df425-139">Cadeia de caracteres JSON das configurações de preferência no formato binário, esses valores podem ser substituídos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="df425-139">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="df425-140">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df425-140">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="df425-141">policyPayload</span><span class="sxs-lookup"><span data-stu-id="df425-141">policyPayload</span></span>|<span data-ttu-id="df425-142">Stream</span><span class="sxs-lookup"><span data-stu-id="df425-142">Stream</span></span>|<span data-ttu-id="df425-143">Cadeia de caracteres JSON de configurações de política no formato binário, esses valores não podem ser alterados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="df425-143">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="df425-144">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df425-144">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="df425-145">description</span><span class="sxs-lookup"><span data-stu-id="df425-145">description</span></span>|<span data-ttu-id="df425-146">String</span><span class="sxs-lookup"><span data-stu-id="df425-146">String</span></span>|<span data-ttu-id="df425-147">Descrição fornecida pelo administrador da política de configuração de cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="df425-147">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="df425-148">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df425-148">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="df425-149">displayName</span><span class="sxs-lookup"><span data-stu-id="df425-149">displayName</span></span>|<span data-ttu-id="df425-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df425-150">String</span></span>|<span data-ttu-id="df425-151">Nome fornecido pelo administrador da política de configuração de cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="df425-151">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="df425-152">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df425-152">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="df425-153">assignments</span><span class="sxs-lookup"><span data-stu-id="df425-153">assignments</span></span>|<span data-ttu-id="df425-154">coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="df425-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="df425-155">A lista de atribuições de grupo para a política..</span><span class="sxs-lookup"><span data-stu-id="df425-155">The list of group assignments for the policy..</span></span> <span data-ttu-id="df425-156">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df425-156">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="df425-157">prioridade</span><span class="sxs-lookup"><span data-stu-id="df425-157">priority</span></span>|<span data-ttu-id="df425-158">Int32</span><span class="sxs-lookup"><span data-stu-id="df425-158">Int32</span></span>|<span data-ttu-id="df425-159">O valor de prioridade deve ser um valor exclusivo para cada política em um locatário e será usado para resolução de conflitos, a prioridade média de valores menores é alta.</span><span class="sxs-lookup"><span data-stu-id="df425-159">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="df425-160">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df425-160">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="df425-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df425-161">lastModifiedDateTime</span></span>|<span data-ttu-id="df425-162">DateTime</span><span class="sxs-lookup"><span data-stu-id="df425-162">DateTime</span></span>|<span data-ttu-id="df425-163">Carimbo de data/hora da última modificação da política.</span><span class="sxs-lookup"><span data-stu-id="df425-163">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="df425-164">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df425-164">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="df425-165">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="df425-165">userCheckinSummary</span></span>|[<span data-ttu-id="df425-166">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="df425-166">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="df425-167">Resumo de check-in do usuário da política.</span><span class="sxs-lookup"><span data-stu-id="df425-167">User check-in summary for the policy.</span></span> <span data-ttu-id="df425-168">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df425-168">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="df425-169">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="df425-169">checkinStatuses</span></span>|<span data-ttu-id="df425-170">coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="df425-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="df425-171">Lista de status de check-in do cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="df425-171">List of office Client check-in status.</span></span> <span data-ttu-id="df425-172">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df425-172">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|




## <a name="response"></a><span data-ttu-id="df425-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="df425-173">Response</span></span>
<span data-ttu-id="df425-174">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df425-174">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df425-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df425-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="df425-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df425-176">Request</span></span>
<span data-ttu-id="df425-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df425-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
Content-type: application/json
Content-length: 1028

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "Description value",
  "displayName": "Display Name value",
  "priority": 8,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "userId": "User Id value",
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="df425-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="df425-178">Response</span></span>
<span data-ttu-id="df425-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df425-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1077

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
  "id": "f90ca1a5-a1a5-f90c-a5a1-0cf9a5a10cf9",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "Description value",
  "displayName": "Display Name value",
  "priority": 8,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "userId": "User Id value",
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ]
    }
  ]
}
```



