---
title: Criar userExperienceAnalyticsScoreHistory
description: Criar um novo objeto userExperienceAnalyticsScoreHistory.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f1a6d5275a8214f5698a41a711c1b82b1e48b960
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792657"
---
# <a name="create-userexperienceanalyticsscorehistory"></a><span data-ttu-id="e3865-103">Criar userExperienceAnalyticsScoreHistory</span><span class="sxs-lookup"><span data-stu-id="e3865-103">Create userExperienceAnalyticsScoreHistory</span></span>

<span data-ttu-id="e3865-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3865-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3865-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e3865-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3865-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e3865-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3865-107">Criar um novo objeto [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) .</span><span class="sxs-lookup"><span data-stu-id="e3865-107">Create a new [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3865-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e3865-108">Prerequisites</span></span>
<span data-ttu-id="e3865-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3865-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3865-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3865-111">Permission type</span></span>|<span data-ttu-id="e3865-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e3865-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3865-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3865-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3865-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3865-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e3865-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3865-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3865-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3865-116">Not supported.</span></span>|
|<span data-ttu-id="e3865-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3865-117">Application</span></span>|<span data-ttu-id="e3865-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3865-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3865-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3865-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsScoreHistory
```

## <a name="request-headers"></a><span data-ttu-id="e3865-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3865-120">Request headers</span></span>
|<span data-ttu-id="e3865-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e3865-121">Header</span></span>|<span data-ttu-id="e3865-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e3865-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3865-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3865-123">Authorization</span></span>|<span data-ttu-id="e3865-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3865-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3865-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e3865-125">Accept</span></span>|<span data-ttu-id="e3865-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3865-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3865-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3865-127">Request body</span></span>
<span data-ttu-id="e3865-128">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsScoreHistory.</span><span class="sxs-lookup"><span data-stu-id="e3865-128">In the request body, supply a JSON representation for the userExperienceAnalyticsScoreHistory object.</span></span>

<span data-ttu-id="e3865-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsScoreHistory.</span><span class="sxs-lookup"><span data-stu-id="e3865-129">The following table shows the properties that are required when you create the userExperienceAnalyticsScoreHistory.</span></span>

|<span data-ttu-id="e3865-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3865-130">Property</span></span>|<span data-ttu-id="e3865-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3865-131">Type</span></span>|<span data-ttu-id="e3865-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3865-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3865-133">id</span><span class="sxs-lookup"><span data-stu-id="e3865-133">id</span></span>|<span data-ttu-id="e3865-134">String</span><span class="sxs-lookup"><span data-stu-id="e3865-134">String</span></span>|<span data-ttu-id="e3865-135">O identificador exclusivo do processo de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e3865-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="e3865-136">startupDateTime</span><span class="sxs-lookup"><span data-stu-id="e3865-136">startupDateTime</span></span>|<span data-ttu-id="e3865-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3865-137">DateTimeOffset</span></span>|<span data-ttu-id="e3865-138">A experiência do usuário da data de início do dispositivo de análise.</span><span class="sxs-lookup"><span data-stu-id="e3865-138">The user experience analytics device startup date time.</span></span>|
|<span data-ttu-id="e3865-139">startupScore</span><span class="sxs-lookup"><span data-stu-id="e3865-139">startupScore</span></span>|<span data-ttu-id="e3865-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e3865-140">Int32</span></span>|<span data-ttu-id="e3865-141">Pontuação de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e3865-141">User experience analytics device startup score.</span></span> <span data-ttu-id="e3865-142">A pontuação será no intervalo 0-100, 100 é a pontuação ideal.</span><span class="sxs-lookup"><span data-stu-id="e3865-142">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="e3865-143">coreBootScore</span><span class="sxs-lookup"><span data-stu-id="e3865-143">coreBootScore</span></span>|<span data-ttu-id="e3865-144">Int32</span><span class="sxs-lookup"><span data-stu-id="e3865-144">Int32</span></span>|<span data-ttu-id="e3865-145">A pontuação de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e3865-145">The user experience analytics device core boot score.</span></span> <span data-ttu-id="e3865-146">A pontuação será no intervalo 0-100, 100 é a pontuação ideal.</span><span class="sxs-lookup"><span data-stu-id="e3865-146">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="e3865-147">coreSigninScore</span><span class="sxs-lookup"><span data-stu-id="e3865-147">coreSigninScore</span></span>|<span data-ttu-id="e3865-148">Int32</span><span class="sxs-lookup"><span data-stu-id="e3865-148">Int32</span></span>|<span data-ttu-id="e3865-149">A pontuação de entrada do core do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e3865-149">The User experience analytics device core sign-in score.</span></span> <span data-ttu-id="e3865-150">A pontuação será no intervalo 0-100, 100 é a pontuação ideal.</span><span class="sxs-lookup"><span data-stu-id="e3865-150">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="e3865-151">recommendedSoftwareScore</span><span class="sxs-lookup"><span data-stu-id="e3865-151">recommendedSoftwareScore</span></span>|<span data-ttu-id="e3865-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e3865-152">Int32</span></span>|<span data-ttu-id="e3865-153">A pontuação de entrada do core do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e3865-153">The User experience analytics device core sign-in score.</span></span> <span data-ttu-id="e3865-154">A pontuação será no intervalo 0-100, 100 é a pontuação ideal.</span><span class="sxs-lookup"><span data-stu-id="e3865-154">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="e3865-155">restartScore</span><span class="sxs-lookup"><span data-stu-id="e3865-155">restartScore</span></span>|<span data-ttu-id="e3865-156">Int32</span><span class="sxs-lookup"><span data-stu-id="e3865-156">Int32</span></span>|<span data-ttu-id="e3865-157">Reinicie o placar.</span><span class="sxs-lookup"><span data-stu-id="e3865-157">Restart score.</span></span> <span data-ttu-id="e3865-158">A pontuação será no intervalo 0-100, 100 é a pontuação ideal, 0 indica reinicializações em excesso.</span><span class="sxs-lookup"><span data-stu-id="e3865-158">Score will be in the range 0-100, 100 is the ideal score, 0 indicates excessive restarts.</span></span> <span data-ttu-id="e3865-159">Valores válidos de 0 a 9999999</span><span class="sxs-lookup"><span data-stu-id="e3865-159">Valid values 0 to 9999999</span></span>|



## <a name="response"></a><span data-ttu-id="e3865-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3865-160">Response</span></span>
<span data-ttu-id="e3865-161">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3865-161">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3865-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3865-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3865-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3865-163">Request</span></span>
<span data-ttu-id="e3865-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3865-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "restartScore": 12
}
```

### <a name="response"></a><span data-ttu-id="e3865-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3865-165">Response</span></span>
<span data-ttu-id="e3865-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3865-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 315

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "id": "d15e3ba8-3ba8-d15e-a83b-5ed1a83b5ed1",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "restartScore": 12
}
```



