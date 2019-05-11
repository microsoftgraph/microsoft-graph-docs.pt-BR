---
title: Listar windowsInformationProtectionAppLearningSummaries
description: Listar propriedades e relações de objetos de windowsInformationProtectionAppLearningSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9d448a5f663cf4d5d6f58f399273251fad8e688b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33897783"
---
# <a name="list-windowsinformationprotectionapplearningsummaries"></a><span data-ttu-id="a275f-103">Listar windowsInformationProtectionAppLearningSummaries</span><span class="sxs-lookup"><span data-stu-id="a275f-103">List windowsInformationProtectionAppLearningSummaries</span></span>

> <span data-ttu-id="a275f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a275f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a275f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a275f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a275f-106">Listar propriedades e relações de objetos de [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="a275f-106">List properties and relationships of the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a275f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a275f-107">Prerequisites</span></span>
<span data-ttu-id="a275f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a275f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a275f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a275f-110">Permission type</span></span>|<span data-ttu-id="a275f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a275f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a275f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a275f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a275f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a275f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a275f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a275f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a275f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a275f-115">Not supported.</span></span>|
|<span data-ttu-id="a275f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a275f-116">Application</span></span>|<span data-ttu-id="a275f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a275f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a275f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a275f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="a275f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a275f-119">Request headers</span></span>
|<span data-ttu-id="a275f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a275f-120">Header</span></span>|<span data-ttu-id="a275f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a275f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a275f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a275f-122">Authorization</span></span>|<span data-ttu-id="a275f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a275f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a275f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a275f-124">Accept</span></span>|<span data-ttu-id="a275f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a275f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a275f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a275f-126">Request body</span></span>
<span data-ttu-id="a275f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a275f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a275f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a275f-128">Response</span></span>
<span data-ttu-id="a275f-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a275f-129">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a275f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a275f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a275f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a275f-131">Request</span></span>
<span data-ttu-id="a275f-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a275f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries
```

### <a name="response"></a><span data-ttu-id="a275f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a275f-133">Response</span></span>
<span data-ttu-id="a275f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a275f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




