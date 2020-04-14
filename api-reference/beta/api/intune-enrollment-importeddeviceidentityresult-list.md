---
title: Listar importedDeviceIdentityResults
description: Listar Propriedades e relações dos objetos importedDeviceIdentityResult.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8009b7b53b173ce4e62b0f606b780b2ef0db7c11
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450957"
---
# <a name="list-importeddeviceidentityresults"></a><span data-ttu-id="e7a6d-103">Listar importedDeviceIdentityResults</span><span class="sxs-lookup"><span data-stu-id="e7a6d-103">List importedDeviceIdentityResults</span></span>

<span data-ttu-id="e7a6d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7a6d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7a6d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e7a6d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7a6d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e7a6d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7a6d-107">Listar Propriedades e relações dos objetos [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="e7a6d-107">List properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7a6d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7a6d-108">Prerequisites</span></span>
<span data-ttu-id="e7a6d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7a6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7a6d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7a6d-111">Permission type</span></span>|<span data-ttu-id="e7a6d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e7a6d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7a6d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7a6d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7a6d-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7a6d-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e7a6d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7a6d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7a6d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7a6d-116">Not supported.</span></span>|
|<span data-ttu-id="e7a6d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7a6d-117">Application</span></span>|<span data-ttu-id="e7a6d-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7a6d-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7a6d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7a6d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="e7a6d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7a6d-120">Request headers</span></span>
|<span data-ttu-id="e7a6d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7a6d-121">Header</span></span>|<span data-ttu-id="e7a6d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e7a6d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7a6d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7a6d-123">Authorization</span></span>|<span data-ttu-id="e7a6d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7a6d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7a6d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e7a6d-125">Accept</span></span>|<span data-ttu-id="e7a6d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7a6d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7a6d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7a6d-127">Request body</span></span>
<span data-ttu-id="e7a6d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7a6d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7a6d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7a6d-129">Response</span></span>
<span data-ttu-id="e7a6d-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7a6d-130">If successful, this method returns a `200 OK` response code and a collection of [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7a6d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7a6d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7a6d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7a6d-132">Request</span></span>
<span data-ttu-id="e7a6d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7a6d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="e7a6d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7a6d-134">Response</span></span>
<span data-ttu-id="e7a6d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7a6d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 606

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
      "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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



