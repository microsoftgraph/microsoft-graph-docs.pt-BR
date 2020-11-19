---
title: Listar macOSSoftwareUpdateCategorySummaries
description: Listar Propriedades e relações dos objetos macOSSoftwareUpdateCategorySummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ad41dbf61c8fe894b28c911bcfa7221c3c40eab2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49236481"
---
# <a name="list-macossoftwareupdatecategorysummaries"></a><span data-ttu-id="bedd0-103">Listar macOSSoftwareUpdateCategorySummaries</span><span class="sxs-lookup"><span data-stu-id="bedd0-103">List macOSSoftwareUpdateCategorySummaries</span></span>

<span data-ttu-id="bedd0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bedd0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bedd0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bedd0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bedd0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bedd0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bedd0-107">Listar Propriedades e relações dos objetos [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) .</span><span class="sxs-lookup"><span data-stu-id="bedd0-107">List properties and relationships of the [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bedd0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bedd0-108">Prerequisites</span></span>
<span data-ttu-id="bedd0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bedd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bedd0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bedd0-111">Permission type</span></span>|<span data-ttu-id="bedd0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bedd0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bedd0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bedd0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bedd0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bedd0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bedd0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bedd0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bedd0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bedd0-116">Not supported.</span></span>|
|<span data-ttu-id="bedd0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bedd0-117">Application</span></span>|<span data-ttu-id="bedd0-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bedd0-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bedd0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bedd0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries
```

## <a name="request-headers"></a><span data-ttu-id="bedd0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bedd0-120">Request headers</span></span>
|<span data-ttu-id="bedd0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bedd0-121">Header</span></span>|<span data-ttu-id="bedd0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bedd0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bedd0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bedd0-123">Authorization</span></span>|<span data-ttu-id="bedd0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bedd0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bedd0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bedd0-125">Accept</span></span>|<span data-ttu-id="bedd0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bedd0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bedd0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bedd0-127">Request body</span></span>
<span data-ttu-id="bedd0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bedd0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bedd0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bedd0-129">Response</span></span>
<span data-ttu-id="bedd0-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bedd0-130">If successful, this method returns a `200 OK` response code and a collection of [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bedd0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bedd0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bedd0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bedd0-132">Request</span></span>
<span data-ttu-id="bedd0-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bedd0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries
```

### <a name="response"></a><span data-ttu-id="bedd0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bedd0-134">Response</span></span>
<span data-ttu-id="bedd0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bedd0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 495

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSSoftwareUpdateCategorySummary",
      "id": "f1fda232-a232-f1fd-32a2-fdf132a2fdf1",
      "displayName": "Display Name value",
      "deviceId": "Device Id value",
      "userId": "User Id value",
      "updateCategory": "configurationDataFile",
      "successfulUpdateCount": 5,
      "failedUpdateCount": 1,
      "totalUpdateCount": 0,
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```




