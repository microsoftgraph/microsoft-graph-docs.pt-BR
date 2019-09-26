---
title: Obter importedAppleDeviceIdentity
description: Leia as propriedades e as relações do objeto importedAppleDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a9238d8ef8b05eca09fba91c21f52b63c04ac325
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37185074"
---
# <a name="get-importedappledeviceidentity"></a><span data-ttu-id="d768d-103">Obter importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="d768d-103">Get importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="d768d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d768d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d768d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d768d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d768d-106">Leia as propriedades e as relações do objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="d768d-106">Read properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d768d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d768d-107">Prerequisites</span></span>
<span data-ttu-id="d768d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d768d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d768d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d768d-110">Permission type</span></span>|<span data-ttu-id="d768d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d768d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d768d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d768d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d768d-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d768d-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d768d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d768d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d768d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d768d-115">Not supported.</span></span>|
|<span data-ttu-id="d768d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d768d-116">Application</span></span>|<span data-ttu-id="d768d-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d768d-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d768d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d768d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d768d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d768d-119">Optional query parameters</span></span>
<span data-ttu-id="d768d-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d768d-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d768d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d768d-121">Request headers</span></span>
|<span data-ttu-id="d768d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d768d-122">Header</span></span>|<span data-ttu-id="d768d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d768d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d768d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d768d-124">Authorization</span></span>|<span data-ttu-id="d768d-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d768d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d768d-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d768d-126">Accept</span></span>|<span data-ttu-id="d768d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d768d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d768d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d768d-128">Request body</span></span>
<span data-ttu-id="d768d-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d768d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d768d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d768d-130">Response</span></span>
<span data-ttu-id="d768d-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d768d-131">If successful, this method returns a `200 OK` response code and [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d768d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d768d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d768d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d768d-133">Request</span></span>
<span data-ttu-id="d768d-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d768d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="d768d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d768d-135">Response</span></span>
<span data-ttu-id="d768d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d768d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 648

{
  "value": {
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
}
```




