---
title: ação createDownloadUrl
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1e9ab5b0e1d780a64f533026d492ffa9ce0e0e02
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49286175"
---
# <a name="createdownloadurl-action"></a><span data-ttu-id="9c672-103">ação createDownloadUrl</span><span class="sxs-lookup"><span data-stu-id="9c672-103">createDownloadUrl action</span></span>

<span data-ttu-id="9c672-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c672-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c672-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9c672-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c672-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9c672-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c672-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9c672-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c672-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9c672-108">Prerequisites</span></span>
<span data-ttu-id="9c672-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c672-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c672-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c672-111">Permission type</span></span>|<span data-ttu-id="9c672-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9c672-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c672-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c672-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c672-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c672-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9c672-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c672-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c672-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c672-116">Not supported.</span></span>|
|<span data-ttu-id="9c672-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c672-117">Application</span></span>|<span data-ttu-id="9c672-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c672-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c672-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c672-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}/createDownloadUrl
```

## <a name="request-headers"></a><span data-ttu-id="9c672-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c672-120">Request headers</span></span>
|<span data-ttu-id="9c672-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9c672-121">Header</span></span>|<span data-ttu-id="9c672-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9c672-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c672-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c672-123">Authorization</span></span>|<span data-ttu-id="9c672-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c672-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c672-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9c672-125">Accept</span></span>|<span data-ttu-id="9c672-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c672-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c672-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c672-127">Request body</span></span>
<span data-ttu-id="9c672-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9c672-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c672-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c672-129">Response</span></span>
<span data-ttu-id="9c672-130">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e um [appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c672-130">If successful, this action returns a `200 OK` response code and a [appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c672-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c672-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c672-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c672-132">Request</span></span>
<span data-ttu-id="9c672-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c672-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}/createDownloadUrl
```

### <a name="response"></a><span data-ttu-id="9c672-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c672-134">Response</span></span>
<span data-ttu-id="9c672-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9c672-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 239

{
  "value": {
    "@odata.type": "microsoft.graph.appLogCollectionDownloadDetails",
    "downloadUrl": "https://example.com/downloadUrl/",
    "decryptionKey": "Decryption Key value",
    "appLogDecryptionAlgorithm": "aes256"
  }
}
```




