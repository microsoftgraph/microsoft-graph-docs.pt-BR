---
title: Criar userExperienceAnalyticsMetricHistory
description: Criar um novo objeto userExperienceAnalyticsMetricHistory.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ac109c158205e21e28b2fb8c5defa60ad9b3b576
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793148"
---
# <a name="create-userexperienceanalyticsmetrichistory"></a><span data-ttu-id="4e3dd-103">Criar userExperienceAnalyticsMetricHistory</span><span class="sxs-lookup"><span data-stu-id="4e3dd-103">Create userExperienceAnalyticsMetricHistory</span></span>

<span data-ttu-id="4e3dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e3dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e3dd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4e3dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e3dd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e3dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e3dd-107">Criar um novo objeto [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) .</span><span class="sxs-lookup"><span data-stu-id="4e3dd-107">Create a new [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e3dd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4e3dd-108">Prerequisites</span></span>
<span data-ttu-id="4e3dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e3dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e3dd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e3dd-111">Permission type</span></span>|<span data-ttu-id="4e3dd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4e3dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e3dd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e3dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e3dd-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e3dd-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4e3dd-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e3dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e3dd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e3dd-116">Not supported.</span></span>|
|<span data-ttu-id="4e3dd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e3dd-117">Application</span></span>|<span data-ttu-id="4e3dd-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e3dd-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e3dd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e3dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsMetricHistory
```

## <a name="request-headers"></a><span data-ttu-id="4e3dd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e3dd-120">Request headers</span></span>
|<span data-ttu-id="4e3dd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4e3dd-121">Header</span></span>|<span data-ttu-id="4e3dd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4e3dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e3dd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e3dd-123">Authorization</span></span>|<span data-ttu-id="4e3dd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e3dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e3dd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4e3dd-125">Accept</span></span>|<span data-ttu-id="4e3dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e3dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e3dd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e3dd-127">Request body</span></span>
<span data-ttu-id="4e3dd-128">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsMetricHistory.</span><span class="sxs-lookup"><span data-stu-id="4e3dd-128">In the request body, supply a JSON representation for the userExperienceAnalyticsMetricHistory object.</span></span>

<span data-ttu-id="4e3dd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsMetricHistory.</span><span class="sxs-lookup"><span data-stu-id="4e3dd-129">The following table shows the properties that are required when you create the userExperienceAnalyticsMetricHistory.</span></span>

|<span data-ttu-id="4e3dd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e3dd-130">Property</span></span>|<span data-ttu-id="4e3dd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e3dd-131">Type</span></span>|<span data-ttu-id="4e3dd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e3dd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e3dd-133">id</span><span class="sxs-lookup"><span data-stu-id="4e3dd-133">id</span></span>|<span data-ttu-id="4e3dd-134">String</span><span class="sxs-lookup"><span data-stu-id="4e3dd-134">String</span></span>|<span data-ttu-id="4e3dd-135">O identificador exclusivo do histórico de métricas de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="4e3dd-135">The unique identifier of the user experience analytics metric history.</span></span>|
|<span data-ttu-id="4e3dd-136">metricDateTime</span><span class="sxs-lookup"><span data-stu-id="4e3dd-136">metricDateTime</span></span>|<span data-ttu-id="4e3dd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e3dd-137">DateTimeOffset</span></span>|<span data-ttu-id="4e3dd-138">A data e hora da métrica da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="4e3dd-138">The user experience analytics metric date time.</span></span>|



## <a name="response"></a><span data-ttu-id="4e3dd-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e3dd-139">Response</span></span>
<span data-ttu-id="4e3dd-140">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e3dd-140">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e3dd-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e3dd-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e3dd-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e3dd-142">Request</span></span>
<span data-ttu-id="4e3dd-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e3dd-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsMetricHistory
Content-type: application/json
Content-length: 136

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00"
}
```

### <a name="response"></a><span data-ttu-id="4e3dd-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e3dd-144">Response</span></span>
<span data-ttu-id="4e3dd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e3dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 185

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "id": "2b6d6456-6456-2b6d-5664-6d2b56646d2b",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00"
}
```


