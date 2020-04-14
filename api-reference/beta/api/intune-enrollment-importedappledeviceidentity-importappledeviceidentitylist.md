---
title: Ação importAppleDeviceIdentityList
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 444f895caa9d420fb6c1bad55faefc1dcd550d08
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451187"
---
# <a name="importappledeviceidentitylist-action"></a><span data-ttu-id="96332-103">Ação importAppleDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="96332-103">importAppleDeviceIdentityList action</span></span>

<span data-ttu-id="96332-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96332-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96332-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="96332-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96332-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96332-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96332-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="96332-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96332-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="96332-108">Prerequisites</span></span>
<span data-ttu-id="96332-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96332-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96332-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96332-111">Permission type</span></span>|<span data-ttu-id="96332-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="96332-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96332-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96332-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96332-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96332-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="96332-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96332-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96332-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96332-116">Not supported.</span></span>|
|<span data-ttu-id="96332-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96332-117">Application</span></span>|<span data-ttu-id="96332-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96332-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96332-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96332-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="96332-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96332-120">Request headers</span></span>
|<span data-ttu-id="96332-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96332-121">Header</span></span>|<span data-ttu-id="96332-122">Valor</span><span class="sxs-lookup"><span data-stu-id="96332-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96332-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="96332-123">Authorization</span></span>|<span data-ttu-id="96332-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96332-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96332-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="96332-125">Accept</span></span>|<span data-ttu-id="96332-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96332-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96332-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96332-127">Request body</span></span>
<span data-ttu-id="96332-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="96332-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="96332-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="96332-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="96332-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96332-130">Property</span></span>|<span data-ttu-id="96332-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="96332-131">Type</span></span>|<span data-ttu-id="96332-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="96332-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96332-133">importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="96332-133">importedAppleDeviceIdentities</span></span>|<span data-ttu-id="96332-134">coleção [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="96332-134">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="96332-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="96332-135">Not yet documented</span></span>|
|<span data-ttu-id="96332-136">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="96332-136">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="96332-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="96332-137">Boolean</span></span>|<span data-ttu-id="96332-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="96332-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="96332-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="96332-139">Response</span></span>
<span data-ttu-id="96332-140">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96332-140">If successful, this action returns a `200 OK` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96332-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96332-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="96332-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96332-142">Request</span></span>
<span data-ttu-id="96332-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96332-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList

Content-type: application/json
Content-length: 782

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
      "isDeleted": true,
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

### <a name="response"></a><span data-ttu-id="96332-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="96332-144">Response</span></span>
<span data-ttu-id="96332-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96332-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 741

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
      "isDeleted": true,
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



