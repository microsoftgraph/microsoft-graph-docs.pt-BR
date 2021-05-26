---
title: Criar windowsOfficeClientConfiguration
description: Crie uma nova política que não seja de segurança com grupos de direcionamento.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 159a99785a63e74f863c977a8c0bfe933f8ced75
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665680"
---
# <a name="create-windowsofficeclientconfiguration"></a><span data-ttu-id="3ea30-103">Criar windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="3ea30-103">Create windowsOfficeClientConfiguration</span></span>

<span data-ttu-id="3ea30-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ea30-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ea30-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3ea30-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ea30-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3ea30-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ea30-107">Crie uma nova política que não seja de segurança com grupos de direcionamento.</span><span class="sxs-lookup"><span data-stu-id="3ea30-107">Create a new non-security policy with targeting groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ea30-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3ea30-108">Prerequisites</span></span>
<span data-ttu-id="3ea30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ea30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ea30-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ea30-111">Permission type</span></span>|<span data-ttu-id="3ea30-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3ea30-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ea30-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ea30-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3ea30-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ea30-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3ea30-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ea30-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ea30-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ea30-116">Not supported.</span></span>|
|<span data-ttu-id="3ea30-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ea30-117">Application</span></span>|<span data-ttu-id="3ea30-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ea30-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ea30-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ea30-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3ea30-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ea30-120">Request headers</span></span>
|<span data-ttu-id="3ea30-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3ea30-121">Header</span></span>|<span data-ttu-id="3ea30-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3ea30-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ea30-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ea30-123">Authorization</span></span>|<span data-ttu-id="3ea30-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ea30-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ea30-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3ea30-125">Accept</span></span>|<span data-ttu-id="3ea30-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ea30-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ea30-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ea30-127">Request body</span></span>
<span data-ttu-id="3ea30-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsOfficeClientConfiguration.](../resources/intune-cirrus-windowsofficeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea30-128">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="3ea30-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3ea30-129">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="3ea30-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ea30-130">Property</span></span>|<span data-ttu-id="3ea30-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ea30-131">Type</span></span>|<span data-ttu-id="3ea30-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ea30-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ea30-133">id</span><span class="sxs-lookup"><span data-stu-id="3ea30-133">id</span></span>|<span data-ttu-id="3ea30-134">String</span><span class="sxs-lookup"><span data-stu-id="3ea30-134">String</span></span>|<span data-ttu-id="3ea30-135">ID da política de configuração do cliente do office.</span><span class="sxs-lookup"><span data-stu-id="3ea30-135">Id of the office client configuration policy.</span></span> <span data-ttu-id="3ea30-136">Herdado [do officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea30-136">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3ea30-137">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="3ea30-137">userPreferencePayload</span></span>|<span data-ttu-id="3ea30-138">Stream</span><span class="sxs-lookup"><span data-stu-id="3ea30-138">Stream</span></span>|<span data-ttu-id="3ea30-139">Configurações de preferência Cadeia de caracteres JSON no formato binário, esses valores podem ser substituídos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="3ea30-139">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="3ea30-140">Herdado [do officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea30-140">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3ea30-141">policyPayload</span><span class="sxs-lookup"><span data-stu-id="3ea30-141">policyPayload</span></span>|<span data-ttu-id="3ea30-142">Stream</span><span class="sxs-lookup"><span data-stu-id="3ea30-142">Stream</span></span>|<span data-ttu-id="3ea30-143">Configurações de política Cadeia de caracteres JSON em formato binário, esses valores não podem ser alterados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="3ea30-143">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="3ea30-144">Herdado [do officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea30-144">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3ea30-145">descrição</span><span class="sxs-lookup"><span data-stu-id="3ea30-145">description</span></span>|<span data-ttu-id="3ea30-146">String</span><span class="sxs-lookup"><span data-stu-id="3ea30-146">String</span></span>|<span data-ttu-id="3ea30-147">O administrador forneceu a descrição da política de configuração do cliente do office.</span><span class="sxs-lookup"><span data-stu-id="3ea30-147">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="3ea30-148">Herdado [do officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea30-148">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3ea30-149">displayName</span><span class="sxs-lookup"><span data-stu-id="3ea30-149">displayName</span></span>|<span data-ttu-id="3ea30-150">String</span><span class="sxs-lookup"><span data-stu-id="3ea30-150">String</span></span>|<span data-ttu-id="3ea30-151">O administrador forneceu o nome da política de configuração do cliente do office.</span><span class="sxs-lookup"><span data-stu-id="3ea30-151">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="3ea30-152">Herdado [do officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea30-152">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3ea30-153">assignments</span><span class="sxs-lookup"><span data-stu-id="3ea30-153">assignments</span></span>|<span data-ttu-id="3ea30-154">[Coleção officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3ea30-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3ea30-155">A lista de atribuições de grupo para a política..</span><span class="sxs-lookup"><span data-stu-id="3ea30-155">The list of group assignments for the policy..</span></span> <span data-ttu-id="3ea30-156">Herdado [do officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea30-156">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3ea30-157">prioridade</span><span class="sxs-lookup"><span data-stu-id="3ea30-157">priority</span></span>|<span data-ttu-id="3ea30-158">Int32</span><span class="sxs-lookup"><span data-stu-id="3ea30-158">Int32</span></span>|<span data-ttu-id="3ea30-159">O valor de prioridade deve ser o valor exclusivo para cada política em um locatário e será usado para resolução de conflitos, valores mais baixos a prioridade média é alta.</span><span class="sxs-lookup"><span data-stu-id="3ea30-159">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="3ea30-160">Herdado [do officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea30-160">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3ea30-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ea30-161">lastModifiedDateTime</span></span>|<span data-ttu-id="3ea30-162">DateTime</span><span class="sxs-lookup"><span data-stu-id="3ea30-162">DateTime</span></span>|<span data-ttu-id="3ea30-163">Carimbo de data da última modificação da política.</span><span class="sxs-lookup"><span data-stu-id="3ea30-163">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="3ea30-164">Herdado [do officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea30-164">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3ea30-165">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="3ea30-165">userCheckinSummary</span></span>|[<span data-ttu-id="3ea30-166">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="3ea30-166">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="3ea30-167">Resumo de check-in do usuário para a política.</span><span class="sxs-lookup"><span data-stu-id="3ea30-167">User check-in summary for the policy.</span></span> <span data-ttu-id="3ea30-168">Herdado [do officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea30-168">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3ea30-169">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="3ea30-169">checkinStatuses</span></span>|<span data-ttu-id="3ea30-170">[Coleção officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="3ea30-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="3ea30-171">Lista de status de check-in do cliente do office.</span><span class="sxs-lookup"><span data-stu-id="3ea30-171">List of office Client check-in status.</span></span> <span data-ttu-id="3ea30-172">Herdado [do officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea30-172">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="3ea30-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ea30-173">Response</span></span>
<span data-ttu-id="3ea30-174">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ea30-174">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ea30-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ea30-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ea30-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ea30-176">Request</span></span>
<span data-ttu-id="3ea30-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ea30-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3ea30-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ea30-178">Response</span></span>
<span data-ttu-id="3ea30-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ea30-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




