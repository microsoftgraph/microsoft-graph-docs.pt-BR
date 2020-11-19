---
title: Listar importedAppleDeviceIdentities
description: Listar Propriedades e relações dos objetos importedAppleDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d000035525ef8bd9da4f42b53fe9775038bea3c5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49263432"
---
# <a name="list-importedappledeviceidentities"></a><span data-ttu-id="2a03c-103">Listar importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="2a03c-103">List importedAppleDeviceIdentities</span></span>

<span data-ttu-id="2a03c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a03c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a03c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2a03c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a03c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2a03c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a03c-107">Listar Propriedades e relações dos objetos [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="2a03c-107">List properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a03c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2a03c-108">Prerequisites</span></span>
<span data-ttu-id="2a03c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a03c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a03c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a03c-111">Permission type</span></span>|<span data-ttu-id="2a03c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2a03c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a03c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a03c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a03c-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a03c-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2a03c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a03c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a03c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a03c-116">Not supported.</span></span>|
|<span data-ttu-id="2a03c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a03c-117">Application</span></span>|<span data-ttu-id="2a03c-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a03c-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a03c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a03c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="2a03c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a03c-120">Request headers</span></span>
|<span data-ttu-id="2a03c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a03c-121">Header</span></span>|<span data-ttu-id="2a03c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2a03c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a03c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a03c-123">Authorization</span></span>|<span data-ttu-id="2a03c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a03c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a03c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2a03c-125">Accept</span></span>|<span data-ttu-id="2a03c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a03c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a03c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a03c-127">Request body</span></span>
<span data-ttu-id="2a03c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2a03c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a03c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a03c-129">Response</span></span>
<span data-ttu-id="2a03c-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a03c-130">If successful, this method returns a `200 OK` response code and a collection of [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a03c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a03c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a03c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a03c-132">Request</span></span>
<span data-ttu-id="2a03c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a03c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="2a03c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a03c-134">Response</span></span>
<span data-ttu-id="2a03c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a03c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 712

{
  "value": [
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
  ]
}
```




