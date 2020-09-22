---
title: Obter userExperienceAnalyticsScoreHistory
description: Leia as propriedades e as relações do objeto userExperienceAnalyticsScoreHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eee751ad0bbe9f2280cde1724e649bf84c006738
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48047438"
---
# <a name="get-userexperienceanalyticsscorehistory"></a><span data-ttu-id="a0bd0-103">Obter userExperienceAnalyticsScoreHistory</span><span class="sxs-lookup"><span data-stu-id="a0bd0-103">Get userExperienceAnalyticsScoreHistory</span></span>

<span data-ttu-id="a0bd0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0bd0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0bd0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a0bd0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0bd0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0bd0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0bd0-107">Leia as propriedades e as relações do objeto [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) .</span><span class="sxs-lookup"><span data-stu-id="a0bd0-107">Read properties and relationships of the [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0bd0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0bd0-108">Prerequisites</span></span>
<span data-ttu-id="a0bd0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0bd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0bd0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0bd0-111">Permission type</span></span>|<span data-ttu-id="a0bd0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0bd0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0bd0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0bd0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0bd0-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0bd0-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a0bd0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0bd0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0bd0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0bd0-116">Not supported.</span></span>|
|<span data-ttu-id="a0bd0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0bd0-117">Application</span></span>|<span data-ttu-id="a0bd0-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0bd0-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0bd0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0bd0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0bd0-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a0bd0-120">Optional query parameters</span></span>
<span data-ttu-id="a0bd0-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a0bd0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0bd0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0bd0-122">Request headers</span></span>
|<span data-ttu-id="a0bd0-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0bd0-123">Header</span></span>|<span data-ttu-id="a0bd0-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a0bd0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0bd0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0bd0-125">Authorization</span></span>|<span data-ttu-id="a0bd0-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0bd0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0bd0-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0bd0-127">Accept</span></span>|<span data-ttu-id="a0bd0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a0bd0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0bd0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0bd0-129">Request body</span></span>
<span data-ttu-id="a0bd0-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0bd0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0bd0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0bd0-131">Response</span></span>
<span data-ttu-id="a0bd0-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0bd0-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0bd0-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0bd0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0bd0-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0bd0-134">Request</span></span>
<span data-ttu-id="a0bd0-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0bd0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
```

### <a name="response"></a><span data-ttu-id="a0bd0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0bd0-136">Response</span></span>
<span data-ttu-id="a0bd0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0bd0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 350

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
    "id": "d15e3ba8-3ba8-d15e-a83b-5ed1a83b5ed1",
    "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
    "startupScore": 12,
    "coreBootScore": 13,
    "coreSigninScore": 15,
    "recommendedSoftwareScore": 8,
    "restartScore": 12
  }
}
```






