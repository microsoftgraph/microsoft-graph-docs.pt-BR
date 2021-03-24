---
title: Atualizar userExperienceAnalyticsImpactingProcess
description: Atualize as propriedades de um objeto userExperienceAnalyticsImpactingProcess.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f2d1f2c3a2791e6536e701be35bc0c5c91e62949
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146220"
---
# <a name="update-userexperienceanalyticsimpactingprocess"></a><span data-ttu-id="98b65-103">Atualizar userExperienceAnalyticsImpactingProcess</span><span class="sxs-lookup"><span data-stu-id="98b65-103">Update userExperienceAnalyticsImpactingProcess</span></span>

<span data-ttu-id="98b65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98b65-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98b65-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="98b65-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98b65-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="98b65-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98b65-107">Atualize as propriedades de [um objeto userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)</span><span class="sxs-lookup"><span data-stu-id="98b65-107">Update the properties of a [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98b65-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="98b65-108">Prerequisites</span></span>
<span data-ttu-id="98b65-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98b65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98b65-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98b65-111">Permission type</span></span>|<span data-ttu-id="98b65-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="98b65-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98b65-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98b65-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98b65-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98b65-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="98b65-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98b65-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98b65-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98b65-116">Not supported.</span></span>|
|<span data-ttu-id="98b65-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98b65-117">Application</span></span>|<span data-ttu-id="98b65-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98b65-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="98b65-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98b65-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsImpactingProcess/{userExperienceAnalyticsImpactingProcessId}
```

## <a name="request-headers"></a><span data-ttu-id="98b65-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98b65-120">Request headers</span></span>
|<span data-ttu-id="98b65-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="98b65-121">Header</span></span>|<span data-ttu-id="98b65-122">Valor</span><span class="sxs-lookup"><span data-stu-id="98b65-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98b65-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="98b65-123">Authorization</span></span>|<span data-ttu-id="98b65-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98b65-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98b65-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="98b65-125">Accept</span></span>|<span data-ttu-id="98b65-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98b65-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98b65-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98b65-127">Request body</span></span>
<span data-ttu-id="98b65-128">No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)</span><span class="sxs-lookup"><span data-stu-id="98b65-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) object.</span></span>

<span data-ttu-id="98b65-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md).</span><span class="sxs-lookup"><span data-stu-id="98b65-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md).</span></span>

|<span data-ttu-id="98b65-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98b65-130">Property</span></span>|<span data-ttu-id="98b65-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="98b65-131">Type</span></span>|<span data-ttu-id="98b65-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="98b65-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98b65-133">id</span><span class="sxs-lookup"><span data-stu-id="98b65-133">id</span></span>|<span data-ttu-id="98b65-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98b65-134">String</span></span>|<span data-ttu-id="98b65-135">O identificador exclusivo da entidade de processo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="98b65-135">The unique identifier of the user experience analytics top impacting process entity.</span></span>|
|<span data-ttu-id="98b65-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="98b65-136">deviceId</span></span>|<span data-ttu-id="98b65-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98b65-137">String</span></span>|<span data-ttu-id="98b65-138">O identificador exclusivo do dispositivo afetado.</span><span class="sxs-lookup"><span data-stu-id="98b65-138">The unique identifier of the impacted device.</span></span>|
|<span data-ttu-id="98b65-139">category</span><span class="sxs-lookup"><span data-stu-id="98b65-139">category</span></span>|<span data-ttu-id="98b65-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98b65-140">String</span></span>|<span data-ttu-id="98b65-141">A categoria do processo de impacto.</span><span class="sxs-lookup"><span data-stu-id="98b65-141">The category of impacting process.</span></span>|
|<span data-ttu-id="98b65-142">processName</span><span class="sxs-lookup"><span data-stu-id="98b65-142">processName</span></span>|<span data-ttu-id="98b65-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98b65-143">String</span></span>|<span data-ttu-id="98b65-144">O nome do processo.</span><span class="sxs-lookup"><span data-stu-id="98b65-144">The process name.</span></span>|
|<span data-ttu-id="98b65-145">descrição</span><span class="sxs-lookup"><span data-stu-id="98b65-145">description</span></span>|<span data-ttu-id="98b65-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98b65-146">String</span></span>|<span data-ttu-id="98b65-147">A descrição do processo.</span><span class="sxs-lookup"><span data-stu-id="98b65-147">The description of process.</span></span>|
|<span data-ttu-id="98b65-148">publicador</span><span class="sxs-lookup"><span data-stu-id="98b65-148">publisher</span></span>|<span data-ttu-id="98b65-149">String</span><span class="sxs-lookup"><span data-stu-id="98b65-149">String</span></span>|<span data-ttu-id="98b65-150">O editor do processo.</span><span class="sxs-lookup"><span data-stu-id="98b65-150">The publisher of the process.</span></span>|
|<span data-ttu-id="98b65-151">impactValue</span><span class="sxs-lookup"><span data-stu-id="98b65-151">impactValue</span></span>|<span data-ttu-id="98b65-152">Duplo</span><span class="sxs-lookup"><span data-stu-id="98b65-152">Double</span></span>|<span data-ttu-id="98b65-153">O valor de impacto do processo.</span><span class="sxs-lookup"><span data-stu-id="98b65-153">The impact value of the process.</span></span> <span data-ttu-id="98b65-154">Valores válidos de 0 a 1,79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="98b65-154">Valid values 0 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="98b65-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="98b65-155">Response</span></span>
<span data-ttu-id="98b65-156">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98b65-156">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98b65-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98b65-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="98b65-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98b65-158">Request</span></span>
<span data-ttu-id="98b65-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98b65-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsImpactingProcess/{userExperienceAnalyticsImpactingProcessId}
Content-type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsImpactingProcess",
  "deviceId": "Device Id value",
  "category": "Category value",
  "processName": "Process Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "impactValue": 3.6666666666666665
}
```

### <a name="response"></a><span data-ttu-id="98b65-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="98b65-160">Response</span></span>
<span data-ttu-id="98b65-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98b65-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 349

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsImpactingProcess",
  "id": "faefd665-d665-faef-65d6-effa65d6effa",
  "deviceId": "Device Id value",
  "category": "Category value",
  "processName": "Process Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "impactValue": 3.6666666666666665
}
```




