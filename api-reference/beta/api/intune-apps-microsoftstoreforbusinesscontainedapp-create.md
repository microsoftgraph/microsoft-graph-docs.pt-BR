---
title: Criar microsoftStoreForBusinessContainedApp
description: Criar um novo objeto microsoftStoreForBusinessContainedApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1f068fc347ebc0352ccaf9e627cc3cfb35f57721
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43404916"
---
# <a name="create-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="5cdf5-103">Criar microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="5cdf5-103">Create microsoftStoreForBusinessContainedApp</span></span>

<span data-ttu-id="5cdf5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cdf5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5cdf5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5cdf5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5cdf5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5cdf5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cdf5-107">Criar um novo objeto [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="5cdf5-107">Create a new [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5cdf5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5cdf5-108">Prerequisites</span></span>
<span data-ttu-id="5cdf5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cdf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cdf5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5cdf5-111">Permission type</span></span>|<span data-ttu-id="5cdf5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5cdf5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cdf5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5cdf5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5cdf5-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cdf5-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5cdf5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5cdf5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cdf5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5cdf5-116">Not supported.</span></span>|
|<span data-ttu-id="5cdf5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5cdf5-117">Application</span></span>|<span data-ttu-id="5cdf5-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cdf5-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cdf5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5cdf5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="5cdf5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5cdf5-120">Request headers</span></span>
|<span data-ttu-id="5cdf5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5cdf5-121">Header</span></span>|<span data-ttu-id="5cdf5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5cdf5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cdf5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5cdf5-123">Authorization</span></span>|<span data-ttu-id="5cdf5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5cdf5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cdf5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5cdf5-125">Accept</span></span>|<span data-ttu-id="5cdf5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5cdf5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cdf5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5cdf5-127">Request body</span></span>
<span data-ttu-id="5cdf5-128">No corpo da solicitação, forneça uma representação JSON do objeto microsoftStoreForBusinessContainedApp.</span><span class="sxs-lookup"><span data-stu-id="5cdf5-128">In the request body, supply a JSON representation for the microsoftStoreForBusinessContainedApp object.</span></span>

<span data-ttu-id="5cdf5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar microsoftStoreForBusinessContainedApp.</span><span class="sxs-lookup"><span data-stu-id="5cdf5-129">The following table shows the properties that are required when you create the microsoftStoreForBusinessContainedApp.</span></span>

|<span data-ttu-id="5cdf5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5cdf5-130">Property</span></span>|<span data-ttu-id="5cdf5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5cdf5-131">Type</span></span>|<span data-ttu-id="5cdf5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cdf5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cdf5-133">id</span><span class="sxs-lookup"><span data-stu-id="5cdf5-133">id</span></span>|<span data-ttu-id="5cdf5-134">String</span><span class="sxs-lookup"><span data-stu-id="5cdf5-134">String</span></span>|<span data-ttu-id="5cdf5-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5cdf5-135">Key of the entity.</span></span> <span data-ttu-id="5cdf5-136">Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="5cdf5-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="5cdf5-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="5cdf5-137">appUserModelId</span></span>|<span data-ttu-id="5cdf5-138">String</span><span class="sxs-lookup"><span data-stu-id="5cdf5-138">String</span></span>|<span data-ttu-id="5cdf5-139">A ID do modelo do usuário do aplicativo do aplicativo contido de um MicrosoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="5cdf5-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="5cdf5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cdf5-140">Response</span></span>
<span data-ttu-id="5cdf5-141">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5cdf5-141">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cdf5-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5cdf5-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="5cdf5-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5cdf5-143">Request</span></span>
<span data-ttu-id="5cdf5-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5cdf5-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="5cdf5-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cdf5-145">Response</span></span>
<span data-ttu-id="5cdf5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5cdf5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 176

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "id": "bf1d79df-79df-bf1d-df79-1dbfdf791dbf",
  "appUserModelId": "App User Model Id value"
}
```



