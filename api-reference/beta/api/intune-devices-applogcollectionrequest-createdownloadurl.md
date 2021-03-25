---
title: ação createDownloadUrl
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7d3c3a46b47d45d80532697aa7c900b74c40c57e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150651"
---
# <a name="createdownloadurl-action"></a><span data-ttu-id="cf660-103">ação createDownloadUrl</span><span class="sxs-lookup"><span data-stu-id="cf660-103">createDownloadUrl action</span></span>

<span data-ttu-id="cf660-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf660-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf660-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cf660-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf660-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf660-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf660-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cf660-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf660-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf660-108">Prerequisites</span></span>
<span data-ttu-id="cf660-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf660-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf660-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf660-111">Permission type</span></span>|<span data-ttu-id="cf660-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf660-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf660-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf660-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf660-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf660-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cf660-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf660-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf660-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf660-116">Not supported.</span></span>|
|<span data-ttu-id="cf660-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf660-117">Application</span></span>|<span data-ttu-id="cf660-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf660-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf660-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf660-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}/createDownloadUrl
```

## <a name="request-headers"></a><span data-ttu-id="cf660-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf660-120">Request headers</span></span>
|<span data-ttu-id="cf660-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf660-121">Header</span></span>|<span data-ttu-id="cf660-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cf660-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf660-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf660-123">Authorization</span></span>|<span data-ttu-id="cf660-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf660-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf660-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cf660-125">Accept</span></span>|<span data-ttu-id="cf660-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf660-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf660-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf660-127">Request body</span></span>
<span data-ttu-id="cf660-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cf660-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf660-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf660-129">Response</span></span>
<span data-ttu-id="cf660-130">Se tiver êxito, essa ação retornará um código de `200 OK` resposta e um [appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf660-130">If successful, this action returns a `200 OK` response code and a [appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf660-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf660-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf660-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf660-132">Request</span></span>
<span data-ttu-id="cf660-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf660-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}/createDownloadUrl
```

### <a name="response"></a><span data-ttu-id="cf660-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf660-134">Response</span></span>
<span data-ttu-id="cf660-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf660-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




