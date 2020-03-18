---
title: Obter userExperienceAnalyticsStartupScoreHistory
description: Leia as propriedades e as relações do objeto userExperienceAnalyticsStartupScoreHistory.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cde9869ff44b2de0f7642a8ad03e3c4eb7ebd046
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813758"
---
# <a name="get-userexperienceanalyticsstartupscorehistory"></a><span data-ttu-id="130fd-103">Obter userExperienceAnalyticsStartupScoreHistory</span><span class="sxs-lookup"><span data-stu-id="130fd-103">Get userExperienceAnalyticsStartupScoreHistory</span></span>

> <span data-ttu-id="130fd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="130fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="130fd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="130fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="130fd-106">Leia as propriedades e as relações do objeto [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) .</span><span class="sxs-lookup"><span data-stu-id="130fd-106">Read properties and relationships of the [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="130fd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="130fd-107">Prerequisites</span></span>
<span data-ttu-id="130fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="130fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="130fd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="130fd-110">Permission type</span></span>|<span data-ttu-id="130fd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="130fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="130fd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="130fd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="130fd-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="130fd-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="130fd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="130fd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="130fd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="130fd-115">Not supported.</span></span>|
|<span data-ttu-id="130fd-116">Application</span><span class="sxs-lookup"><span data-stu-id="130fd-116">Application</span></span>|<span data-ttu-id="130fd-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="130fd-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="130fd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="130fd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsStartupScoreHistory/{userExperienceAnalyticsStartupScoreHistoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="130fd-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="130fd-119">Optional query parameters</span></span>
<span data-ttu-id="130fd-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="130fd-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="130fd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="130fd-121">Request headers</span></span>
|<span data-ttu-id="130fd-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="130fd-122">Header</span></span>|<span data-ttu-id="130fd-123">Valor</span><span class="sxs-lookup"><span data-stu-id="130fd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="130fd-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="130fd-124">Authorization</span></span>|<span data-ttu-id="130fd-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="130fd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="130fd-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="130fd-126">Accept</span></span>|<span data-ttu-id="130fd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="130fd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="130fd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="130fd-128">Request body</span></span>
<span data-ttu-id="130fd-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="130fd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="130fd-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="130fd-130">Response</span></span>
<span data-ttu-id="130fd-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="130fd-131">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="130fd-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="130fd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="130fd-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="130fd-133">Request</span></span>
<span data-ttu-id="130fd-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="130fd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsStartupScoreHistory/{userExperienceAnalyticsStartupScoreHistoryId}
```

### <a name="response"></a><span data-ttu-id="130fd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="130fd-135">Response</span></span>
<span data-ttu-id="130fd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="130fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 332

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsStartupScoreHistory",
    "id": "52efee0b-ee0b-52ef-0bee-ef520beeef52",
    "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
    "startupScore": 12,
    "coreBootScore": 13,
    "coreSigninScore": 15,
    "recommendedSoftwareScore": 8
  }
}
```




