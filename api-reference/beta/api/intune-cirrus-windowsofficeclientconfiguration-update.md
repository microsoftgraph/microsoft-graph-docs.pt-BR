---
title: Atualizar windowsOfficeClientConfiguration
description: Corrigir uma carga de política específica de não segurança.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 09c663609e80ac3db7e85fe3f2e35cac33745bd7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36322160"
---
# <a name="update-windowsofficeclientconfiguration"></a><span data-ttu-id="545e7-103">Atualizar windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="545e7-103">Update windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="545e7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="545e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="545e7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="545e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="545e7-106">Corrigir uma carga de política específica de não segurança.</span><span class="sxs-lookup"><span data-stu-id="545e7-106">Patch a specific non-security policy payload.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="545e7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="545e7-107">Prerequisites</span></span>
<span data-ttu-id="545e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="545e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="545e7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="545e7-110">Permission type</span></span>|<span data-ttu-id="545e7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="545e7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="545e7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="545e7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="545e7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="545e7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="545e7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="545e7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="545e7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="545e7-115">Not supported.</span></span>|
|<span data-ttu-id="545e7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="545e7-116">Application</span></span>|<span data-ttu-id="545e7-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="545e7-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="545e7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="545e7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="545e7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="545e7-119">Request headers</span></span>
|<span data-ttu-id="545e7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="545e7-120">Header</span></span>|<span data-ttu-id="545e7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="545e7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="545e7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="545e7-122">Authorization</span></span>|<span data-ttu-id="545e7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="545e7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="545e7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="545e7-124">Accept</span></span>|<span data-ttu-id="545e7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="545e7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="545e7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="545e7-126">Request body</span></span>
<span data-ttu-id="545e7-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="545e7-127">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="545e7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="545e7-128">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="545e7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="545e7-129">Property</span></span>|<span data-ttu-id="545e7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="545e7-130">Type</span></span>|<span data-ttu-id="545e7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="545e7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="545e7-132">id</span><span class="sxs-lookup"><span data-stu-id="545e7-132">id</span></span>|<span data-ttu-id="545e7-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="545e7-133">String</span></span>|<span data-ttu-id="545e7-134">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545e7-134">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="545e7-135">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="545e7-135">userPreferencePayload</span></span>|<span data-ttu-id="545e7-136">Fluxo</span><span class="sxs-lookup"><span data-stu-id="545e7-136">Stream</span></span>|<span data-ttu-id="545e7-137">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545e7-137">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="545e7-138">policyPayload</span><span class="sxs-lookup"><span data-stu-id="545e7-138">policyPayload</span></span>|<span data-ttu-id="545e7-139">Fluxo</span><span class="sxs-lookup"><span data-stu-id="545e7-139">Stream</span></span>|<span data-ttu-id="545e7-140">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545e7-140">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="545e7-141">descrição</span><span class="sxs-lookup"><span data-stu-id="545e7-141">description</span></span>|<span data-ttu-id="545e7-142">String</span><span class="sxs-lookup"><span data-stu-id="545e7-142">String</span></span>|<span data-ttu-id="545e7-143">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545e7-143">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="545e7-144">displayName</span><span class="sxs-lookup"><span data-stu-id="545e7-144">displayName</span></span>|<span data-ttu-id="545e7-145">String</span><span class="sxs-lookup"><span data-stu-id="545e7-145">String</span></span>|<span data-ttu-id="545e7-146">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545e7-146">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="545e7-147">prioridade</span><span class="sxs-lookup"><span data-stu-id="545e7-147">priority</span></span>|<span data-ttu-id="545e7-148">Int32</span><span class="sxs-lookup"><span data-stu-id="545e7-148">Int32</span></span>|<span data-ttu-id="545e7-149">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545e7-149">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="545e7-150">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="545e7-150">userCheckinSummary</span></span>|[<span data-ttu-id="545e7-151">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="545e7-151">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="545e7-152">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545e7-152">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="545e7-153">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="545e7-153">checkinStatuses</span></span>|<span data-ttu-id="545e7-154">coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="545e7-154">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="545e7-155">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545e7-155">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="545e7-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="545e7-156">Response</span></span>
<span data-ttu-id="545e7-157">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="545e7-157">If successful, this method returns a `200 OK` response code and an updated [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="545e7-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="545e7-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="545e7-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="545e7-159">Request</span></span>
<span data-ttu-id="545e7-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="545e7-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="545e7-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="545e7-161">Response</span></span>
<span data-ttu-id="545e7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="545e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






