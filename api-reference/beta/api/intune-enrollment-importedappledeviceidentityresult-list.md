---
title: Listar importedAppleDeviceIdentityResults
description: Listar Propriedades e relações dos objetos importedAppleDeviceIdentityResult.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e19413bcbf554c58fbfe65311569ea0e38ad0343
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729128"
---
# <a name="list-importedappledeviceidentityresults"></a><span data-ttu-id="e8f77-103">Listar importedAppleDeviceIdentityResults</span><span class="sxs-lookup"><span data-stu-id="e8f77-103">List importedAppleDeviceIdentityResults</span></span>

<span data-ttu-id="e8f77-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8f77-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8f77-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e8f77-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8f77-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8f77-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8f77-107">Listar Propriedades e relações dos objetos [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="e8f77-107">List properties and relationships of the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8f77-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e8f77-108">Prerequisites</span></span>
<span data-ttu-id="e8f77-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8f77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8f77-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8f77-111">Permission type</span></span>|<span data-ttu-id="e8f77-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e8f77-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8f77-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8f77-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8f77-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8f77-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e8f77-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8f77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8f77-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8f77-116">Not supported.</span></span>|
|<span data-ttu-id="e8f77-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8f77-117">Application</span></span>|<span data-ttu-id="e8f77-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8f77-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8f77-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8f77-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="e8f77-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8f77-120">Request headers</span></span>
|<span data-ttu-id="e8f77-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8f77-121">Header</span></span>|<span data-ttu-id="e8f77-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e8f77-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8f77-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8f77-123">Authorization</span></span>|<span data-ttu-id="e8f77-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8f77-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8f77-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e8f77-125">Accept</span></span>|<span data-ttu-id="e8f77-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8f77-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8f77-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8f77-127">Request body</span></span>
<span data-ttu-id="e8f77-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8f77-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8f77-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8f77-129">Response</span></span>
<span data-ttu-id="e8f77-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8f77-130">If successful, this method returns a `200 OK` response code and a collection of [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8f77-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8f77-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8f77-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8f77-132">Request</span></span>
<span data-ttu-id="e8f77-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8f77-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="e8f77-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8f77-134">Response</span></span>
<span data-ttu-id="e8f77-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8f77-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





