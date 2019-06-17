---
title: Listar importedAppleDeviceIdentities
description: Listar Propriedades e relações dos objetos importedAppleDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 837b14176441546fce084a4a1746fa43ce80af0d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34982032"
---
# <a name="list-importedappledeviceidentities"></a><span data-ttu-id="41724-103">Listar importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="41724-103">List importedAppleDeviceIdentities</span></span>

> <span data-ttu-id="41724-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="41724-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41724-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="41724-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41724-106">Listar Propriedades e relações dos objetos [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="41724-106">List properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41724-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="41724-107">Prerequisites</span></span>
<span data-ttu-id="41724-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41724-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41724-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41724-110">Permission type</span></span>|<span data-ttu-id="41724-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="41724-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41724-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41724-112">Delegated (work or school account)</span></span>|<span data-ttu-id="41724-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="41724-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="41724-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41724-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41724-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41724-115">Not supported.</span></span>|
|<span data-ttu-id="41724-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41724-116">Application</span></span>|<span data-ttu-id="41724-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41724-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41724-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41724-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="41724-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41724-119">Request headers</span></span>
|<span data-ttu-id="41724-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41724-120">Header</span></span>|<span data-ttu-id="41724-121">Valor</span><span class="sxs-lookup"><span data-stu-id="41724-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41724-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="41724-122">Authorization</span></span>|<span data-ttu-id="41724-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41724-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41724-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="41724-124">Accept</span></span>|<span data-ttu-id="41724-125">application/json</span><span class="sxs-lookup"><span data-stu-id="41724-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41724-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41724-126">Request body</span></span>
<span data-ttu-id="41724-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41724-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41724-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="41724-128">Response</span></span>
<span data-ttu-id="41724-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41724-129">If successful, this method returns a `200 OK` response code and a collection of [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41724-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41724-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="41724-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41724-131">Request</span></span>
<span data-ttu-id="41724-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41724-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="41724-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="41724-133">Response</span></span>
<span data-ttu-id="41724-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41724-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 686

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
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios"
    }
  ]
}
```





