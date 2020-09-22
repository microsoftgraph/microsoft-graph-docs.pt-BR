---
title: Criar windowsUniversalAppXContainedApp
description: Criar um novo objeto windowsUniversalAppXContainedApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 751808f3a63bfca7fd9ab56e39752f0631f98c71
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47976015"
---
# <a name="create-windowsuniversalappxcontainedapp"></a><span data-ttu-id="f272b-103">Criar windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="f272b-103">Create windowsUniversalAppXContainedApp</span></span>

<span data-ttu-id="f272b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f272b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f272b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f272b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f272b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f272b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f272b-107">Criar um novo objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f272b-107">Create a new [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f272b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f272b-108">Prerequisites</span></span>
<span data-ttu-id="f272b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f272b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f272b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f272b-111">Permission type</span></span>|<span data-ttu-id="f272b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f272b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f272b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f272b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f272b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f272b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f272b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f272b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f272b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f272b-116">Not supported.</span></span>|
|<span data-ttu-id="f272b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f272b-117">Application</span></span>|<span data-ttu-id="f272b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f272b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f272b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f272b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="f272b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f272b-120">Request headers</span></span>
|<span data-ttu-id="f272b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f272b-121">Header</span></span>|<span data-ttu-id="f272b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f272b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f272b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f272b-123">Authorization</span></span>|<span data-ttu-id="f272b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f272b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f272b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f272b-125">Accept</span></span>|<span data-ttu-id="f272b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f272b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f272b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f272b-127">Request body</span></span>
<span data-ttu-id="f272b-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsUniversalAppXContainedApp.</span><span class="sxs-lookup"><span data-stu-id="f272b-128">In the request body, supply a JSON representation for the windowsUniversalAppXContainedApp object.</span></span>

<span data-ttu-id="f272b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsUniversalAppXContainedApp.</span><span class="sxs-lookup"><span data-stu-id="f272b-129">The following table shows the properties that are required when you create the windowsUniversalAppXContainedApp.</span></span>

|<span data-ttu-id="f272b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f272b-130">Property</span></span>|<span data-ttu-id="f272b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f272b-131">Type</span></span>|<span data-ttu-id="f272b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f272b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f272b-133">id</span><span class="sxs-lookup"><span data-stu-id="f272b-133">id</span></span>|<span data-ttu-id="f272b-134">String</span><span class="sxs-lookup"><span data-stu-id="f272b-134">String</span></span>|<span data-ttu-id="f272b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f272b-135">Key of the entity.</span></span> <span data-ttu-id="f272b-136">Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="f272b-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="f272b-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="f272b-137">appUserModelId</span></span>|<span data-ttu-id="f272b-138">String</span><span class="sxs-lookup"><span data-stu-id="f272b-138">String</span></span>|<span data-ttu-id="f272b-139">A ID do modelo do usuário do aplicativo do aplicativo contido de um aplicativo do WindowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="f272b-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="f272b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f272b-140">Response</span></span>
<span data-ttu-id="f272b-141">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f272b-141">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f272b-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f272b-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="f272b-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f272b-143">Request</span></span>
<span data-ttu-id="f272b-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f272b-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="f272b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f272b-145">Response</span></span>
<span data-ttu-id="f272b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f272b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






