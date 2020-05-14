---
title: Obter windowsInformationProtectionAppLearningSummary
description: Ler propriedades e relações do objeto windowsInformationProtectionAppLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6aae392b05bf727286ce7da72899ecd323efee0a
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "43439700"
---
# <a name="get-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="f1ea4-103">Obter windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="f1ea4-103">Get windowsInformationProtectionAppLearningSummary</span></span>

<span data-ttu-id="f1ea4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1ea4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1ea4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f1ea4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1ea4-106">Ler propriedades e relações do objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="f1ea4-106">Read properties and relationships of the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1ea4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f1ea4-107">Prerequisites</span></span>
<span data-ttu-id="f1ea4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1ea4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1ea4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1ea4-110">Permission type</span></span>|<span data-ttu-id="f1ea4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f1ea4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1ea4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1ea4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1ea4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1ea4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f1ea4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1ea4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1ea4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1ea4-115">Not supported.</span></span>|
|<span data-ttu-id="f1ea4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1ea4-116">Application</span></span>|<span data-ttu-id="f1ea4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1ea4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1ea4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1ea4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f1ea4-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f1ea4-119">Optional query parameters</span></span>
<span data-ttu-id="f1ea4-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f1ea4-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1ea4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1ea4-121">Request headers</span></span>
|<span data-ttu-id="f1ea4-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1ea4-122">Header</span></span>|<span data-ttu-id="f1ea4-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f1ea4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1ea4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1ea4-124">Authorization</span></span>|<span data-ttu-id="f1ea4-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1ea4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1ea4-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f1ea4-126">Accept</span></span>|<span data-ttu-id="f1ea4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f1ea4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1ea4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1ea4-128">Request body</span></span>
<span data-ttu-id="f1ea4-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1ea4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1ea4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1ea4-130">Response</span></span>
<span data-ttu-id="f1ea4-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1ea4-131">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1ea4-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1ea4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1ea4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1ea4-133">Request</span></span>
<span data-ttu-id="f1ea4-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1ea4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="f1ea4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1ea4-135">Response</span></span>
<span data-ttu-id="f1ea4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1ea4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






