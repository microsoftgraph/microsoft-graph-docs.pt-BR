---
title: Atualizar windowsOfficeClientSecurityConfiguration
description: Atualiza as propriedades de um objeto windowsOfficeClientSecurityConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8ff4df803272ef4c3d3ec8f07d553fe7abddbb65
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32483247"
---
# <a name="update-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="f381b-103">Atualizar windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="f381b-103">Update windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="f381b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f381b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f381b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f381b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f381b-106">Atualiza as propriedades de um objeto [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f381b-106">Update the properties of a [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f381b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f381b-107">Prerequisites</span></span>
<span data-ttu-id="f381b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f381b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f381b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f381b-110">Permission type</span></span>|<span data-ttu-id="f381b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f381b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f381b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f381b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f381b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f381b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f381b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f381b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f381b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f381b-115">Not supported.</span></span>|
|<span data-ttu-id="f381b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f381b-116">Application</span></span>|<span data-ttu-id="f381b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f381b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f381b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f381b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f381b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f381b-119">Request headers</span></span>
|<span data-ttu-id="f381b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f381b-120">Header</span></span>|<span data-ttu-id="f381b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f381b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f381b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f381b-122">Authorization</span></span>|<span data-ttu-id="f381b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f381b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f381b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f381b-124">Accept</span></span>|<span data-ttu-id="f381b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f381b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f381b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f381b-126">Request body</span></span>
<span data-ttu-id="f381b-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f381b-127">In the request body, supply a JSON representation for the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

<span data-ttu-id="f381b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f381b-128">The following table shows the properties that are required when you create the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

|<span data-ttu-id="f381b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f381b-129">Property</span></span>|<span data-ttu-id="f381b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f381b-130">Type</span></span>|<span data-ttu-id="f381b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f381b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f381b-132">id</span><span class="sxs-lookup"><span data-stu-id="f381b-132">id</span></span>|<span data-ttu-id="f381b-133">String</span><span class="sxs-lookup"><span data-stu-id="f381b-133">String</span></span>|<span data-ttu-id="f381b-134">ID da política de configuração de cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="f381b-134">Id of the office client configuration policy.</span></span> <span data-ttu-id="f381b-135">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f381b-135">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="f381b-136">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="f381b-136">userPreferencePayload</span></span>|<span data-ttu-id="f381b-137">Stream</span><span class="sxs-lookup"><span data-stu-id="f381b-137">Stream</span></span>|<span data-ttu-id="f381b-138">Cadeia de caracteres JSON das configurações de preferência no formato binário, esses valores podem ser substituídos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="f381b-138">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="f381b-139">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f381b-139">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="f381b-140">policyPayload</span><span class="sxs-lookup"><span data-stu-id="f381b-140">policyPayload</span></span>|<span data-ttu-id="f381b-141">Stream</span><span class="sxs-lookup"><span data-stu-id="f381b-141">Stream</span></span>|<span data-ttu-id="f381b-142">Cadeia de caracteres JSON de configurações de política no formato binário, esses valores não podem ser alterados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="f381b-142">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="f381b-143">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f381b-143">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="f381b-144">description</span><span class="sxs-lookup"><span data-stu-id="f381b-144">description</span></span>|<span data-ttu-id="f381b-145">String</span><span class="sxs-lookup"><span data-stu-id="f381b-145">String</span></span>|<span data-ttu-id="f381b-146">Descrição fornecida pelo administrador da política de configuração de cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="f381b-146">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="f381b-147">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f381b-147">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="f381b-148">displayName</span><span class="sxs-lookup"><span data-stu-id="f381b-148">displayName</span></span>|<span data-ttu-id="f381b-149">String</span><span class="sxs-lookup"><span data-stu-id="f381b-149">String</span></span>|<span data-ttu-id="f381b-150">Nome fornecido pelo administrador da política de configuração de cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="f381b-150">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="f381b-151">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f381b-151">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="f381b-152">assignments</span><span class="sxs-lookup"><span data-stu-id="f381b-152">assignments</span></span>|<span data-ttu-id="f381b-153">coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f381b-153">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="f381b-154">A lista de atribuições de grupo para a política..</span><span class="sxs-lookup"><span data-stu-id="f381b-154">The list of group assignments for the policy..</span></span> <span data-ttu-id="f381b-155">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f381b-155">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="f381b-156">prioridade</span><span class="sxs-lookup"><span data-stu-id="f381b-156">priority</span></span>|<span data-ttu-id="f381b-157">Int32</span><span class="sxs-lookup"><span data-stu-id="f381b-157">Int32</span></span>|<span data-ttu-id="f381b-158">O valor de prioridade deve ser um valor exclusivo para cada política em um locatário e será usado para resolução de conflitos, a prioridade média de valores menores é alta.</span><span class="sxs-lookup"><span data-stu-id="f381b-158">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="f381b-159">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f381b-159">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="f381b-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f381b-160">lastModifiedDateTime</span></span>|<span data-ttu-id="f381b-161">DateTime</span><span class="sxs-lookup"><span data-stu-id="f381b-161">DateTime</span></span>|<span data-ttu-id="f381b-162">Carimbo de data/hora da última modificação da política.</span><span class="sxs-lookup"><span data-stu-id="f381b-162">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="f381b-163">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f381b-163">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="f381b-164">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="f381b-164">userCheckinSummary</span></span>|[<span data-ttu-id="f381b-165">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="f381b-165">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="f381b-166">Resumo de check-in do usuário da política.</span><span class="sxs-lookup"><span data-stu-id="f381b-166">User check-in summary for the policy.</span></span> <span data-ttu-id="f381b-167">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f381b-167">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="f381b-168">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="f381b-168">checkinStatuses</span></span>|<span data-ttu-id="f381b-169">coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="f381b-169">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="f381b-170">Lista de status de check-in do cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="f381b-170">List of office Client check-in status.</span></span> <span data-ttu-id="f381b-171">Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f381b-171">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f381b-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="f381b-172">Response</span></span>
<span data-ttu-id="f381b-173">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f381b-173">If successful, this method returns a `200 OK` response code and an updated [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f381b-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f381b-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="f381b-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f381b-175">Request</span></span>
<span data-ttu-id="f381b-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f381b-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f381b-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="f381b-177">Response</span></span>
<span data-ttu-id="f381b-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f381b-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



