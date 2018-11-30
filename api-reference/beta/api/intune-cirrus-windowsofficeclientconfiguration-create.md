---
title: Criar windowsOfficeClientConfiguration
description: Crie uma nova política de não relacionadas à segurança com o direcionamento de grupos.
ms.openlocfilehash: add83255d614306677787b3ed35a9792822deec2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033904"
---
# <a name="create-windowsofficeclientconfiguration"></a><span data-ttu-id="1d0f6-103">Criar windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="1d0f6-103">Create windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="1d0f6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d0f6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d0f6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d0f6-107">Crie uma nova política de não relacionadas à segurança com o direcionamento de grupos.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-107">Create a new non-security policy with targeting groups.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1d0f6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1d0f6-108">Prerequisites</span></span>
<span data-ttu-id="1d0f6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d0f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d0f6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d0f6-111">Permission type</span></span>|<span data-ttu-id="1d0f6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1d0f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d0f6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d0f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d0f6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d0f6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1d0f6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d0f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d0f6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-116">Not supported.</span></span>|
|<span data-ttu-id="1d0f6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d0f6-117">Application</span></span>|<span data-ttu-id="1d0f6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d0f6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d0f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1d0f6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d0f6-120">Request headers</span></span>
|<span data-ttu-id="1d0f6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d0f6-121">Header</span></span>|<span data-ttu-id="1d0f6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1d0f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d0f6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d0f6-123">Authorization</span></span>|<span data-ttu-id="1d0f6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d0f6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1d0f6-125">Accept</span></span>|<span data-ttu-id="1d0f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d0f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d0f6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d0f6-127">Request body</span></span>
<span data-ttu-id="1d0f6-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1d0f6-128">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="1d0f6-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d0f6-129">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="1d0f6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d0f6-130">Property</span></span>|<span data-ttu-id="1d0f6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d0f6-131">Type</span></span>|<span data-ttu-id="1d0f6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d0f6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d0f6-133">id</span><span class="sxs-lookup"><span data-stu-id="1d0f6-133">id</span></span>|<span data-ttu-id="1d0f6-134">String</span><span class="sxs-lookup"><span data-stu-id="1d0f6-134">String</span></span>|<span data-ttu-id="1d0f6-135">ID da diretiva de configuração do cliente do office.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-135">Id of the office client configuration policy.</span></span> <span data-ttu-id="1d0f6-136">Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d0f6-136">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="1d0f6-137">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="1d0f6-137">userPreferencePayload</span></span>|<span data-ttu-id="1d0f6-138">Stream</span><span class="sxs-lookup"><span data-stu-id="1d0f6-138">Stream</span></span>|<span data-ttu-id="1d0f6-139">Configurações de preferência JSON da cadeia de caracteres em formato binário, esses valores podem ser substituídos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-139">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="1d0f6-140">Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d0f6-140">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="1d0f6-141">policyPayload</span><span class="sxs-lookup"><span data-stu-id="1d0f6-141">policyPayload</span></span>|<span data-ttu-id="1d0f6-142">Stream</span><span class="sxs-lookup"><span data-stu-id="1d0f6-142">Stream</span></span>|<span data-ttu-id="1d0f6-143">Configurações de diretiva JSON da cadeia de caracteres em formato binário, esses valores não podem ser alterados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-143">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="1d0f6-144">Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d0f6-144">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="1d0f6-145">description</span><span class="sxs-lookup"><span data-stu-id="1d0f6-145">description</span></span>|<span data-ttu-id="1d0f6-146">String</span><span class="sxs-lookup"><span data-stu-id="1d0f6-146">String</span></span>|<span data-ttu-id="1d0f6-147">Admin fornecida a descrição do cliente do office política de configuração.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-147">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="1d0f6-148">Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d0f6-148">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="1d0f6-149">displayName</span><span class="sxs-lookup"><span data-stu-id="1d0f6-149">displayName</span></span>|<span data-ttu-id="1d0f6-150">String</span><span class="sxs-lookup"><span data-stu-id="1d0f6-150">String</span></span>|<span data-ttu-id="1d0f6-151">Admin fornecido o nome da política de configuração do cliente office.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-151">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="1d0f6-152">Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d0f6-152">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="1d0f6-153">assignments</span><span class="sxs-lookup"><span data-stu-id="1d0f6-153">assignments</span></span>|<span data-ttu-id="1d0f6-154">coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1d0f6-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="1d0f6-155">A lista de atribuições de grupo para a política..</span><span class="sxs-lookup"><span data-stu-id="1d0f6-155">The list of group assignments for the policy..</span></span> <span data-ttu-id="1d0f6-156">Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d0f6-156">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="1d0f6-157">prioridade</span><span class="sxs-lookup"><span data-stu-id="1d0f6-157">priority</span></span>|<span data-ttu-id="1d0f6-158">Int32</span><span class="sxs-lookup"><span data-stu-id="1d0f6-158">Int32</span></span>|<span data-ttu-id="1d0f6-159">Valor de prioridade deve ser um valor exclusivo para cada política em um locatário e será usado para resolução de conflito, valores inferiores média de prioridade é alta.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-159">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="1d0f6-160">Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d0f6-160">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="1d0f6-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d0f6-161">lastModifiedDateTime</span></span>|<span data-ttu-id="1d0f6-162">DateTime</span><span class="sxs-lookup"><span data-stu-id="1d0f6-162">DateTime</span></span>|<span data-ttu-id="1d0f6-163">Carimbo de data e hora modificadas por último da política.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-163">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="1d0f6-164">Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d0f6-164">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="1d0f6-165">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="1d0f6-165">userCheckinSummary</span></span>|[<span data-ttu-id="1d0f6-166">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="1d0f6-166">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="1d0f6-167">Check-in do resumo do usuário para a política.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-167">User check-in summary for the policy.</span></span> <span data-ttu-id="1d0f6-168">Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d0f6-168">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="1d0f6-169">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="1d0f6-169">checkinStatuses</span></span>|<span data-ttu-id="1d0f6-170">coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="1d0f6-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="1d0f6-171">Lista de status de check-in do cliente do office.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-171">List of office Client check-in status.</span></span> <span data-ttu-id="1d0f6-172">Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d0f6-172">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="1d0f6-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d0f6-173">Response</span></span>
<span data-ttu-id="1d0f6-174">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-174">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d0f6-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d0f6-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="1d0f6-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d0f6-176">Request</span></span>
<span data-ttu-id="1d0f6-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1d0f6-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d0f6-178">Response</span></span>
<span data-ttu-id="1d0f6-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



