---
title: Obter appLogCollectionRequest
description: Leia as propriedades e as relações do objeto appLogCollectionRequest.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f3daa16ac5a343db6f057e74f80096c568bc0eb
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959849"
---
# <a name="get-applogcollectionrequest"></a><span data-ttu-id="8adfc-103">Obter appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="8adfc-103">Get appLogCollectionRequest</span></span>

> <span data-ttu-id="8adfc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8adfc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8adfc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8adfc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8adfc-106">Leia as propriedades e as relações do objeto [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="8adfc-106">Read properties and relationships of the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8adfc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8adfc-107">Prerequisites</span></span>
<span data-ttu-id="8adfc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8adfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8adfc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8adfc-110">Permission type</span></span>|<span data-ttu-id="8adfc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8adfc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8adfc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8adfc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8adfc-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8adfc-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="8adfc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8adfc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8adfc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8adfc-115">Not supported.</span></span>|
|<span data-ttu-id="8adfc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8adfc-116">Application</span></span>|<span data-ttu-id="8adfc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8adfc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8adfc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8adfc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8adfc-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8adfc-119">Optional query parameters</span></span>
<span data-ttu-id="8adfc-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8adfc-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8adfc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8adfc-121">Request headers</span></span>
|<span data-ttu-id="8adfc-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8adfc-122">Header</span></span>|<span data-ttu-id="8adfc-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8adfc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8adfc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8adfc-124">Authorization</span></span>|<span data-ttu-id="8adfc-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8adfc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8adfc-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8adfc-126">Accept</span></span>|<span data-ttu-id="8adfc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8adfc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8adfc-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8adfc-128">Request body</span></span>
<span data-ttu-id="8adfc-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8adfc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8adfc-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8adfc-130">Response</span></span>
<span data-ttu-id="8adfc-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8adfc-131">If successful, this method returns a `200 OK` response code and [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8adfc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8adfc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8adfc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8adfc-133">Request</span></span>
<span data-ttu-id="8adfc-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8adfc-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

### <a name="response"></a><span data-ttu-id="8adfc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8adfc-135">Response</span></span>
<span data-ttu-id="8adfc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8adfc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 341

{
  "value": {
    "@odata.type": "#microsoft.graph.appLogCollectionRequest",
    "id": "cca685ff-85ff-cca6-ff85-a6ccff85a6cc",
    "status": "completed",
    "errorMessage": "Error Message value",
    "customLogFolders": [
      "Custom Log Folders value"
    ],
    "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
  }
}
```




