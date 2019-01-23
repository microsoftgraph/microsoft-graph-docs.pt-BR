---
title: Criar windowsOfficeClientConfiguration
description: Crie uma nova política de não relacionadas à segurança com o direcionamento de grupos.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a915447ad22438d021bb4577fc856bbe89db1fdc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394373"
---
# <a name="create-windowsofficeclientconfiguration"></a><span data-ttu-id="01735-103">Criar windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="01735-103">Create windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="01735-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="01735-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="01735-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="01735-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01735-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="01735-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01735-107">Crie uma nova política de não relacionadas à segurança com o direcionamento de grupos.</span><span class="sxs-lookup"><span data-stu-id="01735-107">Create a new non-security policy with targeting groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01735-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="01735-108">Prerequisites</span></span>
<span data-ttu-id="01735-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01735-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01735-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01735-111">Permission type</span></span>|<span data-ttu-id="01735-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="01735-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01735-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01735-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01735-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01735-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01735-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01735-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01735-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01735-116">Not supported.</span></span>|
|<span data-ttu-id="01735-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01735-117">Application</span></span>|<span data-ttu-id="01735-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01735-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01735-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01735-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="01735-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01735-120">Request headers</span></span>
|<span data-ttu-id="01735-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01735-121">Header</span></span>|<span data-ttu-id="01735-122">Valor</span><span class="sxs-lookup"><span data-stu-id="01735-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01735-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="01735-123">Authorization</span></span>|<span data-ttu-id="01735-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01735-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01735-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="01735-125">Accept</span></span>|<span data-ttu-id="01735-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01735-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01735-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01735-127">Request body</span></span>
<span data-ttu-id="01735-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="01735-128">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="01735-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01735-129">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="01735-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01735-130">Property</span></span>|<span data-ttu-id="01735-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="01735-131">Type</span></span>|<span data-ttu-id="01735-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="01735-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01735-133">id</span><span class="sxs-lookup"><span data-stu-id="01735-133">id</span></span>|<span data-ttu-id="01735-134">String</span><span class="sxs-lookup"><span data-stu-id="01735-134">String</span></span>|<span data-ttu-id="01735-135">ID da diretiva de configuração do cliente do office.</span><span class="sxs-lookup"><span data-stu-id="01735-135">Id of the office client configuration policy.</span></span> <span data-ttu-id="01735-136">Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01735-136">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="01735-137">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="01735-137">userPreferencePayload</span></span>|<span data-ttu-id="01735-138">Stream</span><span class="sxs-lookup"><span data-stu-id="01735-138">Stream</span></span>|<span data-ttu-id="01735-139">Configurações de preferência JSON da cadeia de caracteres em formato binário, esses valores podem ser substituídos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="01735-139">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="01735-140">Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01735-140">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="01735-141">policyPayload</span><span class="sxs-lookup"><span data-stu-id="01735-141">policyPayload</span></span>|<span data-ttu-id="01735-142">Stream</span><span class="sxs-lookup"><span data-stu-id="01735-142">Stream</span></span>|<span data-ttu-id="01735-143">Configurações de diretiva JSON da cadeia de caracteres em formato binário, esses valores não podem ser alterados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="01735-143">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="01735-144">Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01735-144">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="01735-145">description</span><span class="sxs-lookup"><span data-stu-id="01735-145">description</span></span>|<span data-ttu-id="01735-146">String</span><span class="sxs-lookup"><span data-stu-id="01735-146">String</span></span>|<span data-ttu-id="01735-147">Admin fornecida a descrição do cliente do office política de configuração.</span><span class="sxs-lookup"><span data-stu-id="01735-147">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="01735-148">Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01735-148">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="01735-149">displayName</span><span class="sxs-lookup"><span data-stu-id="01735-149">displayName</span></span>|<span data-ttu-id="01735-150">String</span><span class="sxs-lookup"><span data-stu-id="01735-150">String</span></span>|<span data-ttu-id="01735-151">Admin fornecido o nome da política de configuração do cliente office.</span><span class="sxs-lookup"><span data-stu-id="01735-151">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="01735-152">Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01735-152">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="01735-153">assignments</span><span class="sxs-lookup"><span data-stu-id="01735-153">assignments</span></span>|<span data-ttu-id="01735-154">coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="01735-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="01735-155">A lista de atribuições de grupo para a política..</span><span class="sxs-lookup"><span data-stu-id="01735-155">The list of group assignments for the policy..</span></span> <span data-ttu-id="01735-156">Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01735-156">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="01735-157">prioridade</span><span class="sxs-lookup"><span data-stu-id="01735-157">priority</span></span>|<span data-ttu-id="01735-158">Int32</span><span class="sxs-lookup"><span data-stu-id="01735-158">Int32</span></span>|<span data-ttu-id="01735-159">Valor de prioridade deve ser um valor exclusivo para cada política em um locatário e será usado para resolução de conflito, valores inferiores média de prioridade é alta.</span><span class="sxs-lookup"><span data-stu-id="01735-159">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="01735-160">Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01735-160">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="01735-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01735-161">lastModifiedDateTime</span></span>|<span data-ttu-id="01735-162">DateTime</span><span class="sxs-lookup"><span data-stu-id="01735-162">DateTime</span></span>|<span data-ttu-id="01735-163">Carimbo de data e hora modificadas por último da política.</span><span class="sxs-lookup"><span data-stu-id="01735-163">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="01735-164">Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01735-164">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="01735-165">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="01735-165">userCheckinSummary</span></span>|[<span data-ttu-id="01735-166">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="01735-166">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="01735-167">Check-in do resumo do usuário para a política.</span><span class="sxs-lookup"><span data-stu-id="01735-167">User check-in summary for the policy.</span></span> <span data-ttu-id="01735-168">Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01735-168">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="01735-169">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="01735-169">checkinStatuses</span></span>|<span data-ttu-id="01735-170">coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="01735-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="01735-171">Lista de status de check-in do cliente do office.</span><span class="sxs-lookup"><span data-stu-id="01735-171">List of office Client check-in status.</span></span> <span data-ttu-id="01735-172">Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01735-172">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="01735-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="01735-173">Response</span></span>
<span data-ttu-id="01735-174">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01735-174">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01735-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01735-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="01735-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01735-176">Request</span></span>
<span data-ttu-id="01735-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01735-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
Content-type: application/json
Content-length: 1020

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
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

### <a name="response"></a><span data-ttu-id="01735-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="01735-178">Response</span></span>
<span data-ttu-id="01735-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01735-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1069

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
  "id": "13a5ac73-ac73-13a5-73ac-a51373aca513",
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



