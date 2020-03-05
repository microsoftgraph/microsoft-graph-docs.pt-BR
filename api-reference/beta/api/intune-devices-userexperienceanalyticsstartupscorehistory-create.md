---
title: Criar userExperienceAnalyticsStartupScoreHistory
description: Criar um novo objeto userExperienceAnalyticsStartupScoreHistory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fd2dfad7eecfd373c6fa92c8b1023200b08a61d8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468044"
---
# <a name="create-userexperienceanalyticsstartupscorehistory"></a><span data-ttu-id="11e09-103">Criar userExperienceAnalyticsStartupScoreHistory</span><span class="sxs-lookup"><span data-stu-id="11e09-103">Create userExperienceAnalyticsStartupScoreHistory</span></span>

<span data-ttu-id="11e09-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="11e09-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11e09-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="11e09-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11e09-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="11e09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11e09-107">Criar um novo objeto [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) .</span><span class="sxs-lookup"><span data-stu-id="11e09-107">Create a new [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11e09-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="11e09-108">Prerequisites</span></span>
<span data-ttu-id="11e09-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11e09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11e09-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11e09-111">Permission type</span></span>|<span data-ttu-id="11e09-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="11e09-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11e09-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11e09-113">Delegated (work or school account)</span></span>|<span data-ttu-id="11e09-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11e09-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="11e09-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11e09-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11e09-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11e09-116">Not supported.</span></span>|
|<span data-ttu-id="11e09-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11e09-117">Application</span></span>|<span data-ttu-id="11e09-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11e09-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="11e09-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11e09-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsStartupScoreHistory
```

## <a name="request-headers"></a><span data-ttu-id="11e09-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11e09-120">Request headers</span></span>
|<span data-ttu-id="11e09-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="11e09-121">Header</span></span>|<span data-ttu-id="11e09-122">Valor</span><span class="sxs-lookup"><span data-stu-id="11e09-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11e09-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="11e09-123">Authorization</span></span>|<span data-ttu-id="11e09-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11e09-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11e09-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="11e09-125">Accept</span></span>|<span data-ttu-id="11e09-126">application/json</span><span class="sxs-lookup"><span data-stu-id="11e09-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11e09-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11e09-127">Request body</span></span>
<span data-ttu-id="11e09-128">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsStartupScoreHistory.</span><span class="sxs-lookup"><span data-stu-id="11e09-128">In the request body, supply a JSON representation for the userExperienceAnalyticsStartupScoreHistory object.</span></span>

<span data-ttu-id="11e09-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsStartupScoreHistory.</span><span class="sxs-lookup"><span data-stu-id="11e09-129">The following table shows the properties that are required when you create the userExperienceAnalyticsStartupScoreHistory.</span></span>

|<span data-ttu-id="11e09-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11e09-130">Property</span></span>|<span data-ttu-id="11e09-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="11e09-131">Type</span></span>|<span data-ttu-id="11e09-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="11e09-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11e09-133">id</span><span class="sxs-lookup"><span data-stu-id="11e09-133">id</span></span>|<span data-ttu-id="11e09-134">String</span><span class="sxs-lookup"><span data-stu-id="11e09-134">String</span></span>|<span data-ttu-id="11e09-135">O identificador exclusivo do processo de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="11e09-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="11e09-136">startupDateTime</span><span class="sxs-lookup"><span data-stu-id="11e09-136">startupDateTime</span></span>|<span data-ttu-id="11e09-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11e09-137">DateTimeOffset</span></span>|<span data-ttu-id="11e09-138">A experiência do usuário da data de início do dispositivo de análise.</span><span class="sxs-lookup"><span data-stu-id="11e09-138">The user experience analytics device startup date time.</span></span>|
|<span data-ttu-id="11e09-139">startupScore</span><span class="sxs-lookup"><span data-stu-id="11e09-139">startupScore</span></span>|<span data-ttu-id="11e09-140">Int32</span><span class="sxs-lookup"><span data-stu-id="11e09-140">Int32</span></span>|<span data-ttu-id="11e09-141">Pontuação de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="11e09-141">User experience analytics device startup score.</span></span>|
|<span data-ttu-id="11e09-142">coreBootScore</span><span class="sxs-lookup"><span data-stu-id="11e09-142">coreBootScore</span></span>|<span data-ttu-id="11e09-143">Int32</span><span class="sxs-lookup"><span data-stu-id="11e09-143">Int32</span></span>|<span data-ttu-id="11e09-144">A pontuação de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="11e09-144">The user experience analytics device core boot score.</span></span>|
|<span data-ttu-id="11e09-145">coreSigninScore</span><span class="sxs-lookup"><span data-stu-id="11e09-145">coreSigninScore</span></span>|<span data-ttu-id="11e09-146">Int32</span><span class="sxs-lookup"><span data-stu-id="11e09-146">Int32</span></span>|<span data-ttu-id="11e09-147">A pontuação de entrada do core do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="11e09-147">The User experience analytics device core sign-in score.</span></span>|



## <a name="response"></a><span data-ttu-id="11e09-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="11e09-148">Response</span></span>
<span data-ttu-id="11e09-149">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11e09-149">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11e09-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11e09-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="11e09-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11e09-151">Request</span></span>
<span data-ttu-id="11e09-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11e09-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsStartupScoreHistory
Content-type: application/json
Content-length: 216

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsStartupScoreHistory",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15
}
```

### <a name="response"></a><span data-ttu-id="11e09-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="11e09-153">Response</span></span>
<span data-ttu-id="11e09-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11e09-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 265

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsStartupScoreHistory",
  "id": "52efee0b-ee0b-52ef-0bee-ef520beeef52",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15
}
```





