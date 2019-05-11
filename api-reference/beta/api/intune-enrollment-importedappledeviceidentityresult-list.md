---
title: Listar importedAppleDeviceIdentityResults
description: Listar Propriedades e relações dos objetos importedAppleDeviceIdentityResult.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ff70a47048a4228092052bfc3364fa982b59a724
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908641"
---
# <a name="list-importedappledeviceidentityresults"></a><span data-ttu-id="8935b-103">Listar importedAppleDeviceIdentityResults</span><span class="sxs-lookup"><span data-stu-id="8935b-103">List importedAppleDeviceIdentityResults</span></span>

> <span data-ttu-id="8935b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8935b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8935b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8935b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8935b-106">Listar Propriedades e relações dos objetos [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="8935b-106">List properties and relationships of the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8935b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8935b-107">Prerequisites</span></span>
<span data-ttu-id="8935b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8935b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8935b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8935b-110">Permission type</span></span>|<span data-ttu-id="8935b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8935b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8935b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8935b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8935b-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8935b-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8935b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8935b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8935b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8935b-115">Not supported.</span></span>|
|<span data-ttu-id="8935b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8935b-116">Application</span></span>|<span data-ttu-id="8935b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8935b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8935b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8935b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="8935b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8935b-119">Request headers</span></span>
|<span data-ttu-id="8935b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8935b-120">Header</span></span>|<span data-ttu-id="8935b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8935b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8935b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8935b-122">Authorization</span></span>|<span data-ttu-id="8935b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8935b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8935b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8935b-124">Accept</span></span>|<span data-ttu-id="8935b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8935b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8935b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8935b-126">Request body</span></span>
<span data-ttu-id="8935b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8935b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8935b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8935b-128">Response</span></span>
<span data-ttu-id="8935b-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8935b-129">If successful, this method returns a `200 OK` response code and a collection of [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8935b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8935b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8935b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8935b-131">Request</span></span>
<span data-ttu-id="8935b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8935b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="8935b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8935b-133">Response</span></span>
<span data-ttu-id="8935b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8935b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




