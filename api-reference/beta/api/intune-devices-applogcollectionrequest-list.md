---
title: Listar appLogCollectionRequests
description: Listar propriedades e relações dos objetos appLogCollectionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f1ade110b94bea678db2fc15016aafd05e9ca51b
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612110"
---
# <a name="list-applogcollectionrequests"></a><span data-ttu-id="17b59-103">Listar appLogCollectionRequests</span><span class="sxs-lookup"><span data-stu-id="17b59-103">List appLogCollectionRequests</span></span>

<span data-ttu-id="17b59-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17b59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17b59-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="17b59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17b59-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="17b59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17b59-107">Listar propriedades e relações dos [objetos appLogCollectionRequest.](../resources/intune-devices-applogcollectionrequest.md)</span><span class="sxs-lookup"><span data-stu-id="17b59-107">List properties and relationships of the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17b59-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="17b59-108">Prerequisites</span></span>
<span data-ttu-id="17b59-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17b59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17b59-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17b59-111">Permission type</span></span>|<span data-ttu-id="17b59-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17b59-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17b59-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17b59-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17b59-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17b59-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="17b59-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17b59-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17b59-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17b59-116">Not supported.</span></span>|
|<span data-ttu-id="17b59-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17b59-117">Application</span></span>|<span data-ttu-id="17b59-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17b59-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17b59-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17b59-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="17b59-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17b59-120">Request headers</span></span>
|<span data-ttu-id="17b59-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17b59-121">Header</span></span>|<span data-ttu-id="17b59-122">Valor</span><span class="sxs-lookup"><span data-stu-id="17b59-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17b59-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="17b59-123">Authorization</span></span>|<span data-ttu-id="17b59-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17b59-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17b59-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="17b59-125">Accept</span></span>|<span data-ttu-id="17b59-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17b59-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17b59-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17b59-127">Request body</span></span>
<span data-ttu-id="17b59-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="17b59-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17b59-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="17b59-129">Response</span></span>
<span data-ttu-id="17b59-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17b59-130">If successful, this method returns a `200 OK` response code and a collection of [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17b59-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17b59-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="17b59-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17b59-132">Request</span></span>
<span data-ttu-id="17b59-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17b59-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

### <a name="response"></a><span data-ttu-id="17b59-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="17b59-134">Response</span></span>
<span data-ttu-id="17b59-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17b59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 371

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appLogCollectionRequest",
      "id": "cca685ff-85ff-cca6-ff85-a6ccff85a6cc",
      "status": "completed",
      "errorMessage": "Error Message value",
      "customLogFolders": [
        "Custom Log Folders value"
      ],
      "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
    }
  ]
}
```




