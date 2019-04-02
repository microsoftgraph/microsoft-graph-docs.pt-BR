---
title: Atualizar windowsUniversalAppXContainedApp
description: Atualiza as propriedades de um objeto windowsUniversalAppXContainedApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4eeae30dd48689b2df656a5ea78139af01970c1b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959156"
---
# <a name="update-windowsuniversalappxcontainedapp"></a><span data-ttu-id="a2fbd-103">Atualizar windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="a2fbd-103">Update windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="a2fbd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a2fbd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2fbd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a2fbd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2fbd-106">Atualiza as propriedades de um objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="a2fbd-106">Update the properties of a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2fbd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a2fbd-107">Prerequisites</span></span>
<span data-ttu-id="a2fbd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2fbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2fbd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2fbd-110">Permission type</span></span>|<span data-ttu-id="a2fbd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a2fbd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2fbd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2fbd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2fbd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2fbd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a2fbd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2fbd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2fbd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2fbd-115">Not supported.</span></span>|
|<span data-ttu-id="a2fbd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2fbd-116">Application</span></span>|<span data-ttu-id="a2fbd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2fbd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2fbd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2fbd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="a2fbd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2fbd-119">Request headers</span></span>
|<span data-ttu-id="a2fbd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a2fbd-120">Header</span></span>|<span data-ttu-id="a2fbd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a2fbd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2fbd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2fbd-122">Authorization</span></span>|<span data-ttu-id="a2fbd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2fbd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2fbd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a2fbd-124">Accept</span></span>|<span data-ttu-id="a2fbd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a2fbd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2fbd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2fbd-126">Request body</span></span>
<span data-ttu-id="a2fbd-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="a2fbd-127">In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

<span data-ttu-id="a2fbd-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2fbd-128">The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

|<span data-ttu-id="a2fbd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2fbd-129">Property</span></span>|<span data-ttu-id="a2fbd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2fbd-130">Type</span></span>|<span data-ttu-id="a2fbd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2fbd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2fbd-132">id</span><span class="sxs-lookup"><span data-stu-id="a2fbd-132">id</span></span>|<span data-ttu-id="a2fbd-133">String</span><span class="sxs-lookup"><span data-stu-id="a2fbd-133">String</span></span>|<span data-ttu-id="a2fbd-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a2fbd-134">Key of the entity.</span></span> <span data-ttu-id="a2fbd-135">Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="a2fbd-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="a2fbd-136">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="a2fbd-136">appUserModelId</span></span>|<span data-ttu-id="a2fbd-137">String</span><span class="sxs-lookup"><span data-stu-id="a2fbd-137">String</span></span>|<span data-ttu-id="a2fbd-138">A ID do modelo do usuário do aplicativo do aplicativo contido de um aplicativo do WindowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="a2fbd-138">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="a2fbd-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2fbd-139">Response</span></span>
<span data-ttu-id="a2fbd-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2fbd-140">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2fbd-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2fbd-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2fbd-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2fbd-142">Request</span></span>
<span data-ttu-id="a2fbd-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2fbd-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="a2fbd-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2fbd-144">Response</span></span>
<span data-ttu-id="a2fbd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2fbd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 171

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
  "appUserModelId": "App User Model Id value"
}
```




