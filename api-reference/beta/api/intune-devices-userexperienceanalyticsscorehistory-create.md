---
title: Criar userExperienceAnalyticsScoreHistory
description: Crie um novo objeto userExperienceAnalyticsScoreHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2cee5d19742711a4ea6f0858d3054337fabf3309
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52663807"
---
# <a name="create-userexperienceanalyticsscorehistory"></a><span data-ttu-id="3ce85-103">Criar userExperienceAnalyticsScoreHistory</span><span class="sxs-lookup"><span data-stu-id="3ce85-103">Create userExperienceAnalyticsScoreHistory</span></span>

<span data-ttu-id="3ce85-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ce85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ce85-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3ce85-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ce85-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3ce85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ce85-107">Crie um novo [objeto userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)</span><span class="sxs-lookup"><span data-stu-id="3ce85-107">Create a new [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ce85-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3ce85-108">Prerequisites</span></span>
<span data-ttu-id="3ce85-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ce85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ce85-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ce85-111">Permission type</span></span>|<span data-ttu-id="3ce85-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ce85-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ce85-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ce85-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3ce85-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ce85-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3ce85-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ce85-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ce85-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ce85-116">Not supported.</span></span>|
|<span data-ttu-id="3ce85-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ce85-117">Application</span></span>|<span data-ttu-id="3ce85-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ce85-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ce85-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ce85-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsScoreHistory
```

## <a name="request-headers"></a><span data-ttu-id="3ce85-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ce85-120">Request headers</span></span>
|<span data-ttu-id="3ce85-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3ce85-121">Header</span></span>|<span data-ttu-id="3ce85-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3ce85-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ce85-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ce85-123">Authorization</span></span>|<span data-ttu-id="3ce85-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ce85-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ce85-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3ce85-125">Accept</span></span>|<span data-ttu-id="3ce85-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ce85-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ce85-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ce85-127">Request body</span></span>
<span data-ttu-id="3ce85-128">No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsScoreHistory.</span><span class="sxs-lookup"><span data-stu-id="3ce85-128">In the request body, supply a JSON representation for the userExperienceAnalyticsScoreHistory object.</span></span>

<span data-ttu-id="3ce85-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o userExperienceAnalyticsScoreHistory.</span><span class="sxs-lookup"><span data-stu-id="3ce85-129">The following table shows the properties that are required when you create the userExperienceAnalyticsScoreHistory.</span></span>

|<span data-ttu-id="3ce85-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ce85-130">Property</span></span>|<span data-ttu-id="3ce85-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ce85-131">Type</span></span>|<span data-ttu-id="3ce85-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ce85-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ce85-133">id</span><span class="sxs-lookup"><span data-stu-id="3ce85-133">id</span></span>|<span data-ttu-id="3ce85-134">String</span><span class="sxs-lookup"><span data-stu-id="3ce85-134">String</span></span>|<span data-ttu-id="3ce85-135">O identificador exclusivo do processo de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="3ce85-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="3ce85-136">startupDateTime</span><span class="sxs-lookup"><span data-stu-id="3ce85-136">startupDateTime</span></span>|<span data-ttu-id="3ce85-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ce85-137">DateTimeOffset</span></span>|<span data-ttu-id="3ce85-138">A data de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="3ce85-138">The user experience analytics device startup date time.</span></span>|
|<span data-ttu-id="3ce85-139">overallScore</span><span class="sxs-lookup"><span data-stu-id="3ce85-139">overallScore</span></span>|<span data-ttu-id="3ce85-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3ce85-140">Int32</span></span>|<span data-ttu-id="3ce85-141">Pontuação geral da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="3ce85-141">User experience analytics overall score.</span></span> <span data-ttu-id="3ce85-142">A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal.</span><span class="sxs-lookup"><span data-stu-id="3ce85-142">Score will be in the range 0-100, 100 is the ideal score.</span></span> <span data-ttu-id="3ce85-143">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="3ce85-143">Valid values 0 to 100</span></span>|
|<span data-ttu-id="3ce85-144">startupScore</span><span class="sxs-lookup"><span data-stu-id="3ce85-144">startupScore</span></span>|<span data-ttu-id="3ce85-145">Int32</span><span class="sxs-lookup"><span data-stu-id="3ce85-145">Int32</span></span>|<span data-ttu-id="3ce85-146">Pontuação de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="3ce85-146">User experience analytics device startup score.</span></span> <span data-ttu-id="3ce85-147">A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal.</span><span class="sxs-lookup"><span data-stu-id="3ce85-147">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="3ce85-148">coreBootScore</span><span class="sxs-lookup"><span data-stu-id="3ce85-148">coreBootScore</span></span>|<span data-ttu-id="3ce85-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3ce85-149">Int32</span></span>|<span data-ttu-id="3ce85-150">A pontuação de inicialização principal do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="3ce85-150">The user experience analytics device core boot score.</span></span> <span data-ttu-id="3ce85-151">A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal.</span><span class="sxs-lookup"><span data-stu-id="3ce85-151">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="3ce85-152">coreSigninScore</span><span class="sxs-lookup"><span data-stu-id="3ce85-152">coreSigninScore</span></span>|<span data-ttu-id="3ce85-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3ce85-153">Int32</span></span>|<span data-ttu-id="3ce85-154">A pontuação de entrada principal do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="3ce85-154">The User experience analytics device core sign-in score.</span></span> <span data-ttu-id="3ce85-155">A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal.</span><span class="sxs-lookup"><span data-stu-id="3ce85-155">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="3ce85-156">recommendedSoftwareScore</span><span class="sxs-lookup"><span data-stu-id="3ce85-156">recommendedSoftwareScore</span></span>|<span data-ttu-id="3ce85-157">Int32</span><span class="sxs-lookup"><span data-stu-id="3ce85-157">Int32</span></span>|<span data-ttu-id="3ce85-158">A pontuação de entrada principal do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="3ce85-158">The User experience analytics device core sign-in score.</span></span> <span data-ttu-id="3ce85-159">A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal.</span><span class="sxs-lookup"><span data-stu-id="3ce85-159">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="3ce85-160">restartScore</span><span class="sxs-lookup"><span data-stu-id="3ce85-160">restartScore</span></span>|<span data-ttu-id="3ce85-161">Int32</span><span class="sxs-lookup"><span data-stu-id="3ce85-161">Int32</span></span>|<span data-ttu-id="3ce85-162">Reinicie a pontuação.</span><span class="sxs-lookup"><span data-stu-id="3ce85-162">Restart score.</span></span> <span data-ttu-id="3ce85-163">A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal, 0 indica reinicializações excessivas.</span><span class="sxs-lookup"><span data-stu-id="3ce85-163">Score will be in the range 0-100, 100 is the ideal score, 0 indicates excessive restarts.</span></span> <span data-ttu-id="3ce85-164">Valores válidos de 0 a 9999999</span><span class="sxs-lookup"><span data-stu-id="3ce85-164">Valid values 0 to 9999999</span></span>|



## <a name="response"></a><span data-ttu-id="3ce85-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ce85-165">Response</span></span>
<span data-ttu-id="3ce85-166">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ce85-166">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ce85-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ce85-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ce85-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ce85-168">Request</span></span>
<span data-ttu-id="3ce85-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ce85-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory
Content-type: application/json
Content-length: 289

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "overallScore": 12,
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "restartScore": 12
}
```

### <a name="response"></a><span data-ttu-id="3ce85-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ce85-170">Response</span></span>
<span data-ttu-id="3ce85-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ce85-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 338

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "id": "d15e3ba8-3ba8-d15e-a83b-5ed1a83b5ed1",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "overallScore": 12,
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "restartScore": 12
}
```




