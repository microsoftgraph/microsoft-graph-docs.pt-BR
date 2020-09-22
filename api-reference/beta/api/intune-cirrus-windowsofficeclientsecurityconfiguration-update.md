---
title: Atualizar windowsOfficeClientSecurityConfiguration
description: Atualiza as propriedades de um objeto windowsOfficeClientSecurityConfiguration.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 085205dd127fbbfac4076c2c2838fdbf6e0a94e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47975098"
---
# <a name="update-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="9eac4-103">Atualizar windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="9eac4-103">Update windowsOfficeClientSecurityConfiguration</span></span>

<span data-ttu-id="9eac4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9eac4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9eac4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9eac4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9eac4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9eac4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9eac4-107">Atualiza as propriedades de um objeto [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9eac4-107">Update the properties of a [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9eac4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9eac4-108">Prerequisites</span></span>
<span data-ttu-id="9eac4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9eac4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9eac4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9eac4-111">Permission type</span></span>|<span data-ttu-id="9eac4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9eac4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9eac4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9eac4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9eac4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9eac4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9eac4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9eac4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9eac4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9eac4-116">Not supported.</span></span>|
|<span data-ttu-id="9eac4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9eac4-117">Application</span></span>|<span data-ttu-id="9eac4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9eac4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9eac4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9eac4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9eac4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9eac4-120">Request headers</span></span>
|<span data-ttu-id="9eac4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9eac4-121">Header</span></span>|<span data-ttu-id="9eac4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9eac4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9eac4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9eac4-123">Authorization</span></span>|<span data-ttu-id="9eac4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9eac4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9eac4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9eac4-125">Accept</span></span>|<span data-ttu-id="9eac4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9eac4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9eac4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9eac4-127">Request body</span></span>
<span data-ttu-id="9eac4-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9eac4-128">In the request body, supply a JSON representation for the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

<span data-ttu-id="9eac4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9eac4-129">The following table shows the properties that are required when you create the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

|<span data-ttu-id="9eac4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9eac4-130">Property</span></span>|<span data-ttu-id="9eac4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9eac4-131">Type</span></span>|<span data-ttu-id="9eac4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9eac4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9eac4-133">id</span><span class="sxs-lookup"><span data-stu-id="9eac4-133">id</span></span>|<span data-ttu-id="9eac4-134">String</span><span class="sxs-lookup"><span data-stu-id="9eac4-134">String</span></span>|<span data-ttu-id="9eac4-135">ID da política de configuração de cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="9eac4-135">Id of the office client configuration policy.</span></span> <span data-ttu-id="9eac4-136">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9eac4-136">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="9eac4-137">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="9eac4-137">userPreferencePayload</span></span>|<span data-ttu-id="9eac4-138">Stream</span><span class="sxs-lookup"><span data-stu-id="9eac4-138">Stream</span></span>|<span data-ttu-id="9eac4-139">Cadeia de caracteres JSON das configurações de preferência no formato binário, esses valores podem ser substituídos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="9eac4-139">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="9eac4-140">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9eac4-140">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="9eac4-141">policyPayload</span><span class="sxs-lookup"><span data-stu-id="9eac4-141">policyPayload</span></span>|<span data-ttu-id="9eac4-142">Stream</span><span class="sxs-lookup"><span data-stu-id="9eac4-142">Stream</span></span>|<span data-ttu-id="9eac4-143">Cadeia de caracteres JSON de configurações de política no formato binário, esses valores não podem ser alterados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="9eac4-143">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="9eac4-144">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9eac4-144">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="9eac4-145">description</span><span class="sxs-lookup"><span data-stu-id="9eac4-145">description</span></span>|<span data-ttu-id="9eac4-146">String</span><span class="sxs-lookup"><span data-stu-id="9eac4-146">String</span></span>|<span data-ttu-id="9eac4-147">Descrição fornecida pelo administrador da política de configuração de cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="9eac4-147">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="9eac4-148">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9eac4-148">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="9eac4-149">displayName</span><span class="sxs-lookup"><span data-stu-id="9eac4-149">displayName</span></span>|<span data-ttu-id="9eac4-150">String</span><span class="sxs-lookup"><span data-stu-id="9eac4-150">String</span></span>|<span data-ttu-id="9eac4-151">Nome fornecido pelo administrador da política de configuração de cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="9eac4-151">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="9eac4-152">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9eac4-152">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="9eac4-153">assignments</span><span class="sxs-lookup"><span data-stu-id="9eac4-153">assignments</span></span>|<span data-ttu-id="9eac4-154">coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9eac4-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="9eac4-155">A lista de atribuições de grupo para a política..</span><span class="sxs-lookup"><span data-stu-id="9eac4-155">The list of group assignments for the policy..</span></span> <span data-ttu-id="9eac4-156">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9eac4-156">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="9eac4-157">prioridade</span><span class="sxs-lookup"><span data-stu-id="9eac4-157">priority</span></span>|<span data-ttu-id="9eac4-158">Int32</span><span class="sxs-lookup"><span data-stu-id="9eac4-158">Int32</span></span>|<span data-ttu-id="9eac4-159">O valor de prioridade deve ser um valor exclusivo para cada política em um locatário e será usado para resolução de conflitos, a prioridade média de valores menores é alta.</span><span class="sxs-lookup"><span data-stu-id="9eac4-159">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="9eac4-160">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9eac4-160">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="9eac4-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9eac4-161">lastModifiedDateTime</span></span>|<span data-ttu-id="9eac4-162">DateTime</span><span class="sxs-lookup"><span data-stu-id="9eac4-162">DateTime</span></span>|<span data-ttu-id="9eac4-163">Carimbo de data/hora da última modificação da política.</span><span class="sxs-lookup"><span data-stu-id="9eac4-163">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="9eac4-164">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9eac4-164">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="9eac4-165">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="9eac4-165">userCheckinSummary</span></span>|[<span data-ttu-id="9eac4-166">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="9eac4-166">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="9eac4-167">Resumo de check-in do usuário da política.</span><span class="sxs-lookup"><span data-stu-id="9eac4-167">User check-in summary for the policy.</span></span> <span data-ttu-id="9eac4-168">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9eac4-168">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="9eac4-169">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="9eac4-169">checkinStatuses</span></span>|<span data-ttu-id="9eac4-170">coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="9eac4-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="9eac4-171">Lista de status de check-in do cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="9eac4-171">List of office Client check-in status.</span></span> <span data-ttu-id="9eac4-172">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9eac4-172">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="9eac4-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="9eac4-173">Response</span></span>
<span data-ttu-id="9eac4-174">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9eac4-174">If successful, this method returns a `200 OK` response code and an updated [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9eac4-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9eac4-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="9eac4-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9eac4-176">Request</span></span>
<span data-ttu-id="9eac4-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9eac4-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}
Content-type: application/json
Content-length: 949

{
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

### <a name="response"></a><span data-ttu-id="9eac4-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="9eac4-178">Response</span></span>
<span data-ttu-id="9eac4-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9eac4-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






