---
title: Listar windowsInformationProtectionAppLearningSummaries
description: Listar propriedades e relações de objetos de windowsInformationProtectionAppLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dba4e35d8911dfef29106177a1f1ff7893e6b50e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028654"
---
# <a name="list-windowsinformationprotectionapplearningsummaries"></a><span data-ttu-id="944bd-103">Listar windowsInformationProtectionAppLearningSummaries</span><span class="sxs-lookup"><span data-stu-id="944bd-103">List windowsInformationProtectionAppLearningSummaries</span></span>

<span data-ttu-id="944bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="944bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="944bd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="944bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="944bd-106">Listar propriedades e relações de objetos de [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="944bd-106">List properties and relationships of the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="944bd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="944bd-107">Prerequisites</span></span>
<span data-ttu-id="944bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="944bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="944bd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="944bd-110">Permission type</span></span>|<span data-ttu-id="944bd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="944bd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="944bd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="944bd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="944bd-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="944bd-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="944bd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="944bd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="944bd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="944bd-115">Not supported.</span></span>|
|<span data-ttu-id="944bd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="944bd-116">Application</span></span>|<span data-ttu-id="944bd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="944bd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="944bd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="944bd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="944bd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="944bd-119">Request headers</span></span>
|<span data-ttu-id="944bd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="944bd-120">Header</span></span>|<span data-ttu-id="944bd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="944bd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="944bd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="944bd-122">Authorization</span></span>|<span data-ttu-id="944bd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="944bd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="944bd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="944bd-124">Accept</span></span>|<span data-ttu-id="944bd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="944bd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="944bd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="944bd-126">Request body</span></span>
<span data-ttu-id="944bd-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="944bd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="944bd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="944bd-128">Response</span></span>
<span data-ttu-id="944bd-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="944bd-129">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="944bd-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="944bd-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="944bd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="944bd-131">Request</span></span>
<span data-ttu-id="944bd-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="944bd-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries
```

### <a name="response"></a><span data-ttu-id="944bd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="944bd-133">Response</span></span>
<span data-ttu-id="944bd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="944bd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 293

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
      "id": "063baf50-af50-063b-50af-3b0650af3b06",
      "applicationName": "Application Name value",
      "applicationType": "desktop",
      "deviceCount": 11
    }
  ]
}
```









