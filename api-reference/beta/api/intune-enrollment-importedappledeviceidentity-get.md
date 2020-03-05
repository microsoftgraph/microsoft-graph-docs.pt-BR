---
title: Obter importedAppleDeviceIdentity
description: Leia as propriedades e as relações do objeto importedAppleDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cebca7811657a17a6e62bdb3dce5e63559991d99
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42466791"
---
# <a name="get-importedappledeviceidentity"></a><span data-ttu-id="71313-103">Obter importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="71313-103">Get importedAppleDeviceIdentity</span></span>

<span data-ttu-id="71313-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="71313-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71313-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="71313-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71313-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71313-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71313-107">Leia as propriedades e as relações do objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="71313-107">Read properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71313-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="71313-108">Prerequisites</span></span>
<span data-ttu-id="71313-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71313-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71313-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71313-111">Permission type</span></span>|<span data-ttu-id="71313-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="71313-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71313-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71313-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71313-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="71313-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="71313-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71313-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71313-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71313-116">Not supported.</span></span>|
|<span data-ttu-id="71313-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71313-117">Application</span></span>|<span data-ttu-id="71313-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="71313-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71313-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71313-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71313-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="71313-120">Optional query parameters</span></span>
<span data-ttu-id="71313-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="71313-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71313-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71313-122">Request headers</span></span>
|<span data-ttu-id="71313-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="71313-123">Header</span></span>|<span data-ttu-id="71313-124">Valor</span><span class="sxs-lookup"><span data-stu-id="71313-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71313-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="71313-125">Authorization</span></span>|<span data-ttu-id="71313-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71313-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71313-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="71313-127">Accept</span></span>|<span data-ttu-id="71313-128">application/json</span><span class="sxs-lookup"><span data-stu-id="71313-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71313-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71313-129">Request body</span></span>
<span data-ttu-id="71313-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="71313-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71313-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="71313-131">Response</span></span>
<span data-ttu-id="71313-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71313-132">If successful, this method returns a `200 OK` response code and [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71313-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71313-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="71313-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71313-134">Request</span></span>
<span data-ttu-id="71313-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71313-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="71313-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="71313-136">Response</span></span>
<span data-ttu-id="71313-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71313-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 672

{
  "value": {
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
}
```





