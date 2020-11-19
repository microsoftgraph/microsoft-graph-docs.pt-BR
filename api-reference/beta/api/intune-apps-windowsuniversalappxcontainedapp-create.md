---
title: Criar windowsUniversalAppXContainedApp
description: Criar um novo objeto windowsUniversalAppXContainedApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3cf163d05e084d17b5f46df6f78d731db9561c2b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49245932"
---
# <a name="create-windowsuniversalappxcontainedapp"></a><span data-ttu-id="1c3c8-103">Criar windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="1c3c8-103">Create windowsUniversalAppXContainedApp</span></span>

<span data-ttu-id="1c3c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c3c8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c3c8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1c3c8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c3c8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1c3c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c3c8-107">Criar um novo objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="1c3c8-107">Create a new [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c3c8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1c3c8-108">Prerequisites</span></span>
<span data-ttu-id="1c3c8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c3c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c3c8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c3c8-111">Permission type</span></span>|<span data-ttu-id="1c3c8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1c3c8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c3c8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c3c8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c3c8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c3c8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1c3c8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c3c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c3c8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c3c8-116">Not supported.</span></span>|
|<span data-ttu-id="1c3c8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c3c8-117">Application</span></span>|<span data-ttu-id="1c3c8-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c3c8-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c3c8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c3c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="1c3c8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c3c8-120">Request headers</span></span>
|<span data-ttu-id="1c3c8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c3c8-121">Header</span></span>|<span data-ttu-id="1c3c8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1c3c8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c3c8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c3c8-123">Authorization</span></span>|<span data-ttu-id="1c3c8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c3c8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c3c8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1c3c8-125">Accept</span></span>|<span data-ttu-id="1c3c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1c3c8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c3c8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c3c8-127">Request body</span></span>
<span data-ttu-id="1c3c8-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsUniversalAppXContainedApp.</span><span class="sxs-lookup"><span data-stu-id="1c3c8-128">In the request body, supply a JSON representation for the windowsUniversalAppXContainedApp object.</span></span>

<span data-ttu-id="1c3c8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsUniversalAppXContainedApp.</span><span class="sxs-lookup"><span data-stu-id="1c3c8-129">The following table shows the properties that are required when you create the windowsUniversalAppXContainedApp.</span></span>

|<span data-ttu-id="1c3c8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c3c8-130">Property</span></span>|<span data-ttu-id="1c3c8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c3c8-131">Type</span></span>|<span data-ttu-id="1c3c8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c3c8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c3c8-133">id</span><span class="sxs-lookup"><span data-stu-id="1c3c8-133">id</span></span>|<span data-ttu-id="1c3c8-134">String</span><span class="sxs-lookup"><span data-stu-id="1c3c8-134">String</span></span>|<span data-ttu-id="1c3c8-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1c3c8-135">Key of the entity.</span></span> <span data-ttu-id="1c3c8-136">Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="1c3c8-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="1c3c8-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="1c3c8-137">appUserModelId</span></span>|<span data-ttu-id="1c3c8-138">String</span><span class="sxs-lookup"><span data-stu-id="1c3c8-138">String</span></span>|<span data-ttu-id="1c3c8-139">A ID do modelo do usuário do aplicativo do aplicativo contido de um aplicativo do WindowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="1c3c8-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="1c3c8-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c3c8-140">Response</span></span>
<span data-ttu-id="1c3c8-141">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c3c8-141">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c3c8-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c3c8-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c3c8-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c3c8-143">Request</span></span>
<span data-ttu-id="1c3c8-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c3c8-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="1c3c8-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c3c8-145">Response</span></span>
<span data-ttu-id="1c3c8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c3c8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 171

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
  "appUserModelId": "App User Model Id value"
}
```




