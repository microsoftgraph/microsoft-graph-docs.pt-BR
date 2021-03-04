---
title: Atualizar userExperienceAnalyticsMetricHistory
description: Atualize as propriedades de um objeto userExperienceAnalyticsMetricHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7ca67205cd47625b08ba31173c2bbcf152147581
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434969"
---
# <a name="update-userexperienceanalyticsmetrichistory"></a><span data-ttu-id="52629-103">Atualizar userExperienceAnalyticsMetricHistory</span><span class="sxs-lookup"><span data-stu-id="52629-103">Update userExperienceAnalyticsMetricHistory</span></span>

<span data-ttu-id="52629-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52629-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52629-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="52629-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52629-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52629-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52629-107">Atualize as propriedades de [um objeto userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)</span><span class="sxs-lookup"><span data-stu-id="52629-107">Update the properties of a [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52629-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="52629-108">Prerequisites</span></span>
<span data-ttu-id="52629-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52629-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52629-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52629-111">Permission type</span></span>|<span data-ttu-id="52629-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="52629-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52629-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52629-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52629-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52629-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="52629-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52629-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52629-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52629-116">Not supported.</span></span>|
|<span data-ttu-id="52629-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52629-117">Application</span></span>|<span data-ttu-id="52629-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52629-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52629-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52629-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsMetricHistory/{userExperienceAnalyticsMetricHistoryId}
PATCH /deviceManagement/userExperienceAnalyticsDeviceMetricHistory/{userExperienceAnalyticsMetricHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="52629-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52629-120">Request headers</span></span>
|<span data-ttu-id="52629-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="52629-121">Header</span></span>|<span data-ttu-id="52629-122">Valor</span><span class="sxs-lookup"><span data-stu-id="52629-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52629-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="52629-123">Authorization</span></span>|<span data-ttu-id="52629-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52629-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52629-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="52629-125">Accept</span></span>|<span data-ttu-id="52629-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52629-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52629-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52629-127">Request body</span></span>
<span data-ttu-id="52629-128">No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)</span><span class="sxs-lookup"><span data-stu-id="52629-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object.</span></span>

<span data-ttu-id="52629-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md).</span><span class="sxs-lookup"><span data-stu-id="52629-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md).</span></span>

|<span data-ttu-id="52629-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52629-130">Property</span></span>|<span data-ttu-id="52629-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="52629-131">Type</span></span>|<span data-ttu-id="52629-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="52629-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52629-133">id</span><span class="sxs-lookup"><span data-stu-id="52629-133">id</span></span>|<span data-ttu-id="52629-134">String</span><span class="sxs-lookup"><span data-stu-id="52629-134">String</span></span>|<span data-ttu-id="52629-135">O identificador exclusivo do histórico métrico de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="52629-135">The unique identifier of the user experience analytics metric history.</span></span>|
|<span data-ttu-id="52629-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="52629-136">deviceId</span></span>|<span data-ttu-id="52629-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52629-137">String</span></span>|<span data-ttu-id="52629-138">A ID do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="52629-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="52629-139">metricDateTime</span><span class="sxs-lookup"><span data-stu-id="52629-139">metricDateTime</span></span>|<span data-ttu-id="52629-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52629-140">DateTimeOffset</span></span>|<span data-ttu-id="52629-141">A data de data métrica da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="52629-141">The user experience analytics metric date time.</span></span>|
|<span data-ttu-id="52629-142">metricType</span><span class="sxs-lookup"><span data-stu-id="52629-142">metricType</span></span>|<span data-ttu-id="52629-143">String</span><span class="sxs-lookup"><span data-stu-id="52629-143">String</span></span>|<span data-ttu-id="52629-144">O tipo métrico de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="52629-144">The user experience analytics metric type.</span></span>|



## <a name="response"></a><span data-ttu-id="52629-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="52629-145">Response</span></span>
<span data-ttu-id="52629-146">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52629-146">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52629-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52629-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="52629-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52629-148">Request</span></span>
<span data-ttu-id="52629-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52629-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsMetricHistory/{userExperienceAnalyticsMetricHistoryId}
Content-type: application/json
Content-length: 208

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "deviceId": "Device Id value",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00",
  "metricType": "Metric Type value"
}
```

### <a name="response"></a><span data-ttu-id="52629-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="52629-150">Response</span></span>
<span data-ttu-id="52629-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52629-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 257

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "id": "2b6d6456-6456-2b6d-5664-6d2b56646d2b",
  "deviceId": "Device Id value",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00",
  "metricType": "Metric Type value"
}
```




