---
title: Atualizar userExperienceAnalyticsWorkFromAnywhereMetric
description: Atualize as propriedades de um objeto userExperienceAnalyticsWorkFromAnywhereMetric.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e38f85106bf472c9eed7b0a6f1dff806fd075b5d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868328"
---
# <a name="update-userexperienceanalyticsworkfromanywheremetric"></a><span data-ttu-id="2b5c0-103">Atualizar userExperienceAnalyticsWorkFromAnywhereMetric</span><span class="sxs-lookup"><span data-stu-id="2b5c0-103">Update userExperienceAnalyticsWorkFromAnywhereMetric</span></span>

<span data-ttu-id="2b5c0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b5c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b5c0-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2b5c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b5c0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2b5c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b5c0-107">Atualize as propriedades de [um objeto userExperienceAnalyticsWorkFromAnywhereMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md)</span><span class="sxs-lookup"><span data-stu-id="2b5c0-107">Update the properties of a [userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b5c0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2b5c0-108">Prerequisites</span></span>
<span data-ttu-id="2b5c0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b5c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b5c0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b5c0-111">Permission type</span></span>|<span data-ttu-id="2b5c0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2b5c0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b5c0-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b5c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b5c0-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b5c0-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2b5c0-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b5c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b5c0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b5c0-116">Not supported.</span></span>|
|<span data-ttu-id="2b5c0-117">Application</span><span class="sxs-lookup"><span data-stu-id="2b5c0-117">Application</span></span>|<span data-ttu-id="2b5c0-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b5c0-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b5c0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b5c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}
```

## <a name="request-headers"></a><span data-ttu-id="2b5c0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b5c0-120">Request headers</span></span>
|<span data-ttu-id="2b5c0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2b5c0-121">Header</span></span>|<span data-ttu-id="2b5c0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2b5c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b5c0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b5c0-123">Authorization</span></span>|<span data-ttu-id="2b5c0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b5c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b5c0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2b5c0-125">Accept</span></span>|<span data-ttu-id="2b5c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b5c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b5c0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b5c0-127">Request body</span></span>
<span data-ttu-id="2b5c0-128">No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsWorkFromAnywhereMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md)</span><span class="sxs-lookup"><span data-stu-id="2b5c0-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md) object.</span></span>

<span data-ttu-id="2b5c0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md).</span><span class="sxs-lookup"><span data-stu-id="2b5c0-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md).</span></span>

|<span data-ttu-id="2b5c0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b5c0-130">Property</span></span>|<span data-ttu-id="2b5c0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b5c0-131">Type</span></span>|<span data-ttu-id="2b5c0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b5c0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b5c0-133">id</span><span class="sxs-lookup"><span data-stu-id="2b5c0-133">id</span></span>|<span data-ttu-id="2b5c0-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2b5c0-134">String</span></span>|<span data-ttu-id="2b5c0-135">O identificador exclusivo da análise de experiência do usuário funciona em qualquer lugar.</span><span class="sxs-lookup"><span data-stu-id="2b5c0-135">The unique identifier of the user experience analytics work from anywhere metric.</span></span>|



## <a name="response"></a><span data-ttu-id="2b5c0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b5c0-136">Response</span></span>
<span data-ttu-id="2b5c0-137">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b5c0-137">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b5c0-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b5c0-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b5c0-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b5c0-139">Request</span></span>
<span data-ttu-id="2b5c0-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b5c0-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}
Content-type: application/json
Content-length: 87

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereMetric"
}
```

### <a name="response"></a><span data-ttu-id="2b5c0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b5c0-141">Response</span></span>
<span data-ttu-id="2b5c0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b5c0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 136

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereMetric",
  "id": "7e6fda96-da96-7e6f-96da-6f7e96da6f7e"
}
```




