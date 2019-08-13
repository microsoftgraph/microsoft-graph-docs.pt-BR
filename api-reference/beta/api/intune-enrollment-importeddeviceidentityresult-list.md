---
title: Listar importedDeviceIdentityResults
description: Listar Propriedades e relações dos objetos importedDeviceIdentityResult.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 339f5ec68c050856a4b7c10e843044c26b8b758f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356295"
---
# <a name="list-importeddeviceidentityresults"></a><span data-ttu-id="09ee0-103">Listar importedDeviceIdentityResults</span><span class="sxs-lookup"><span data-stu-id="09ee0-103">List importedDeviceIdentityResults</span></span>

> <span data-ttu-id="09ee0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="09ee0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09ee0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="09ee0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09ee0-106">Listar Propriedades e relações dos objetos [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="09ee0-106">List properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09ee0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="09ee0-107">Prerequisites</span></span>
<span data-ttu-id="09ee0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09ee0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09ee0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09ee0-110">Permission type</span></span>|<span data-ttu-id="09ee0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="09ee0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09ee0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09ee0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="09ee0-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="09ee0-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="09ee0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09ee0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09ee0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09ee0-115">Not supported.</span></span>|
|<span data-ttu-id="09ee0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09ee0-116">Application</span></span>|<span data-ttu-id="09ee0-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="09ee0-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09ee0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09ee0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="09ee0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09ee0-119">Request headers</span></span>
|<span data-ttu-id="09ee0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="09ee0-120">Header</span></span>|<span data-ttu-id="09ee0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="09ee0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09ee0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="09ee0-122">Authorization</span></span>|<span data-ttu-id="09ee0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09ee0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09ee0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="09ee0-124">Accept</span></span>|<span data-ttu-id="09ee0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="09ee0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09ee0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09ee0-126">Request body</span></span>
<span data-ttu-id="09ee0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="09ee0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09ee0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="09ee0-128">Response</span></span>
<span data-ttu-id="09ee0-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09ee0-129">If successful, this method returns a `200 OK` response code and a collection of [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09ee0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09ee0-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="09ee0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09ee0-131">Request</span></span>
<span data-ttu-id="09ee0-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09ee0-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="09ee0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="09ee0-133">Response</span></span>
<span data-ttu-id="09ee0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09ee0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






