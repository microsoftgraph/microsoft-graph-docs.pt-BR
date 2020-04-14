---
title: Atualizar userExperienceAnalyticsScoreHistory
description: Atualiza as propriedades de um objeto userExperienceAnalyticsScoreHistory.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6b44ee2dcbade774c704a7c5d1df1ae31e9423c6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43378823"
---
# <a name="update-userexperienceanalyticsscorehistory"></a><span data-ttu-id="9cc89-103">Atualizar userExperienceAnalyticsScoreHistory</span><span class="sxs-lookup"><span data-stu-id="9cc89-103">Update userExperienceAnalyticsScoreHistory</span></span>

<span data-ttu-id="9cc89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cc89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9cc89-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9cc89-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cc89-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9cc89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cc89-107">Atualiza as propriedades de um objeto [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) .</span><span class="sxs-lookup"><span data-stu-id="9cc89-107">Update the properties of a [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9cc89-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9cc89-108">Prerequisites</span></span>
<span data-ttu-id="9cc89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cc89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cc89-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9cc89-111">Permission type</span></span>|<span data-ttu-id="9cc89-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9cc89-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cc89-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9cc89-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9cc89-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cc89-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9cc89-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9cc89-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cc89-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cc89-116">Not supported.</span></span>|
|<span data-ttu-id="9cc89-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cc89-117">Application</span></span>|<span data-ttu-id="9cc89-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cc89-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cc89-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9cc89-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="9cc89-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc89-120">Request headers</span></span>
|<span data-ttu-id="9cc89-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9cc89-121">Header</span></span>|<span data-ttu-id="9cc89-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9cc89-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cc89-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9cc89-123">Authorization</span></span>|<span data-ttu-id="9cc89-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cc89-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cc89-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9cc89-125">Accept</span></span>|<span data-ttu-id="9cc89-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9cc89-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cc89-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc89-127">Request body</span></span>
<span data-ttu-id="9cc89-128">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) .</span><span class="sxs-lookup"><span data-stu-id="9cc89-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object.</span></span>

<span data-ttu-id="9cc89-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md).</span><span class="sxs-lookup"><span data-stu-id="9cc89-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md).</span></span>

|<span data-ttu-id="9cc89-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9cc89-130">Property</span></span>|<span data-ttu-id="9cc89-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cc89-131">Type</span></span>|<span data-ttu-id="9cc89-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cc89-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cc89-133">id</span><span class="sxs-lookup"><span data-stu-id="9cc89-133">id</span></span>|<span data-ttu-id="9cc89-134">String</span><span class="sxs-lookup"><span data-stu-id="9cc89-134">String</span></span>|<span data-ttu-id="9cc89-135">O identificador exclusivo do processo de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9cc89-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="9cc89-136">startupDateTime</span><span class="sxs-lookup"><span data-stu-id="9cc89-136">startupDateTime</span></span>|<span data-ttu-id="9cc89-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cc89-137">DateTimeOffset</span></span>|<span data-ttu-id="9cc89-138">A experiência do usuário da data de início do dispositivo de análise.</span><span class="sxs-lookup"><span data-stu-id="9cc89-138">The user experience analytics device startup date time.</span></span>|
|<span data-ttu-id="9cc89-139">startupScore</span><span class="sxs-lookup"><span data-stu-id="9cc89-139">startupScore</span></span>|<span data-ttu-id="9cc89-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9cc89-140">Int32</span></span>|<span data-ttu-id="9cc89-141">Pontuação de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9cc89-141">User experience analytics device startup score.</span></span>|
|<span data-ttu-id="9cc89-142">coreBootScore</span><span class="sxs-lookup"><span data-stu-id="9cc89-142">coreBootScore</span></span>|<span data-ttu-id="9cc89-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9cc89-143">Int32</span></span>|<span data-ttu-id="9cc89-144">A pontuação de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9cc89-144">The user experience analytics device core boot score.</span></span>|
|<span data-ttu-id="9cc89-145">coreSigninScore</span><span class="sxs-lookup"><span data-stu-id="9cc89-145">coreSigninScore</span></span>|<span data-ttu-id="9cc89-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9cc89-146">Int32</span></span>|<span data-ttu-id="9cc89-147">A pontuação de entrada do core do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9cc89-147">The User experience analytics device core sign-in score.</span></span>|
|<span data-ttu-id="9cc89-148">recommendedSoftwareScore</span><span class="sxs-lookup"><span data-stu-id="9cc89-148">recommendedSoftwareScore</span></span>|<span data-ttu-id="9cc89-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9cc89-149">Int32</span></span>|<span data-ttu-id="9cc89-150">A pontuação de entrada do core do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9cc89-150">The User experience analytics device core sign-in score.</span></span>|



## <a name="response"></a><span data-ttu-id="9cc89-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cc89-151">Response</span></span>
<span data-ttu-id="9cc89-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9cc89-152">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cc89-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9cc89-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="9cc89-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc89-154">Request</span></span>
<span data-ttu-id="9cc89-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9cc89-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
Content-type: application/json
Content-length: 243

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8
}
```

### <a name="response"></a><span data-ttu-id="9cc89-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cc89-156">Response</span></span>
<span data-ttu-id="9cc89-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9cc89-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 292

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "id": "d15e3ba8-3ba8-d15e-a83b-5ed1a83b5ed1",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8
}
```



