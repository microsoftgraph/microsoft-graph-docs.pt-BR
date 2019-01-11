---
title: Atualizar windowsOfficeClientConfiguration
description: Patch uma carga de diretiva específicas do não relacionadas à segurança.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e13228c6fc467fa49b740c02b4b7068efb1ec42e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863870"
---
# <a name="update-windowsofficeclientconfiguration"></a><span data-ttu-id="ebcd2-103">Atualizar windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="ebcd2-103">Update windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="ebcd2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ebcd2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebcd2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ebcd2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ebcd2-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ebcd2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebcd2-107">Patch uma carga de diretiva específicas do não relacionadas à segurança.</span><span class="sxs-lookup"><span data-stu-id="ebcd2-107">Patch a specific non-security policy payload.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ebcd2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ebcd2-108">Prerequisites</span></span>
<span data-ttu-id="ebcd2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebcd2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebcd2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebcd2-111">Permission type</span></span>|<span data-ttu-id="ebcd2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ebcd2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebcd2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebcd2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ebcd2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebcd2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ebcd2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebcd2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebcd2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebcd2-116">Not supported.</span></span>|
|<span data-ttu-id="ebcd2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebcd2-117">Application</span></span>|<span data-ttu-id="ebcd2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebcd2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebcd2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebcd2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="ebcd2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebcd2-120">Request headers</span></span>
|<span data-ttu-id="ebcd2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ebcd2-121">Header</span></span>|<span data-ttu-id="ebcd2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ebcd2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebcd2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebcd2-123">Authorization</span></span>|<span data-ttu-id="ebcd2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebcd2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebcd2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ebcd2-125">Accept</span></span>|<span data-ttu-id="ebcd2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ebcd2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebcd2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebcd2-127">Request body</span></span>
<span data-ttu-id="ebcd2-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ebcd2-128">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="ebcd2-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ebcd2-129">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="ebcd2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebcd2-130">Property</span></span>|<span data-ttu-id="ebcd2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebcd2-131">Type</span></span>|<span data-ttu-id="ebcd2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebcd2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebcd2-133">id</span><span class="sxs-lookup"><span data-stu-id="ebcd2-133">id</span></span>|<span data-ttu-id="ebcd2-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebcd2-134">String</span></span>|<span data-ttu-id="ebcd2-135">Ainda não documentado Inherited de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebcd2-135">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ebcd2-136">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="ebcd2-136">userPreferencePayload</span></span>|<span data-ttu-id="ebcd2-137">Stream</span><span class="sxs-lookup"><span data-stu-id="ebcd2-137">Stream</span></span>|<span data-ttu-id="ebcd2-138">Ainda não documentado Inherited de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebcd2-138">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ebcd2-139">policyPayload</span><span class="sxs-lookup"><span data-stu-id="ebcd2-139">policyPayload</span></span>|<span data-ttu-id="ebcd2-140">Stream</span><span class="sxs-lookup"><span data-stu-id="ebcd2-140">Stream</span></span>|<span data-ttu-id="ebcd2-141">Ainda não documentado Inherited de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebcd2-141">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ebcd2-142">description</span><span class="sxs-lookup"><span data-stu-id="ebcd2-142">description</span></span>|<span data-ttu-id="ebcd2-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebcd2-143">String</span></span>|<span data-ttu-id="ebcd2-144">Ainda não documentado Inherited de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebcd2-144">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ebcd2-145">displayName</span><span class="sxs-lookup"><span data-stu-id="ebcd2-145">displayName</span></span>|<span data-ttu-id="ebcd2-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebcd2-146">String</span></span>|<span data-ttu-id="ebcd2-147">Ainda não documentado Inherited de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebcd2-147">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ebcd2-148">prioridade</span><span class="sxs-lookup"><span data-stu-id="ebcd2-148">priority</span></span>|<span data-ttu-id="ebcd2-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ebcd2-149">Int32</span></span>|<span data-ttu-id="ebcd2-150">Ainda não documentado Inherited de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebcd2-150">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ebcd2-151">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="ebcd2-151">userCheckinSummary</span></span>|[<span data-ttu-id="ebcd2-152">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="ebcd2-152">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="ebcd2-153">Ainda não documentado Inherited de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebcd2-153">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ebcd2-154">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="ebcd2-154">checkinStatuses</span></span>|<span data-ttu-id="ebcd2-155">coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="ebcd2-155">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="ebcd2-156">Ainda não documentado Inherited de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebcd2-156">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ebcd2-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebcd2-157">Response</span></span>
<span data-ttu-id="ebcd2-158">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebcd2-158">If successful, this method returns a `200 OK` response code and an updated [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebcd2-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebcd2-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="ebcd2-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebcd2-160">Request</span></span>
<span data-ttu-id="ebcd2-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebcd2-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ebcd2-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebcd2-162">Response</span></span>
<span data-ttu-id="ebcd2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ebcd2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



