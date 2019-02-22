---
title: Atualizar windowsOfficeClientConfiguration
description: Corrigir uma carga de política específica de não segurança.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d116d846b6540ea2b9e2a91f54a5abdfa81e2409
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139246"
---
# <a name="update-windowsofficeclientconfiguration"></a><span data-ttu-id="c645c-103">Atualizar windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="c645c-103">Update windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="c645c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c645c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c645c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c645c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c645c-106">Corrigir uma carga de política específica de não segurança.</span><span class="sxs-lookup"><span data-stu-id="c645c-106">Patch a specific non-security policy payload.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c645c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c645c-107">Prerequisites</span></span>
<span data-ttu-id="c645c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c645c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c645c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c645c-110">Permission type</span></span>|<span data-ttu-id="c645c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c645c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c645c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c645c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c645c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c645c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c645c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c645c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c645c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c645c-115">Not supported.</span></span>|
|<span data-ttu-id="c645c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c645c-116">Application</span></span>|<span data-ttu-id="c645c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c645c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c645c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c645c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="c645c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c645c-119">Request headers</span></span>
|<span data-ttu-id="c645c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c645c-120">Header</span></span>|<span data-ttu-id="c645c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c645c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c645c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c645c-122">Authorization</span></span>|<span data-ttu-id="c645c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c645c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c645c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c645c-124">Accept</span></span>|<span data-ttu-id="c645c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c645c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c645c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c645c-126">Request body</span></span>
<span data-ttu-id="c645c-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c645c-127">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="c645c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c645c-128">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="c645c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c645c-129">Property</span></span>|<span data-ttu-id="c645c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c645c-130">Type</span></span>|<span data-ttu-id="c645c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c645c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c645c-132">id</span><span class="sxs-lookup"><span data-stu-id="c645c-132">id</span></span>|<span data-ttu-id="c645c-133">String</span><span class="sxs-lookup"><span data-stu-id="c645c-133">String</span></span>|<span data-ttu-id="c645c-134">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c645c-134">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c645c-135">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="c645c-135">userPreferencePayload</span></span>|<span data-ttu-id="c645c-136">Stream</span><span class="sxs-lookup"><span data-stu-id="c645c-136">Stream</span></span>|<span data-ttu-id="c645c-137">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c645c-137">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c645c-138">policyPayload</span><span class="sxs-lookup"><span data-stu-id="c645c-138">policyPayload</span></span>|<span data-ttu-id="c645c-139">Stream</span><span class="sxs-lookup"><span data-stu-id="c645c-139">Stream</span></span>|<span data-ttu-id="c645c-140">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c645c-140">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c645c-141">description</span><span class="sxs-lookup"><span data-stu-id="c645c-141">description</span></span>|<span data-ttu-id="c645c-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c645c-142">String</span></span>|<span data-ttu-id="c645c-143">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c645c-143">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c645c-144">displayName</span><span class="sxs-lookup"><span data-stu-id="c645c-144">displayName</span></span>|<span data-ttu-id="c645c-145">String</span><span class="sxs-lookup"><span data-stu-id="c645c-145">String</span></span>|<span data-ttu-id="c645c-146">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c645c-146">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c645c-147">prioridade</span><span class="sxs-lookup"><span data-stu-id="c645c-147">priority</span></span>|<span data-ttu-id="c645c-148">Int32</span><span class="sxs-lookup"><span data-stu-id="c645c-148">Int32</span></span>|<span data-ttu-id="c645c-149">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c645c-149">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c645c-150">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="c645c-150">userCheckinSummary</span></span>|[<span data-ttu-id="c645c-151">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="c645c-151">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="c645c-152">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c645c-152">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c645c-153">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="c645c-153">checkinStatuses</span></span>|<span data-ttu-id="c645c-154">coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="c645c-154">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="c645c-155">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c645c-155">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c645c-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="c645c-156">Response</span></span>
<span data-ttu-id="c645c-157">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c645c-157">If successful, this method returns a `200 OK` response code and an updated [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c645c-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c645c-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="c645c-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c645c-159">Request</span></span>
<span data-ttu-id="c645c-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c645c-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c645c-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="c645c-161">Response</span></span>
<span data-ttu-id="c645c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c645c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



