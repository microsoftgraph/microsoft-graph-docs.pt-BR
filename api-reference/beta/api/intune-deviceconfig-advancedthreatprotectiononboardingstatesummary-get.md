---
title: Obter Navegaçãoadvancedthreatprotectiononboardingstatesummary
description: Leia as propriedades e as relações do objeto Navegaçãoadvancedthreatprotectiononboardingstatesummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 94e40e53a9e85c2c063e02b878bf6b7d66d85e40
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37170277"
---
# <a name="get-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="91ddb-103">Obter Navegaçãoadvancedthreatprotectiononboardingstatesummary</span><span class="sxs-lookup"><span data-stu-id="91ddb-103">Get advancedThreatProtectionOnboardingStateSummary</span></span>

> <span data-ttu-id="91ddb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="91ddb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91ddb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91ddb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91ddb-106">Leia as propriedades e as relações do objeto [navegaçãoadvancedthreatprotectiononboardingstatesummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="91ddb-106">Read properties and relationships of the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91ddb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="91ddb-107">Prerequisites</span></span>
<span data-ttu-id="91ddb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91ddb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91ddb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91ddb-110">Permission type</span></span>|<span data-ttu-id="91ddb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="91ddb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91ddb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91ddb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="91ddb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="91ddb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="91ddb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91ddb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91ddb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91ddb-115">Not supported.</span></span>|
|<span data-ttu-id="91ddb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91ddb-116">Application</span></span>|<span data-ttu-id="91ddb-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="91ddb-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91ddb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91ddb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="91ddb-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="91ddb-119">Optional query parameters</span></span>
<span data-ttu-id="91ddb-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="91ddb-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91ddb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91ddb-121">Request headers</span></span>
|<span data-ttu-id="91ddb-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91ddb-122">Header</span></span>|<span data-ttu-id="91ddb-123">Valor</span><span class="sxs-lookup"><span data-stu-id="91ddb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91ddb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="91ddb-124">Authorization</span></span>|<span data-ttu-id="91ddb-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91ddb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91ddb-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="91ddb-126">Accept</span></span>|<span data-ttu-id="91ddb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="91ddb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91ddb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91ddb-128">Request body</span></span>
<span data-ttu-id="91ddb-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="91ddb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91ddb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="91ddb-130">Response</span></span>
<span data-ttu-id="91ddb-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [navegaçãoadvancedthreatprotectiononboardingstatesummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91ddb-131">If successful, this method returns a `200 OK` response code and [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91ddb-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91ddb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="91ddb-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91ddb-133">Request</span></span>
<span data-ttu-id="91ddb-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91ddb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

### <a name="response"></a><span data-ttu-id="91ddb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="91ddb-135">Response</span></span>
<span data-ttu-id="91ddb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91ddb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 419

{
  "value": {
    "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
    "id": "74089602-9602-7408-0296-087402960874",
    "unknownDeviceCount": 2,
    "notApplicableDeviceCount": 8,
    "compliantDeviceCount": 4,
    "remediatedDeviceCount": 5,
    "nonCompliantDeviceCount": 7,
    "errorDeviceCount": 0,
    "conflictDeviceCount": 3,
    "notAssignedDeviceCount": 6
  }
}
```




