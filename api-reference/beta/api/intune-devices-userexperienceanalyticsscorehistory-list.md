---
title: Listar userExperienceAnalyticsScoreHistories
description: Listar propriedades e relações dos objetos userExperienceAnalyticsScoreHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5880d554bf6fb26fd113252406a466d41a266400
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666286"
---
# <a name="list-userexperienceanalyticsscorehistories"></a><span data-ttu-id="87739-103">Listar userExperienceAnalyticsScoreHistories</span><span class="sxs-lookup"><span data-stu-id="87739-103">List userExperienceAnalyticsScoreHistories</span></span>

<span data-ttu-id="87739-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87739-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87739-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="87739-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87739-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="87739-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87739-107">Listar propriedades e relações dos [objetos userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)</span><span class="sxs-lookup"><span data-stu-id="87739-107">List properties and relationships of the [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87739-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="87739-108">Prerequisites</span></span>
<span data-ttu-id="87739-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87739-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87739-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87739-111">Permission type</span></span>|<span data-ttu-id="87739-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87739-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87739-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87739-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87739-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87739-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="87739-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87739-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87739-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87739-116">Not supported.</span></span>|
|<span data-ttu-id="87739-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87739-117">Application</span></span>|<span data-ttu-id="87739-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87739-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87739-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87739-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsScoreHistory
```

## <a name="request-headers"></a><span data-ttu-id="87739-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87739-120">Request headers</span></span>
|<span data-ttu-id="87739-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87739-121">Header</span></span>|<span data-ttu-id="87739-122">Valor</span><span class="sxs-lookup"><span data-stu-id="87739-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87739-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="87739-123">Authorization</span></span>|<span data-ttu-id="87739-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87739-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87739-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="87739-125">Accept</span></span>|<span data-ttu-id="87739-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87739-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87739-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87739-127">Request body</span></span>
<span data-ttu-id="87739-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87739-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87739-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="87739-129">Response</span></span>
<span data-ttu-id="87739-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87739-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87739-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87739-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="87739-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87739-132">Request</span></span>
<span data-ttu-id="87739-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87739-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory
```

### <a name="response"></a><span data-ttu-id="87739-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="87739-134">Response</span></span>
<span data-ttu-id="87739-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87739-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 407

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
      "id": "d15e3ba8-3ba8-d15e-a83b-5ed1a83b5ed1",
      "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
      "overallScore": 12,
      "startupScore": 12,
      "coreBootScore": 13,
      "coreSigninScore": 15,
      "recommendedSoftwareScore": 8,
      "restartScore": 12
    }
  ]
}
```




