---
title: Listar userExperienceAnalyticsBaselines
description: Listar Propriedades e relações dos objetos userExperienceAnalyticsBaseline.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 29a3ad020542cba558d50375248da2ea0d1a6fd7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42773242"
---
# <a name="list-userexperienceanalyticsbaselines"></a><span data-ttu-id="90dea-103">Listar userExperienceAnalyticsBaselines</span><span class="sxs-lookup"><span data-stu-id="90dea-103">List userExperienceAnalyticsBaselines</span></span>

> <span data-ttu-id="90dea-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="90dea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90dea-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90dea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90dea-106">Listar Propriedades e relações dos objetos [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) .</span><span class="sxs-lookup"><span data-stu-id="90dea-106">List properties and relationships of the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90dea-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90dea-107">Prerequisites</span></span>
<span data-ttu-id="90dea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90dea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90dea-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90dea-110">Permission type</span></span>|<span data-ttu-id="90dea-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="90dea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90dea-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90dea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90dea-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="90dea-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="90dea-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90dea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90dea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90dea-115">Not supported.</span></span>|
|<span data-ttu-id="90dea-116">Application</span><span class="sxs-lookup"><span data-stu-id="90dea-116">Application</span></span>|<span data-ttu-id="90dea-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="90dea-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90dea-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90dea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsBaselines
```

## <a name="request-headers"></a><span data-ttu-id="90dea-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90dea-119">Request headers</span></span>
|<span data-ttu-id="90dea-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90dea-120">Header</span></span>|<span data-ttu-id="90dea-121">Valor</span><span class="sxs-lookup"><span data-stu-id="90dea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90dea-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="90dea-122">Authorization</span></span>|<span data-ttu-id="90dea-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90dea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90dea-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90dea-124">Accept</span></span>|<span data-ttu-id="90dea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90dea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90dea-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90dea-126">Request body</span></span>
<span data-ttu-id="90dea-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90dea-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90dea-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="90dea-128">Response</span></span>
<span data-ttu-id="90dea-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90dea-129">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90dea-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90dea-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="90dea-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90dea-131">Request</span></span>
<span data-ttu-id="90dea-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90dea-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines
```

### <a name="response"></a><span data-ttu-id="90dea-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="90dea-133">Response</span></span>
<span data-ttu-id="90dea-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90dea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 323

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
      "id": "1cce2cab-2cab-1cce-ab2c-ce1cab2cce1c",
      "displayName": "Display Name value",
      "overallScore": 12,
      "isBuiltIn": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00"
    }
  ]
}
```




