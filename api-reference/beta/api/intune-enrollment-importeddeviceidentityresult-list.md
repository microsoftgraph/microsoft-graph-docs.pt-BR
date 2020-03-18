---
title: Listar importedDeviceIdentityResults
description: Listar Propriedades e relações dos objetos importedDeviceIdentityResult.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 26f7a19b95d7d33472563f7dd49db8345c7d8fc9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42805133"
---
# <a name="list-importeddeviceidentityresults"></a><span data-ttu-id="86972-103">Listar importedDeviceIdentityResults</span><span class="sxs-lookup"><span data-stu-id="86972-103">List importedDeviceIdentityResults</span></span>

> <span data-ttu-id="86972-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="86972-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86972-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86972-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86972-106">Listar Propriedades e relações dos objetos [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="86972-106">List properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86972-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86972-107">Prerequisites</span></span>
<span data-ttu-id="86972-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86972-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86972-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86972-110">Permission type</span></span>|<span data-ttu-id="86972-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="86972-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86972-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86972-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86972-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="86972-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="86972-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86972-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86972-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86972-115">Not supported.</span></span>|
|<span data-ttu-id="86972-116">Application</span><span class="sxs-lookup"><span data-stu-id="86972-116">Application</span></span>|<span data-ttu-id="86972-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="86972-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86972-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86972-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="86972-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86972-119">Request headers</span></span>
|<span data-ttu-id="86972-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86972-120">Header</span></span>|<span data-ttu-id="86972-121">Valor</span><span class="sxs-lookup"><span data-stu-id="86972-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86972-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="86972-122">Authorization</span></span>|<span data-ttu-id="86972-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86972-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86972-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="86972-124">Accept</span></span>|<span data-ttu-id="86972-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86972-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86972-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86972-126">Request body</span></span>
<span data-ttu-id="86972-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86972-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86972-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="86972-128">Response</span></span>
<span data-ttu-id="86972-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86972-129">If successful, this method returns a `200 OK` response code and a collection of [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86972-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86972-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="86972-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86972-131">Request</span></span>
<span data-ttu-id="86972-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86972-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="86972-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="86972-133">Response</span></span>
<span data-ttu-id="86972-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86972-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




