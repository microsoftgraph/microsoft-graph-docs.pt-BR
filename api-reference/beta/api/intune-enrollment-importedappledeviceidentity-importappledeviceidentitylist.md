---
title: Ação importAppleDeviceIdentityList
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 717824e8d0731fe50cb00537e8c8d73647de3778
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532986"
---
# <a name="importappledeviceidentitylist-action"></a><span data-ttu-id="34e3f-103">Ação importAppleDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="34e3f-103">importAppleDeviceIdentityList action</span></span>

> <span data-ttu-id="34e3f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="34e3f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34e3f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34e3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34e3f-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="34e3f-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34e3f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="34e3f-107">Prerequisites</span></span>
<span data-ttu-id="34e3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34e3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34e3f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34e3f-110">Permission type</span></span>|<span data-ttu-id="34e3f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="34e3f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34e3f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34e3f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34e3f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34e3f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="34e3f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34e3f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34e3f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34e3f-115">Not supported.</span></span>|
|<span data-ttu-id="34e3f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34e3f-116">Application</span></span>|<span data-ttu-id="34e3f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34e3f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34e3f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34e3f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="34e3f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34e3f-119">Request headers</span></span>
|<span data-ttu-id="34e3f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34e3f-120">Header</span></span>|<span data-ttu-id="34e3f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="34e3f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34e3f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="34e3f-122">Authorization</span></span>|<span data-ttu-id="34e3f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34e3f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34e3f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="34e3f-124">Accept</span></span>|<span data-ttu-id="34e3f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34e3f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34e3f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34e3f-126">Request body</span></span>
<span data-ttu-id="34e3f-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="34e3f-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="34e3f-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="34e3f-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="34e3f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34e3f-129">Property</span></span>|<span data-ttu-id="34e3f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="34e3f-130">Type</span></span>|<span data-ttu-id="34e3f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="34e3f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34e3f-132">importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="34e3f-132">importedAppleDeviceIdentities</span></span>|<span data-ttu-id="34e3f-133">coleção [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="34e3f-133">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="34e3f-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="34e3f-134">Not yet documented</span></span>|
|<span data-ttu-id="34e3f-135">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="34e3f-135">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="34e3f-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="34e3f-136">Boolean</span></span>|<span data-ttu-id="34e3f-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="34e3f-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="34e3f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="34e3f-138">Response</span></span>
<span data-ttu-id="34e3f-139">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34e3f-139">If successful, this action returns a `200 OK` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34e3f-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34e3f-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="34e3f-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34e3f-141">Request</span></span>
<span data-ttu-id="34e3f-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34e3f-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="34e3f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="34e3f-143">Response</span></span>
<span data-ttu-id="34e3f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34e3f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





