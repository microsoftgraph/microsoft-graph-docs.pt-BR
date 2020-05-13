---
title: Obter windowsInformationProtectionAppLearningSummary
description: Ler propriedades e relações do objeto windowsInformationProtectionAppLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ad59288d350497c9539b94568d7e92dd72aee2f2
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "43451957"
---
# <a name="get-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="603ed-103">Obter windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="603ed-103">Get windowsInformationProtectionAppLearningSummary</span></span>

<span data-ttu-id="603ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="603ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="603ed-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="603ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="603ed-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="603ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="603ed-107">Ler propriedades e relações do objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="603ed-107">Read properties and relationships of the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="603ed-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="603ed-108">Prerequisites</span></span>
<span data-ttu-id="603ed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="603ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="603ed-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="603ed-111">Permission type</span></span>|<span data-ttu-id="603ed-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="603ed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="603ed-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="603ed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="603ed-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="603ed-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="603ed-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="603ed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="603ed-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="603ed-116">Not supported.</span></span>|
|<span data-ttu-id="603ed-117">Application</span><span class="sxs-lookup"><span data-stu-id="603ed-117">Application</span></span>|<span data-ttu-id="603ed-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="603ed-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="603ed-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="603ed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="603ed-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="603ed-120">Optional query parameters</span></span>
<span data-ttu-id="603ed-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="603ed-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="603ed-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="603ed-122">Request headers</span></span>
|<span data-ttu-id="603ed-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="603ed-123">Header</span></span>|<span data-ttu-id="603ed-124">Valor</span><span class="sxs-lookup"><span data-stu-id="603ed-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="603ed-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="603ed-125">Authorization</span></span>|<span data-ttu-id="603ed-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="603ed-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="603ed-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="603ed-127">Accept</span></span>|<span data-ttu-id="603ed-128">application/json</span><span class="sxs-lookup"><span data-stu-id="603ed-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="603ed-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="603ed-129">Request body</span></span>
<span data-ttu-id="603ed-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="603ed-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="603ed-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="603ed-131">Response</span></span>
<span data-ttu-id="603ed-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="603ed-132">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="603ed-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="603ed-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="603ed-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="603ed-134">Request</span></span>
<span data-ttu-id="603ed-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="603ed-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="603ed-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="603ed-136">Response</span></span>
<span data-ttu-id="603ed-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="603ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
    "id": "063baf50-af50-063b-50af-3b0650af3b06",
    "applicationName": "Application Name value",
    "applicationType": "desktop",
    "deviceCount": 11
  }
}
```



