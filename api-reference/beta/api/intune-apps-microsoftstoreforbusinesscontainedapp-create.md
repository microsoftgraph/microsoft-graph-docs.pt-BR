---
title: Criar microsoftStoreForBusinessContainedApp
description: Criar um novo objeto microsoftStoreForBusinessContainedApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c49fad0821f4eb14041be292997e3e5a94bc485
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761458"
---
# <a name="create-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="6768e-103">Criar microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="6768e-103">Create microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="6768e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6768e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6768e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6768e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6768e-106">Criar um novo objeto [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="6768e-106">Create a new [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6768e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6768e-107">Prerequisites</span></span>
<span data-ttu-id="6768e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6768e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6768e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6768e-110">Permission type</span></span>|<span data-ttu-id="6768e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6768e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6768e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6768e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6768e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6768e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6768e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6768e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6768e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6768e-115">Not supported.</span></span>|
|<span data-ttu-id="6768e-116">Application</span><span class="sxs-lookup"><span data-stu-id="6768e-116">Application</span></span>|<span data-ttu-id="6768e-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6768e-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6768e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6768e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="6768e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6768e-119">Request headers</span></span>
|<span data-ttu-id="6768e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6768e-120">Header</span></span>|<span data-ttu-id="6768e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6768e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6768e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6768e-122">Authorization</span></span>|<span data-ttu-id="6768e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6768e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6768e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6768e-124">Accept</span></span>|<span data-ttu-id="6768e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6768e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6768e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6768e-126">Request body</span></span>
<span data-ttu-id="6768e-127">No corpo da solicitação, forneça uma representação JSON do objeto microsoftStoreForBusinessContainedApp.</span><span class="sxs-lookup"><span data-stu-id="6768e-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessContainedApp object.</span></span>

<span data-ttu-id="6768e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar microsoftStoreForBusinessContainedApp.</span><span class="sxs-lookup"><span data-stu-id="6768e-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessContainedApp.</span></span>

|<span data-ttu-id="6768e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6768e-129">Property</span></span>|<span data-ttu-id="6768e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6768e-130">Type</span></span>|<span data-ttu-id="6768e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6768e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6768e-132">id</span><span class="sxs-lookup"><span data-stu-id="6768e-132">id</span></span>|<span data-ttu-id="6768e-133">String</span><span class="sxs-lookup"><span data-stu-id="6768e-133">String</span></span>|<span data-ttu-id="6768e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6768e-134">Key of the entity.</span></span> <span data-ttu-id="6768e-135">Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="6768e-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="6768e-136">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="6768e-136">appUserModelId</span></span>|<span data-ttu-id="6768e-137">String</span><span class="sxs-lookup"><span data-stu-id="6768e-137">String</span></span>|<span data-ttu-id="6768e-138">A ID do modelo do usuário do aplicativo do aplicativo contido de um MicrosoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="6768e-138">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="6768e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6768e-139">Response</span></span>
<span data-ttu-id="6768e-140">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6768e-140">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6768e-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6768e-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="6768e-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6768e-142">Request</span></span>
<span data-ttu-id="6768e-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6768e-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="6768e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6768e-144">Response</span></span>
<span data-ttu-id="6768e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6768e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




