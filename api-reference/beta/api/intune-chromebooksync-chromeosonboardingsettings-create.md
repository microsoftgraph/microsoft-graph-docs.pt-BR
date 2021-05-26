---
title: Criar chromeOSOnboardingSettings
description: Crie um novo objeto chromeOSOnboardingSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a359b9bd0f638e147af8119ee7ca07a27db0c2e8
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665658"
---
# <a name="create-chromeosonboardingsettings"></a><span data-ttu-id="fc8df-103">Criar chromeOSOnboardingSettings</span><span class="sxs-lookup"><span data-stu-id="fc8df-103">Create chromeOSOnboardingSettings</span></span>

<span data-ttu-id="fc8df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc8df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc8df-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fc8df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc8df-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fc8df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc8df-107">Crie um novo [objeto chromeOSOnboardingSettings.](../resources/intune-chromebooksync-chromeosonboardingsettings.md)</span><span class="sxs-lookup"><span data-stu-id="fc8df-107">Create a new [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc8df-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fc8df-108">Prerequisites</span></span>
<span data-ttu-id="fc8df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc8df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc8df-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc8df-111">Permission type</span></span>|<span data-ttu-id="fc8df-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc8df-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc8df-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc8df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc8df-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc8df-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fc8df-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc8df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc8df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc8df-116">Not supported.</span></span>|
|<span data-ttu-id="fc8df-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc8df-117">Application</span></span>|<span data-ttu-id="fc8df-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc8df-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc8df-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc8df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/chromeOSOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="fc8df-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc8df-120">Request headers</span></span>
|<span data-ttu-id="fc8df-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fc8df-121">Header</span></span>|<span data-ttu-id="fc8df-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fc8df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc8df-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc8df-123">Authorization</span></span>|<span data-ttu-id="fc8df-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc8df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc8df-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fc8df-125">Accept</span></span>|<span data-ttu-id="fc8df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fc8df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc8df-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc8df-127">Request body</span></span>
<span data-ttu-id="fc8df-128">No corpo da solicitação, fornece uma representação JSON para o objeto chromeOSOnboardingSettings.</span><span class="sxs-lookup"><span data-stu-id="fc8df-128">In the request body, supply a JSON representation for the chromeOSOnboardingSettings object.</span></span>

<span data-ttu-id="fc8df-129">A tabela a seguir mostra as propriedades que são necessárias ao criar os chromeOSOnboardingSettings.</span><span class="sxs-lookup"><span data-stu-id="fc8df-129">The following table shows the properties that are required when you create the chromeOSOnboardingSettings.</span></span>

|<span data-ttu-id="fc8df-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc8df-130">Property</span></span>|<span data-ttu-id="fc8df-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc8df-131">Type</span></span>|<span data-ttu-id="fc8df-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc8df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc8df-133">id</span><span class="sxs-lookup"><span data-stu-id="fc8df-133">id</span></span>|<span data-ttu-id="fc8df-134">String</span><span class="sxs-lookup"><span data-stu-id="fc8df-134">String</span></span>|<span data-ttu-id="fc8df-135">A ID do ChromebookTenant</span><span class="sxs-lookup"><span data-stu-id="fc8df-135">The ChromebookTenant's Id</span></span>|
|<span data-ttu-id="fc8df-136">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fc8df-136">ownerUserPrincipalName</span></span>|<span data-ttu-id="fc8df-137">String</span><span class="sxs-lookup"><span data-stu-id="fc8df-137">String</span></span>|<span data-ttu-id="fc8df-138">OwnerUserPrincipalName do ChromebookTenant</span><span class="sxs-lookup"><span data-stu-id="fc8df-138">The ChromebookTenant's OwnerUserPrincipalName</span></span>|
|<span data-ttu-id="fc8df-139">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="fc8df-139">onboardingStatus</span></span>|[<span data-ttu-id="fc8df-140">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="fc8df-140">onboardingStatus</span></span>](../resources/intune-chromebooksync-onboardingstatus.md)|<span data-ttu-id="fc8df-141">OnboardingStatus do ChromebookTenant.</span><span class="sxs-lookup"><span data-stu-id="fc8df-141">The ChromebookTenant's OnboardingStatus.</span></span> <span data-ttu-id="fc8df-142">Os valores possíveis são: `unknown`, `inprogress`, `onboarded`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="fc8df-142">Possible values are: `unknown`, `inprogress`, `onboarded`, `failed`.</span></span>|
|<span data-ttu-id="fc8df-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc8df-143">lastModifiedDateTime</span></span>|<span data-ttu-id="fc8df-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc8df-144">DateTimeOffset</span></span>|<span data-ttu-id="fc8df-145">LastModifiedDateTime do ChromebookTenant</span><span class="sxs-lookup"><span data-stu-id="fc8df-145">The ChromebookTenant's LastModifiedDateTime</span></span>|
|<span data-ttu-id="fc8df-146">lastDirectorySyncDateTime</span><span class="sxs-lookup"><span data-stu-id="fc8df-146">lastDirectorySyncDateTime</span></span>|<span data-ttu-id="fc8df-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc8df-147">DateTimeOffset</span></span>|<span data-ttu-id="fc8df-148">LastDirectorySyncDateTime do ChromebookTenant</span><span class="sxs-lookup"><span data-stu-id="fc8df-148">The ChromebookTenant's LastDirectorySyncDateTime</span></span>|



## <a name="response"></a><span data-ttu-id="fc8df-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc8df-149">Response</span></span>
<span data-ttu-id="fc8df-150">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc8df-150">If successful, this method returns a `201 Created` response code and a [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc8df-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc8df-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc8df-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc8df-152">Request</span></span>
<span data-ttu-id="fc8df-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc8df-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/chromeOSOnboardingSettings
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.chromeOSOnboardingSettings",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "onboardingStatus": "inprogress",
  "lastDirectorySyncDateTime": "2016-12-31T23:57:56.1183185-08:00"
}
```

### <a name="response"></a><span data-ttu-id="fc8df-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc8df-154">Response</span></span>
<span data-ttu-id="fc8df-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc8df-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 351

{
  "@odata.type": "#microsoft.graph.chromeOSOnboardingSettings",
  "id": "0344255d-255d-0344-5d25-44035d254403",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "onboardingStatus": "inprogress",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastDirectorySyncDateTime": "2016-12-31T23:57:56.1183185-08:00"
}
```




