---
title: Listar windowsInformationProtectionAppLearningSummaries
description: Listar propriedades e relações de objetos de windowsInformationProtectionAppLearningSummary.
author: tfitzmac
ms.openlocfilehash: 6fb2a4a9378ab7e5e0ce06ad896409cff95d0fdf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319310"
---
# <a name="list-windowsinformationprotectionapplearningsummaries"></a><span data-ttu-id="8e8da-103">Listar windowsInformationProtectionAppLearningSummaries</span><span class="sxs-lookup"><span data-stu-id="8e8da-103">List windowsInformationProtectionAppLearningSummaries</span></span>

> <span data-ttu-id="8e8da-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8e8da-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e8da-105">Listar propriedades e relações de objetos de [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="8e8da-105">List properties and relationships of the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8e8da-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8e8da-106">Prerequisites</span></span>
<span data-ttu-id="8e8da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e8da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e8da-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e8da-109">Permission type</span></span>|<span data-ttu-id="8e8da-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8e8da-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e8da-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e8da-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8e8da-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e8da-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8e8da-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e8da-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e8da-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e8da-114">Not supported.</span></span>|
|<span data-ttu-id="8e8da-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e8da-115">Application</span></span>|<span data-ttu-id="8e8da-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e8da-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e8da-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e8da-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="8e8da-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e8da-118">Request headers</span></span>
|<span data-ttu-id="8e8da-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e8da-119">Header</span></span>|<span data-ttu-id="8e8da-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8e8da-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e8da-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e8da-121">Authorization</span></span>|<span data-ttu-id="8e8da-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e8da-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e8da-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8e8da-123">Accept</span></span>|<span data-ttu-id="8e8da-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8e8da-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e8da-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e8da-125">Request body</span></span>
<span data-ttu-id="8e8da-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8e8da-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e8da-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e8da-127">Response</span></span>
<span data-ttu-id="8e8da-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e8da-128">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e8da-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e8da-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e8da-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e8da-130">Request</span></span>
<span data-ttu-id="8e8da-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e8da-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries
```

### <a name="response"></a><span data-ttu-id="8e8da-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e8da-132">Response</span></span>
<span data-ttu-id="8e8da-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e8da-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



