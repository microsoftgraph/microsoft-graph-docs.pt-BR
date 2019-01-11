---
title: ação de importAppleDeviceIdentityList
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 75a40be8d2ea3ddafadb78f95662dcadf7a9ac01
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890598"
---
# <a name="importappledeviceidentitylist-action"></a><span data-ttu-id="5979e-103">ação de importAppleDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="5979e-103">importAppleDeviceIdentityList action</span></span>

> <span data-ttu-id="5979e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5979e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5979e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5979e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5979e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5979e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5979e-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5979e-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5979e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5979e-108">Prerequisites</span></span>
<span data-ttu-id="5979e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5979e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5979e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5979e-111">Permission type</span></span>|<span data-ttu-id="5979e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5979e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5979e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5979e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5979e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5979e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5979e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5979e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5979e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5979e-116">Not supported.</span></span>|
|<span data-ttu-id="5979e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5979e-117">Application</span></span>|<span data-ttu-id="5979e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5979e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5979e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5979e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="5979e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5979e-120">Request headers</span></span>
|<span data-ttu-id="5979e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5979e-121">Header</span></span>|<span data-ttu-id="5979e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5979e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5979e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5979e-123">Authorization</span></span>|<span data-ttu-id="5979e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5979e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5979e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5979e-125">Accept</span></span>|<span data-ttu-id="5979e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5979e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5979e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5979e-127">Request body</span></span>
<span data-ttu-id="5979e-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="5979e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5979e-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="5979e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5979e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5979e-130">Property</span></span>|<span data-ttu-id="5979e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5979e-131">Type</span></span>|<span data-ttu-id="5979e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5979e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5979e-133">importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="5979e-133">importedAppleDeviceIdentities</span></span>|<span data-ttu-id="5979e-134">coleção [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5979e-134">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="5979e-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5979e-135">Not yet documented</span></span>|
|<span data-ttu-id="5979e-136">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="5979e-136">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="5979e-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="5979e-137">Boolean</span></span>|<span data-ttu-id="5979e-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5979e-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5979e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5979e-139">Response</span></span>
<span data-ttu-id="5979e-140">Se tiver êxito, essa ação retornará um `200 OK` código de resposta e um conjunto de [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5979e-140">If successful, this action returns a `200 OK` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5979e-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5979e-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="5979e-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5979e-142">Request</span></span>
<span data-ttu-id="5979e-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5979e-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList

Content-type: application/json
Content-length: 756

{
  "importedAppleDeviceIdentities": [
    {
      "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
      "id": "352e3c2f-3c2f-352e-2f3c-2e352f3c2e35",
      "serialNumber": "Serial Number value",
      "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
      "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
      "isSupervised": true,
      "discoverySource": "adminImport",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios"
    }
  ],
  "overwriteImportedDeviceIdentities": true
}
```

### <a name="response"></a><span data-ttu-id="5979e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="5979e-144">Response</span></span>
<span data-ttu-id="5979e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5979e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 715

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
      "id": "557cfb4a-fb4a-557c-4afb-7c554afb7c55",
      "serialNumber": "Serial Number value",
      "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
      "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
      "isSupervised": true,
      "discoverySource": "adminImport",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios",
      "status": true
    }
  ]
}
```





