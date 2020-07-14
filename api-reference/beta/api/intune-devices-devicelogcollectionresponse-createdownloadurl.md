---
title: ação createDownloadUrl
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14a99fd6c09f213cde6494bcf912c5b6ffe58017
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124167"
---
# <a name="createdownloadurl-action"></a><span data-ttu-id="d4e1d-103">ação createDownloadUrl</span><span class="sxs-lookup"><span data-stu-id="d4e1d-103">createDownloadUrl action</span></span>

<span data-ttu-id="d4e1d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4e1d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4e1d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d4e1d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4e1d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d4e1d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4e1d-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d4e1d-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4e1d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d4e1d-108">Prerequisites</span></span>
<span data-ttu-id="d4e1d-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="d4e1d-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d4e1d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4e1d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4e1d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4e1d-111">Permission type</span></span>|<span data-ttu-id="d4e1d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d4e1d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4e1d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4e1d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4e1d-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4e1d-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d4e1d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4e1d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4e1d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4e1d-116">Not supported.</span></span>|
|<span data-ttu-id="d4e1d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4e1d-117">Application</span></span>|<span data-ttu-id="d4e1d-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4e1d-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4e1d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4e1d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests/{deviceLogCollectionResponseId}/createDownloadUrl
```

## <a name="request-headers"></a><span data-ttu-id="d4e1d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e1d-120">Request headers</span></span>
|<span data-ttu-id="d4e1d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4e1d-121">Header</span></span>|<span data-ttu-id="d4e1d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d4e1d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4e1d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4e1d-123">Authorization</span></span>|<span data-ttu-id="d4e1d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4e1d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4e1d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d4e1d-125">Accept</span></span>|<span data-ttu-id="d4e1d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4e1d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4e1d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e1d-127">Request body</span></span>
<span data-ttu-id="d4e1d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4e1d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4e1d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4e1d-129">Response</span></span>
<span data-ttu-id="d4e1d-130">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4e1d-130">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4e1d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4e1d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4e1d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e1d-132">Request</span></span>
<span data-ttu-id="d4e1d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4e1d-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests/{deviceLogCollectionResponseId}/createDownloadUrl
```

### <a name="response"></a><span data-ttu-id="d4e1d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4e1d-134">Response</span></span>
<span data-ttu-id="d4e1d-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="d4e1d-135">Here is an example of the response.</span></span> <span data-ttu-id="d4e1d-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="d4e1d-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d4e1d-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="d4e1d-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 57

{
  "value": "https://example.com/createDownloadUrl/"
}
```



