---
title: Criar userExperienceAnalyticsScoreHistory
description: Crie um novo objeto userExperienceAnalyticsScoreHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f161e58e8ce571d0c4f83e6dcf7b77683e94d70d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146157"
---
# <a name="create-userexperienceanalyticsscorehistory"></a><span data-ttu-id="fb774-103">Criar userExperienceAnalyticsScoreHistory</span><span class="sxs-lookup"><span data-stu-id="fb774-103">Create userExperienceAnalyticsScoreHistory</span></span>

<span data-ttu-id="fb774-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb774-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb774-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fb774-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb774-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fb774-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb774-107">Crie um novo [objeto userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)</span><span class="sxs-lookup"><span data-stu-id="fb774-107">Create a new [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb774-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fb774-108">Prerequisites</span></span>
<span data-ttu-id="fb774-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb774-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb774-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb774-111">Permission type</span></span>|<span data-ttu-id="fb774-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb774-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb774-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb774-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb774-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb774-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fb774-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb774-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb774-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb774-116">Not supported.</span></span>|
|<span data-ttu-id="fb774-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb774-117">Application</span></span>|<span data-ttu-id="fb774-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb774-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb774-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb774-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsScoreHistory
```

## <a name="request-headers"></a><span data-ttu-id="fb774-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb774-120">Request headers</span></span>
|<span data-ttu-id="fb774-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb774-121">Header</span></span>|<span data-ttu-id="fb774-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fb774-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb774-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb774-123">Authorization</span></span>|<span data-ttu-id="fb774-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb774-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb774-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fb774-125">Accept</span></span>|<span data-ttu-id="fb774-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb774-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb774-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb774-127">Request body</span></span>
<span data-ttu-id="fb774-128">No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsScoreHistory.</span><span class="sxs-lookup"><span data-stu-id="fb774-128">In the request body, supply a JSON representation for the userExperienceAnalyticsScoreHistory object.</span></span>

<span data-ttu-id="fb774-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o userExperienceAnalyticsScoreHistory.</span><span class="sxs-lookup"><span data-stu-id="fb774-129">The following table shows the properties that are required when you create the userExperienceAnalyticsScoreHistory.</span></span>

|<span data-ttu-id="fb774-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb774-130">Property</span></span>|<span data-ttu-id="fb774-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb774-131">Type</span></span>|<span data-ttu-id="fb774-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb774-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb774-133">id</span><span class="sxs-lookup"><span data-stu-id="fb774-133">id</span></span>|<span data-ttu-id="fb774-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb774-134">String</span></span>|<span data-ttu-id="fb774-135">O identificador exclusivo do processo de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="fb774-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="fb774-136">startupDateTime</span><span class="sxs-lookup"><span data-stu-id="fb774-136">startupDateTime</span></span>|<span data-ttu-id="fb774-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb774-137">DateTimeOffset</span></span>|<span data-ttu-id="fb774-138">A data de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="fb774-138">The user experience analytics device startup date time.</span></span>|
|<span data-ttu-id="fb774-139">startupScore</span><span class="sxs-lookup"><span data-stu-id="fb774-139">startupScore</span></span>|<span data-ttu-id="fb774-140">Int32</span><span class="sxs-lookup"><span data-stu-id="fb774-140">Int32</span></span>|<span data-ttu-id="fb774-141">Pontuação de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="fb774-141">User experience analytics device startup score.</span></span> <span data-ttu-id="fb774-142">A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal.</span><span class="sxs-lookup"><span data-stu-id="fb774-142">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="fb774-143">coreBootScore</span><span class="sxs-lookup"><span data-stu-id="fb774-143">coreBootScore</span></span>|<span data-ttu-id="fb774-144">Int32</span><span class="sxs-lookup"><span data-stu-id="fb774-144">Int32</span></span>|<span data-ttu-id="fb774-145">A pontuação de inicialização principal do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="fb774-145">The user experience analytics device core boot score.</span></span> <span data-ttu-id="fb774-146">A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal.</span><span class="sxs-lookup"><span data-stu-id="fb774-146">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="fb774-147">coreSigninScore</span><span class="sxs-lookup"><span data-stu-id="fb774-147">coreSigninScore</span></span>|<span data-ttu-id="fb774-148">Int32</span><span class="sxs-lookup"><span data-stu-id="fb774-148">Int32</span></span>|<span data-ttu-id="fb774-149">A pontuação de entrada principal do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="fb774-149">The User experience analytics device core sign-in score.</span></span> <span data-ttu-id="fb774-150">A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal.</span><span class="sxs-lookup"><span data-stu-id="fb774-150">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="fb774-151">recommendedSoftwareScore</span><span class="sxs-lookup"><span data-stu-id="fb774-151">recommendedSoftwareScore</span></span>|<span data-ttu-id="fb774-152">Int32</span><span class="sxs-lookup"><span data-stu-id="fb774-152">Int32</span></span>|<span data-ttu-id="fb774-153">A pontuação de entrada principal do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="fb774-153">The User experience analytics device core sign-in score.</span></span> <span data-ttu-id="fb774-154">A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal.</span><span class="sxs-lookup"><span data-stu-id="fb774-154">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="fb774-155">restartScore</span><span class="sxs-lookup"><span data-stu-id="fb774-155">restartScore</span></span>|<span data-ttu-id="fb774-156">Int32</span><span class="sxs-lookup"><span data-stu-id="fb774-156">Int32</span></span>|<span data-ttu-id="fb774-157">Reinicie a pontuação.</span><span class="sxs-lookup"><span data-stu-id="fb774-157">Restart score.</span></span> <span data-ttu-id="fb774-158">A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal, 0 indica reinicializações excessivas.</span><span class="sxs-lookup"><span data-stu-id="fb774-158">Score will be in the range 0-100, 100 is the ideal score, 0 indicates excessive restarts.</span></span> <span data-ttu-id="fb774-159">Valores válidos de 0 a 9999999</span><span class="sxs-lookup"><span data-stu-id="fb774-159">Valid values 0 to 9999999</span></span>|



## <a name="response"></a><span data-ttu-id="fb774-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb774-160">Response</span></span>
<span data-ttu-id="fb774-161">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb774-161">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb774-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb774-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb774-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb774-163">Request</span></span>
<span data-ttu-id="fb774-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb774-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fb774-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb774-165">Response</span></span>
<span data-ttu-id="fb774-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb774-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




