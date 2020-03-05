---
title: Atualizar windowsUniversalAppXContainedApp
description: Atualiza as propriedades de um objeto windowsUniversalAppXContainedApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5ef2640aef750a466408fee5f036f594f3c2f1b2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444634"
---
# <a name="update-windowsuniversalappxcontainedapp"></a><span data-ttu-id="01ebb-103">Atualizar windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="01ebb-103">Update windowsUniversalAppXContainedApp</span></span>

<span data-ttu-id="01ebb-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="01ebb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01ebb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="01ebb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01ebb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="01ebb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01ebb-107">Atualiza as propriedades de um objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="01ebb-107">Update the properties of a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01ebb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="01ebb-108">Prerequisites</span></span>
<span data-ttu-id="01ebb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01ebb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01ebb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01ebb-111">Permission type</span></span>|<span data-ttu-id="01ebb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="01ebb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01ebb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01ebb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01ebb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01ebb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="01ebb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01ebb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01ebb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01ebb-116">Not supported.</span></span>|
|<span data-ttu-id="01ebb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01ebb-117">Application</span></span>|<span data-ttu-id="01ebb-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01ebb-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01ebb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01ebb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="01ebb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01ebb-120">Request headers</span></span>
|<span data-ttu-id="01ebb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01ebb-121">Header</span></span>|<span data-ttu-id="01ebb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="01ebb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01ebb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="01ebb-123">Authorization</span></span>|<span data-ttu-id="01ebb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01ebb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01ebb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="01ebb-125">Accept</span></span>|<span data-ttu-id="01ebb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01ebb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01ebb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01ebb-127">Request body</span></span>
<span data-ttu-id="01ebb-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="01ebb-128">In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

<span data-ttu-id="01ebb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="01ebb-129">The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

|<span data-ttu-id="01ebb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01ebb-130">Property</span></span>|<span data-ttu-id="01ebb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="01ebb-131">Type</span></span>|<span data-ttu-id="01ebb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="01ebb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01ebb-133">id</span><span class="sxs-lookup"><span data-stu-id="01ebb-133">id</span></span>|<span data-ttu-id="01ebb-134">String</span><span class="sxs-lookup"><span data-stu-id="01ebb-134">String</span></span>|<span data-ttu-id="01ebb-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="01ebb-135">Key of the entity.</span></span> <span data-ttu-id="01ebb-136">Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="01ebb-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="01ebb-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="01ebb-137">appUserModelId</span></span>|<span data-ttu-id="01ebb-138">String</span><span class="sxs-lookup"><span data-stu-id="01ebb-138">String</span></span>|<span data-ttu-id="01ebb-139">A ID do modelo do usuário do aplicativo do aplicativo contido de um aplicativo do WindowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="01ebb-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="01ebb-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="01ebb-140">Response</span></span>
<span data-ttu-id="01ebb-141">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01ebb-141">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01ebb-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01ebb-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="01ebb-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01ebb-143">Request</span></span>
<span data-ttu-id="01ebb-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01ebb-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="01ebb-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="01ebb-145">Response</span></span>
<span data-ttu-id="01ebb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01ebb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





