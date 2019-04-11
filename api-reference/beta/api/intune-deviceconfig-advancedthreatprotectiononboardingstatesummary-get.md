---
title: Obter Navegaçãoadvancedthreatprotectiononboardingstatesummary
description: Leia as propriedades e as relações do objeto Navegaçãoadvancedthreatprotectiononboardingstatesummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ab240e0f72fc08672f7d52796a3b1d1a6b4cbb6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775496"
---
# <a name="get-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="ecdcd-103">Obter Navegaçãoadvancedthreatprotectiononboardingstatesummary</span><span class="sxs-lookup"><span data-stu-id="ecdcd-103">Get advancedThreatProtectionOnboardingStateSummary</span></span>

> <span data-ttu-id="ecdcd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ecdcd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ecdcd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ecdcd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecdcd-106">Leia as propriedades e as relações do objeto [navegaçãoadvancedthreatprotectiononboardingstatesummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="ecdcd-106">Read properties and relationships of the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecdcd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ecdcd-107">Prerequisites</span></span>
<span data-ttu-id="ecdcd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecdcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecdcd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ecdcd-110">Permission type</span></span>|<span data-ttu-id="ecdcd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ecdcd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecdcd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ecdcd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ecdcd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ecdcd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ecdcd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ecdcd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecdcd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecdcd-115">Not supported.</span></span>|
|<span data-ttu-id="ecdcd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ecdcd-116">Application</span></span>|<span data-ttu-id="ecdcd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecdcd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecdcd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ecdcd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ecdcd-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ecdcd-119">Optional query parameters</span></span>
<span data-ttu-id="ecdcd-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ecdcd-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ecdcd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ecdcd-121">Request headers</span></span>
|<span data-ttu-id="ecdcd-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ecdcd-122">Header</span></span>|<span data-ttu-id="ecdcd-123">Valor</span><span class="sxs-lookup"><span data-stu-id="ecdcd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecdcd-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ecdcd-124">Authorization</span></span>|<span data-ttu-id="ecdcd-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecdcd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecdcd-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ecdcd-126">Accept</span></span>|<span data-ttu-id="ecdcd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ecdcd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecdcd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ecdcd-128">Request body</span></span>
<span data-ttu-id="ecdcd-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ecdcd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecdcd-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecdcd-130">Response</span></span>
<span data-ttu-id="ecdcd-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [navegaçãoadvancedthreatprotectiononboardingstatesummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ecdcd-131">If successful, this method returns a `200 OK` response code and [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecdcd-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ecdcd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecdcd-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ecdcd-133">Request</span></span>
<span data-ttu-id="ecdcd-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ecdcd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

### <a name="response"></a><span data-ttu-id="ecdcd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecdcd-135">Response</span></span>
<span data-ttu-id="ecdcd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ecdcd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





