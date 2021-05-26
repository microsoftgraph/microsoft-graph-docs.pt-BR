---
title: Atualizar windowsOfficeClientConfiguration
description: Corrigir uma carga de política não segura específica.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f62b8ebb03efcab5975fabe8d1c5606bd176af5
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666776"
---
# <a name="update-windowsofficeclientconfiguration"></a><span data-ttu-id="956bd-103">Atualizar windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="956bd-103">Update windowsOfficeClientConfiguration</span></span>

<span data-ttu-id="956bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="956bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="956bd-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="956bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="956bd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="956bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="956bd-107">Corrigir uma carga de política não segura específica.</span><span class="sxs-lookup"><span data-stu-id="956bd-107">Patch a specific non-security policy payload.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="956bd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="956bd-108">Prerequisites</span></span>
<span data-ttu-id="956bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="956bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="956bd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="956bd-111">Permission type</span></span>|<span data-ttu-id="956bd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="956bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="956bd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="956bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="956bd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="956bd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="956bd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="956bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="956bd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="956bd-116">Not supported.</span></span>|
|<span data-ttu-id="956bd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="956bd-117">Application</span></span>|<span data-ttu-id="956bd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="956bd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="956bd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="956bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="956bd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="956bd-120">Request headers</span></span>
|<span data-ttu-id="956bd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="956bd-121">Header</span></span>|<span data-ttu-id="956bd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="956bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="956bd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="956bd-123">Authorization</span></span>|<span data-ttu-id="956bd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="956bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="956bd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="956bd-125">Accept</span></span>|<span data-ttu-id="956bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="956bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="956bd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="956bd-127">Request body</span></span>
<span data-ttu-id="956bd-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsOfficeClientConfiguration.](../resources/intune-cirrus-windowsofficeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="956bd-128">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="956bd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="956bd-129">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="956bd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="956bd-130">Property</span></span>|<span data-ttu-id="956bd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="956bd-131">Type</span></span>|<span data-ttu-id="956bd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="956bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="956bd-133">id</span><span class="sxs-lookup"><span data-stu-id="956bd-133">id</span></span>|<span data-ttu-id="956bd-134">String</span><span class="sxs-lookup"><span data-stu-id="956bd-134">String</span></span>|<span data-ttu-id="956bd-135">Ainda não documentado Herdado do [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="956bd-135">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="956bd-136">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="956bd-136">userPreferencePayload</span></span>|<span data-ttu-id="956bd-137">Stream</span><span class="sxs-lookup"><span data-stu-id="956bd-137">Stream</span></span>|<span data-ttu-id="956bd-138">Ainda não documentado Herdado do [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="956bd-138">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="956bd-139">policyPayload</span><span class="sxs-lookup"><span data-stu-id="956bd-139">policyPayload</span></span>|<span data-ttu-id="956bd-140">Stream</span><span class="sxs-lookup"><span data-stu-id="956bd-140">Stream</span></span>|<span data-ttu-id="956bd-141">Ainda não documentado Herdado do [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="956bd-141">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="956bd-142">descrição</span><span class="sxs-lookup"><span data-stu-id="956bd-142">description</span></span>|<span data-ttu-id="956bd-143">String</span><span class="sxs-lookup"><span data-stu-id="956bd-143">String</span></span>|<span data-ttu-id="956bd-144">Ainda não documentado Herdado do [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="956bd-144">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="956bd-145">displayName</span><span class="sxs-lookup"><span data-stu-id="956bd-145">displayName</span></span>|<span data-ttu-id="956bd-146">String</span><span class="sxs-lookup"><span data-stu-id="956bd-146">String</span></span>|<span data-ttu-id="956bd-147">Ainda não documentado Herdado do [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="956bd-147">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="956bd-148">prioridade</span><span class="sxs-lookup"><span data-stu-id="956bd-148">priority</span></span>|<span data-ttu-id="956bd-149">Int32</span><span class="sxs-lookup"><span data-stu-id="956bd-149">Int32</span></span>|<span data-ttu-id="956bd-150">Ainda não documentado Herdado do [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="956bd-150">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="956bd-151">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="956bd-151">userCheckinSummary</span></span>|[<span data-ttu-id="956bd-152">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="956bd-152">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="956bd-153">Ainda não documentado Herdado do [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="956bd-153">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="956bd-154">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="956bd-154">checkinStatuses</span></span>|<span data-ttu-id="956bd-155">[Coleção officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="956bd-155">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="956bd-156">Ainda não documentado Herdado do [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="956bd-156">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="956bd-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="956bd-157">Response</span></span>
<span data-ttu-id="956bd-158">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="956bd-158">If successful, this method returns a `200 OK` response code and an updated [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="956bd-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="956bd-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="956bd-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="956bd-160">Request</span></span>
<span data-ttu-id="956bd-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="956bd-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="956bd-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="956bd-162">Response</span></span>
<span data-ttu-id="956bd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="956bd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




