---
title: Criar windowsUniversalAppXContainedApp
description: Criar um novo objeto windowsUniversalAppXContainedApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ccfbcbf87fad0e8c793d394767f2bc7139e3dc8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983264"
---
# <a name="create-windowsuniversalappxcontainedapp"></a><span data-ttu-id="fe644-103">Criar windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="fe644-103">Create windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="fe644-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fe644-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe644-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fe644-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe644-106">Criar um novo objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="fe644-106">Create a new [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe644-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fe644-107">Prerequisites</span></span>
<span data-ttu-id="fe644-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe644-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe644-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe644-110">Permission type</span></span>|<span data-ttu-id="fe644-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fe644-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe644-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe644-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fe644-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe644-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fe644-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe644-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe644-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe644-115">Not supported.</span></span>|
|<span data-ttu-id="fe644-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe644-116">Application</span></span>|<span data-ttu-id="fe644-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe644-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe644-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe644-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="fe644-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe644-119">Request headers</span></span>
|<span data-ttu-id="fe644-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe644-120">Header</span></span>|<span data-ttu-id="fe644-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fe644-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe644-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe644-122">Authorization</span></span>|<span data-ttu-id="fe644-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe644-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe644-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fe644-124">Accept</span></span>|<span data-ttu-id="fe644-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fe644-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe644-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe644-126">Request body</span></span>
<span data-ttu-id="fe644-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsUniversalAppXContainedApp.</span><span class="sxs-lookup"><span data-stu-id="fe644-127">In the request body, supply a JSON representation for the windowsUniversalAppXContainedApp object.</span></span>

<span data-ttu-id="fe644-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsUniversalAppXContainedApp.</span><span class="sxs-lookup"><span data-stu-id="fe644-128">The following table shows the properties that are required when you create the windowsUniversalAppXContainedApp.</span></span>

|<span data-ttu-id="fe644-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe644-129">Property</span></span>|<span data-ttu-id="fe644-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe644-130">Type</span></span>|<span data-ttu-id="fe644-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe644-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe644-132">id</span><span class="sxs-lookup"><span data-stu-id="fe644-132">id</span></span>|<span data-ttu-id="fe644-133">String</span><span class="sxs-lookup"><span data-stu-id="fe644-133">String</span></span>|<span data-ttu-id="fe644-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fe644-134">Key of the entity.</span></span> <span data-ttu-id="fe644-135">Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe644-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="fe644-136">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="fe644-136">appUserModelId</span></span>|<span data-ttu-id="fe644-137">String</span><span class="sxs-lookup"><span data-stu-id="fe644-137">String</span></span>|<span data-ttu-id="fe644-138">A ID do modelo do usuário do aplicativo do aplicativo contido de um aplicativo do WindowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="fe644-138">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="fe644-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe644-139">Response</span></span>
<span data-ttu-id="fe644-140">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe644-140">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe644-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe644-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe644-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe644-142">Request</span></span>
<span data-ttu-id="fe644-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe644-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="fe644-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe644-144">Response</span></span>
<span data-ttu-id="fe644-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe644-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




