---
title: Atualizar windowsOfficeClientConfiguration
description: Corrigir uma carga de política específica de não segurança.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0537ef70bcac1da1641873e87aef2a43357dd8bd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444389"
---
# <a name="update-windowsofficeclientconfiguration"></a><span data-ttu-id="bc99a-103">Atualizar windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="bc99a-103">Update windowsOfficeClientConfiguration</span></span>

<span data-ttu-id="bc99a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bc99a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc99a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bc99a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc99a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc99a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc99a-107">Corrigir uma carga de política específica de não segurança.</span><span class="sxs-lookup"><span data-stu-id="bc99a-107">Patch a specific non-security policy payload.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc99a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bc99a-108">Prerequisites</span></span>
<span data-ttu-id="bc99a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc99a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc99a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc99a-111">Permission type</span></span>|<span data-ttu-id="bc99a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bc99a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc99a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc99a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc99a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc99a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc99a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc99a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc99a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc99a-116">Not supported.</span></span>|
|<span data-ttu-id="bc99a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc99a-117">Application</span></span>|<span data-ttu-id="bc99a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc99a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc99a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc99a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="bc99a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc99a-120">Request headers</span></span>
|<span data-ttu-id="bc99a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bc99a-121">Header</span></span>|<span data-ttu-id="bc99a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bc99a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc99a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc99a-123">Authorization</span></span>|<span data-ttu-id="bc99a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc99a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc99a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bc99a-125">Accept</span></span>|<span data-ttu-id="bc99a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc99a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc99a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc99a-127">Request body</span></span>
<span data-ttu-id="bc99a-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bc99a-128">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="bc99a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bc99a-129">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="bc99a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc99a-130">Property</span></span>|<span data-ttu-id="bc99a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc99a-131">Type</span></span>|<span data-ttu-id="bc99a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc99a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc99a-133">id</span><span class="sxs-lookup"><span data-stu-id="bc99a-133">id</span></span>|<span data-ttu-id="bc99a-134">String</span><span class="sxs-lookup"><span data-stu-id="bc99a-134">String</span></span>|<span data-ttu-id="bc99a-135">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc99a-135">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="bc99a-136">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="bc99a-136">userPreferencePayload</span></span>|<span data-ttu-id="bc99a-137">Stream</span><span class="sxs-lookup"><span data-stu-id="bc99a-137">Stream</span></span>|<span data-ttu-id="bc99a-138">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc99a-138">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="bc99a-139">policyPayload</span><span class="sxs-lookup"><span data-stu-id="bc99a-139">policyPayload</span></span>|<span data-ttu-id="bc99a-140">Stream</span><span class="sxs-lookup"><span data-stu-id="bc99a-140">Stream</span></span>|<span data-ttu-id="bc99a-141">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc99a-141">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="bc99a-142">description</span><span class="sxs-lookup"><span data-stu-id="bc99a-142">description</span></span>|<span data-ttu-id="bc99a-143">String</span><span class="sxs-lookup"><span data-stu-id="bc99a-143">String</span></span>|<span data-ttu-id="bc99a-144">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc99a-144">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="bc99a-145">displayName</span><span class="sxs-lookup"><span data-stu-id="bc99a-145">displayName</span></span>|<span data-ttu-id="bc99a-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc99a-146">String</span></span>|<span data-ttu-id="bc99a-147">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc99a-147">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="bc99a-148">prioridade</span><span class="sxs-lookup"><span data-stu-id="bc99a-148">priority</span></span>|<span data-ttu-id="bc99a-149">Int32</span><span class="sxs-lookup"><span data-stu-id="bc99a-149">Int32</span></span>|<span data-ttu-id="bc99a-150">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc99a-150">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="bc99a-151">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="bc99a-151">userCheckinSummary</span></span>|[<span data-ttu-id="bc99a-152">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="bc99a-152">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="bc99a-153">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc99a-153">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="bc99a-154">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="bc99a-154">checkinStatuses</span></span>|<span data-ttu-id="bc99a-155">coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="bc99a-155">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="bc99a-156">Ainda não documentado herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc99a-156">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="bc99a-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc99a-157">Response</span></span>
<span data-ttu-id="bc99a-158">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc99a-158">If successful, this method returns a `200 OK` response code and an updated [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc99a-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc99a-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc99a-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc99a-160">Request</span></span>
<span data-ttu-id="bc99a-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc99a-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bc99a-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc99a-162">Response</span></span>
<span data-ttu-id="bc99a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc99a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





