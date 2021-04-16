---
title: Listar userExperienceAnalyticsWorkFromAnywhereMetrics
description: Listar propriedades e relações dos objetos userExperienceAnalyticsWorkFromAnywhereMetric.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2dca9409761f916587e94e7846016d4935bc6303
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868250"
---
# <a name="list-userexperienceanalyticsworkfromanywheremetrics"></a><span data-ttu-id="2f209-103">Listar userExperienceAnalyticsWorkFromAnywhereMetrics</span><span class="sxs-lookup"><span data-stu-id="2f209-103">List userExperienceAnalyticsWorkFromAnywhereMetrics</span></span>

<span data-ttu-id="2f209-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f209-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f209-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2f209-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f209-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f209-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f209-107">Listar propriedades e relações dos [objetos userExperienceAnalyticsWorkFromAnywhereMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md)</span><span class="sxs-lookup"><span data-stu-id="2f209-107">List properties and relationships of the [userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f209-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f209-108">Prerequisites</span></span>
<span data-ttu-id="2f209-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f209-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f209-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f209-111">Permission type</span></span>|<span data-ttu-id="2f209-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f209-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f209-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f209-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f209-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f209-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2f209-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f209-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f209-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f209-116">Not supported.</span></span>|
|<span data-ttu-id="2f209-117">Application</span><span class="sxs-lookup"><span data-stu-id="2f209-117">Application</span></span>|<span data-ttu-id="2f209-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f209-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f209-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f209-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics
```

## <a name="request-headers"></a><span data-ttu-id="2f209-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f209-120">Request headers</span></span>
|<span data-ttu-id="2f209-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f209-121">Header</span></span>|<span data-ttu-id="2f209-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2f209-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f209-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f209-123">Authorization</span></span>|<span data-ttu-id="2f209-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f209-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f209-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f209-125">Accept</span></span>|<span data-ttu-id="2f209-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f209-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f209-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f209-127">Request body</span></span>
<span data-ttu-id="2f209-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2f209-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f209-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f209-129">Response</span></span>
<span data-ttu-id="2f209-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f209-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f209-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f209-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f209-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f209-132">Request</span></span>
<span data-ttu-id="2f209-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f209-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics
```

### <a name="response"></a><span data-ttu-id="2f209-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f209-134">Response</span></span>
<span data-ttu-id="2f209-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f209-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 177

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereMetric",
      "id": "7e6fda96-da96-7e6f-96da-6f7e96da6f7e"
    }
  ]
}
```




