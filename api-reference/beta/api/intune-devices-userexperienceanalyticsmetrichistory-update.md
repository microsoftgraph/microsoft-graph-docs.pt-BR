---
title: Atualizar userExperienceAnalyticsMetricHistory
description: Atualizar as propriedades de um objeto userExperienceAnalyticsMetricHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b914f7d20793caa5b9a8848e90e3dc8bed61577a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161296"
---
# <a name="update-userexperienceanalyticsmetrichistory"></a><span data-ttu-id="8995c-103">Atualizar userExperienceAnalyticsMetricHistory</span><span class="sxs-lookup"><span data-stu-id="8995c-103">Update userExperienceAnalyticsMetricHistory</span></span>

<span data-ttu-id="8995c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8995c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8995c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8995c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8995c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8995c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8995c-107">Atualizar as propriedades de um [objeto userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)</span><span class="sxs-lookup"><span data-stu-id="8995c-107">Update the properties of a [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8995c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8995c-108">Prerequisites</span></span>
<span data-ttu-id="8995c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8995c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8995c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8995c-111">Permission type</span></span>|<span data-ttu-id="8995c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8995c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8995c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8995c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8995c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8995c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8995c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8995c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8995c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8995c-116">Not supported.</span></span>|
|<span data-ttu-id="8995c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8995c-117">Application</span></span>|<span data-ttu-id="8995c-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8995c-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8995c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8995c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsMetricHistory/{userExperienceAnalyticsMetricHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="8995c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8995c-120">Request headers</span></span>
|<span data-ttu-id="8995c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8995c-121">Header</span></span>|<span data-ttu-id="8995c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8995c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8995c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8995c-123">Authorization</span></span>|<span data-ttu-id="8995c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8995c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8995c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8995c-125">Accept</span></span>|<span data-ttu-id="8995c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8995c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8995c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8995c-127">Request body</span></span>
<span data-ttu-id="8995c-128">No corpo da solicitação, fornece uma representação JSON do [objeto userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)</span><span class="sxs-lookup"><span data-stu-id="8995c-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object.</span></span>

<span data-ttu-id="8995c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md).</span><span class="sxs-lookup"><span data-stu-id="8995c-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md).</span></span>

|<span data-ttu-id="8995c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8995c-130">Property</span></span>|<span data-ttu-id="8995c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8995c-131">Type</span></span>|<span data-ttu-id="8995c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8995c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8995c-133">id</span><span class="sxs-lookup"><span data-stu-id="8995c-133">id</span></span>|<span data-ttu-id="8995c-134">String</span><span class="sxs-lookup"><span data-stu-id="8995c-134">String</span></span>|<span data-ttu-id="8995c-135">O identificador exclusivo do histórico de métricas da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8995c-135">The unique identifier of the user experience analytics metric history.</span></span>|
|<span data-ttu-id="8995c-136">metricDateTime</span><span class="sxs-lookup"><span data-stu-id="8995c-136">metricDateTime</span></span>|<span data-ttu-id="8995c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8995c-137">DateTimeOffset</span></span>|<span data-ttu-id="8995c-138">A data e a hora da métrica da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8995c-138">The user experience analytics metric date time.</span></span>|
|<span data-ttu-id="8995c-139">metricType</span><span class="sxs-lookup"><span data-stu-id="8995c-139">metricType</span></span>|<span data-ttu-id="8995c-140">String</span><span class="sxs-lookup"><span data-stu-id="8995c-140">String</span></span>|<span data-ttu-id="8995c-141">O tipo de métrica de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8995c-141">The user experience analytics metric type.</span></span>|



## <a name="response"></a><span data-ttu-id="8995c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8995c-142">Response</span></span>
<span data-ttu-id="8995c-143">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8995c-143">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8995c-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8995c-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="8995c-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8995c-145">Request</span></span>
<span data-ttu-id="8995c-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8995c-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsMetricHistory/{userExperienceAnalyticsMetricHistoryId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00",
  "metricType": "Metric Type value"
}
```

### <a name="response"></a><span data-ttu-id="8995c-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="8995c-147">Response</span></span>
<span data-ttu-id="8995c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8995c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 223

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "id": "2b6d6456-6456-2b6d-5664-6d2b56646d2b",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00",
  "metricType": "Metric Type value"
}
```




