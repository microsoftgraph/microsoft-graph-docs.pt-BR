---
title: Criar userExperienceAnalyticsImpactingProcess
description: Crie um novo objeto userExperienceAnalyticsImpactingProcess.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a2026d52b9b371fd7d0eab7a987808947f0bb43
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153990"
---
# <a name="create-userexperienceanalyticsimpactingprocess"></a><span data-ttu-id="3715c-103">Criar userExperienceAnalyticsImpactingProcess</span><span class="sxs-lookup"><span data-stu-id="3715c-103">Create userExperienceAnalyticsImpactingProcess</span></span>

<span data-ttu-id="3715c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3715c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3715c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3715c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3715c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3715c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3715c-107">Crie um novo [objeto userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)</span><span class="sxs-lookup"><span data-stu-id="3715c-107">Create a new [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3715c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3715c-108">Prerequisites</span></span>
<span data-ttu-id="3715c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3715c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3715c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3715c-111">Permission type</span></span>|<span data-ttu-id="3715c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3715c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3715c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3715c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3715c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3715c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3715c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3715c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3715c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3715c-116">Not supported.</span></span>|
|<span data-ttu-id="3715c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3715c-117">Application</span></span>|<span data-ttu-id="3715c-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3715c-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3715c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3715c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsImpactingProcess
```

## <a name="request-headers"></a><span data-ttu-id="3715c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3715c-120">Request headers</span></span>
|<span data-ttu-id="3715c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3715c-121">Header</span></span>|<span data-ttu-id="3715c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3715c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3715c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3715c-123">Authorization</span></span>|<span data-ttu-id="3715c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3715c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3715c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3715c-125">Accept</span></span>|<span data-ttu-id="3715c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3715c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3715c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3715c-127">Request body</span></span>
<span data-ttu-id="3715c-128">No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsImpactingProcess.</span><span class="sxs-lookup"><span data-stu-id="3715c-128">In the request body, supply a JSON representation for the userExperienceAnalyticsImpactingProcess object.</span></span>

<span data-ttu-id="3715c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o userExperienceAnalyticsImpactingProcess.</span><span class="sxs-lookup"><span data-stu-id="3715c-129">The following table shows the properties that are required when you create the userExperienceAnalyticsImpactingProcess.</span></span>

|<span data-ttu-id="3715c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3715c-130">Property</span></span>|<span data-ttu-id="3715c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3715c-131">Type</span></span>|<span data-ttu-id="3715c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3715c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3715c-133">id</span><span class="sxs-lookup"><span data-stu-id="3715c-133">id</span></span>|<span data-ttu-id="3715c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3715c-134">String</span></span>|<span data-ttu-id="3715c-135">O identificador exclusivo da entidade de processo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="3715c-135">The unique identifier of the user experience analytics top impacting process entity.</span></span>|
|<span data-ttu-id="3715c-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="3715c-136">deviceId</span></span>|<span data-ttu-id="3715c-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3715c-137">String</span></span>|<span data-ttu-id="3715c-138">O identificador exclusivo do dispositivo afetado.</span><span class="sxs-lookup"><span data-stu-id="3715c-138">The unique identifier of the impacted device.</span></span>|
|<span data-ttu-id="3715c-139">category</span><span class="sxs-lookup"><span data-stu-id="3715c-139">category</span></span>|<span data-ttu-id="3715c-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3715c-140">String</span></span>|<span data-ttu-id="3715c-141">A categoria do processo de impacto.</span><span class="sxs-lookup"><span data-stu-id="3715c-141">The category of impacting process.</span></span>|
|<span data-ttu-id="3715c-142">processName</span><span class="sxs-lookup"><span data-stu-id="3715c-142">processName</span></span>|<span data-ttu-id="3715c-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3715c-143">String</span></span>|<span data-ttu-id="3715c-144">O nome do processo.</span><span class="sxs-lookup"><span data-stu-id="3715c-144">The process name.</span></span>|
|<span data-ttu-id="3715c-145">descrição</span><span class="sxs-lookup"><span data-stu-id="3715c-145">description</span></span>|<span data-ttu-id="3715c-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3715c-146">String</span></span>|<span data-ttu-id="3715c-147">A descrição do processo.</span><span class="sxs-lookup"><span data-stu-id="3715c-147">The description of process.</span></span>|
|<span data-ttu-id="3715c-148">publicador</span><span class="sxs-lookup"><span data-stu-id="3715c-148">publisher</span></span>|<span data-ttu-id="3715c-149">String</span><span class="sxs-lookup"><span data-stu-id="3715c-149">String</span></span>|<span data-ttu-id="3715c-150">O editor do processo.</span><span class="sxs-lookup"><span data-stu-id="3715c-150">The publisher of the process.</span></span>|
|<span data-ttu-id="3715c-151">impactValue</span><span class="sxs-lookup"><span data-stu-id="3715c-151">impactValue</span></span>|<span data-ttu-id="3715c-152">Duplo</span><span class="sxs-lookup"><span data-stu-id="3715c-152">Double</span></span>|<span data-ttu-id="3715c-153">O valor de impacto do processo.</span><span class="sxs-lookup"><span data-stu-id="3715c-153">The impact value of the process.</span></span> <span data-ttu-id="3715c-154">Valores válidos de 0 a 1,79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="3715c-154">Valid values 0 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="3715c-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="3715c-155">Response</span></span>
<span data-ttu-id="3715c-156">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3715c-156">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3715c-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3715c-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="3715c-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3715c-158">Request</span></span>
<span data-ttu-id="3715c-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3715c-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsImpactingProcess
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

### <a name="response"></a><span data-ttu-id="3715c-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="3715c-160">Response</span></span>
<span data-ttu-id="3715c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3715c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




