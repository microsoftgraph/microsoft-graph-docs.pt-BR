---
title: Atualizar userExperienceAnalyticsStartupScoreHistory
description: Atualiza as propriedades de um objeto userExperienceAnalyticsStartupScoreHistory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3b3c49164ef636ad7822ca4c82bd81802ea37431
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160830"
---
# <a name="update-userexperienceanalyticsstartupscorehistory"></a><span data-ttu-id="52bde-103">Atualizar userExperienceAnalyticsStartupScoreHistory</span><span class="sxs-lookup"><span data-stu-id="52bde-103">Update userExperienceAnalyticsStartupScoreHistory</span></span>

> <span data-ttu-id="52bde-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="52bde-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52bde-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52bde-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52bde-106">Atualiza as propriedades de um objeto [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) .</span><span class="sxs-lookup"><span data-stu-id="52bde-106">Update the properties of a [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52bde-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="52bde-107">Prerequisites</span></span>
<span data-ttu-id="52bde-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52bde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52bde-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52bde-110">Permission type</span></span>|<span data-ttu-id="52bde-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="52bde-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52bde-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52bde-112">Delegated (work or school account)</span></span>|<span data-ttu-id="52bde-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52bde-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="52bde-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52bde-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52bde-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52bde-115">Not supported.</span></span>|
|<span data-ttu-id="52bde-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52bde-116">Application</span></span>|<span data-ttu-id="52bde-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52bde-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52bde-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52bde-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsStartupScoreHistory/{userExperienceAnalyticsStartupScoreHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="52bde-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52bde-119">Request headers</span></span>
|<span data-ttu-id="52bde-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="52bde-120">Header</span></span>|<span data-ttu-id="52bde-121">Valor</span><span class="sxs-lookup"><span data-stu-id="52bde-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52bde-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="52bde-122">Authorization</span></span>|<span data-ttu-id="52bde-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52bde-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52bde-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="52bde-124">Accept</span></span>|<span data-ttu-id="52bde-125">application/json</span><span class="sxs-lookup"><span data-stu-id="52bde-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52bde-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52bde-126">Request body</span></span>
<span data-ttu-id="52bde-127">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) .</span><span class="sxs-lookup"><span data-stu-id="52bde-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object.</span></span>

<span data-ttu-id="52bde-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md).</span><span class="sxs-lookup"><span data-stu-id="52bde-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md).</span></span>

|<span data-ttu-id="52bde-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52bde-129">Property</span></span>|<span data-ttu-id="52bde-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="52bde-130">Type</span></span>|<span data-ttu-id="52bde-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="52bde-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52bde-132">id</span><span class="sxs-lookup"><span data-stu-id="52bde-132">id</span></span>|<span data-ttu-id="52bde-133">String</span><span class="sxs-lookup"><span data-stu-id="52bde-133">String</span></span>|<span data-ttu-id="52bde-134">O identificador exclusivo do processo de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="52bde-134">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="52bde-135">startupDateTime</span><span class="sxs-lookup"><span data-stu-id="52bde-135">startupDateTime</span></span>|<span data-ttu-id="52bde-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52bde-136">DateTimeOffset</span></span>|<span data-ttu-id="52bde-137">A experiência do usuário da data de início do dispositivo de análise.</span><span class="sxs-lookup"><span data-stu-id="52bde-137">The user experience analytics device startup date time.</span></span>|
|<span data-ttu-id="52bde-138">startupScore</span><span class="sxs-lookup"><span data-stu-id="52bde-138">startupScore</span></span>|<span data-ttu-id="52bde-139">Int32</span><span class="sxs-lookup"><span data-stu-id="52bde-139">Int32</span></span>|<span data-ttu-id="52bde-140">Pontuação de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="52bde-140">User experience analytics device startup score.</span></span>|
|<span data-ttu-id="52bde-141">coreBootScore</span><span class="sxs-lookup"><span data-stu-id="52bde-141">coreBootScore</span></span>|<span data-ttu-id="52bde-142">Int32</span><span class="sxs-lookup"><span data-stu-id="52bde-142">Int32</span></span>|<span data-ttu-id="52bde-143">A pontuação de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="52bde-143">The user experience analytics device core boot score.</span></span>|
|<span data-ttu-id="52bde-144">coreSigninScore</span><span class="sxs-lookup"><span data-stu-id="52bde-144">coreSigninScore</span></span>|<span data-ttu-id="52bde-145">Int32</span><span class="sxs-lookup"><span data-stu-id="52bde-145">Int32</span></span>|<span data-ttu-id="52bde-146">A pontuação de entrada do core do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="52bde-146">The User experience analytics device core sign-in score.</span></span>|



## <a name="response"></a><span data-ttu-id="52bde-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="52bde-147">Response</span></span>
<span data-ttu-id="52bde-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52bde-148">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52bde-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52bde-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="52bde-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52bde-150">Request</span></span>
<span data-ttu-id="52bde-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52bde-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsStartupScoreHistory/{userExperienceAnalyticsStartupScoreHistoryId}
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

### <a name="response"></a><span data-ttu-id="52bde-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="52bde-152">Response</span></span>
<span data-ttu-id="52bde-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52bde-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





