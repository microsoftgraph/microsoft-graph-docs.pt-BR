---
title: Ação importAppleDeviceIdentityList
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 719ce29b6a45bd6f7fc4029944b6aff8d3842626
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149902"
---
# <a name="importappledeviceidentitylist-action"></a><span data-ttu-id="3abfe-103">Ação importAppleDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="3abfe-103">importAppleDeviceIdentityList action</span></span>

<span data-ttu-id="3abfe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3abfe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3abfe-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3abfe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3abfe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3abfe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3abfe-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3abfe-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3abfe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3abfe-108">Prerequisites</span></span>
<span data-ttu-id="3abfe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3abfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3abfe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3abfe-111">Permission type</span></span>|<span data-ttu-id="3abfe-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3abfe-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3abfe-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3abfe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3abfe-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3abfe-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3abfe-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3abfe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3abfe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3abfe-116">Not supported.</span></span>|
|<span data-ttu-id="3abfe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3abfe-117">Application</span></span>|<span data-ttu-id="3abfe-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3abfe-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3abfe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3abfe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="3abfe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3abfe-120">Request headers</span></span>
|<span data-ttu-id="3abfe-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3abfe-121">Header</span></span>|<span data-ttu-id="3abfe-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3abfe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3abfe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3abfe-123">Authorization</span></span>|<span data-ttu-id="3abfe-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3abfe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3abfe-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3abfe-125">Accept</span></span>|<span data-ttu-id="3abfe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3abfe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3abfe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3abfe-127">Request body</span></span>
<span data-ttu-id="3abfe-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3abfe-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3abfe-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="3abfe-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3abfe-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3abfe-130">Property</span></span>|<span data-ttu-id="3abfe-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3abfe-131">Type</span></span>|<span data-ttu-id="3abfe-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3abfe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3abfe-133">importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="3abfe-133">importedAppleDeviceIdentities</span></span>|<span data-ttu-id="3abfe-134">[Coleção importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="3abfe-134">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="3abfe-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3abfe-135">Not yet documented</span></span>|
|<span data-ttu-id="3abfe-136">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="3abfe-136">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="3abfe-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="3abfe-137">Boolean</span></span>|<span data-ttu-id="3abfe-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3abfe-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3abfe-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3abfe-139">Response</span></span>
<span data-ttu-id="3abfe-140">Se tiver êxito, essa ação retornará um código de `200 OK` resposta e uma coleção [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3abfe-140">If successful, this action returns a `200 OK` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3abfe-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3abfe-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="3abfe-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3abfe-142">Request</span></span>
<span data-ttu-id="3abfe-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3abfe-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3abfe-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="3abfe-144">Response</span></span>
<span data-ttu-id="3abfe-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3abfe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




