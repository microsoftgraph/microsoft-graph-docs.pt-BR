---
title: Atualizar windowsUniversalAppXContainedApp
description: Atualize as propriedades de um objeto windowsUniversalAppXContainedApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0b3be9aad8e45c1f91c7be5af8772ee5803c22fa
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133273"
---
# <a name="update-windowsuniversalappxcontainedapp"></a><span data-ttu-id="6b958-103">Atualizar windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="6b958-103">Update windowsUniversalAppXContainedApp</span></span>

<span data-ttu-id="6b958-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b958-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b958-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6b958-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b958-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b958-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b958-107">Atualize as propriedades de um [objeto windowsUniversalAppXContainedApp.](../resources/intune-apps-windowsuniversalappxcontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b958-107">Update the properties of a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b958-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6b958-108">Prerequisites</span></span>
<span data-ttu-id="6b958-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b958-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b958-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b958-111">Permission type</span></span>|<span data-ttu-id="6b958-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b958-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b958-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b958-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6b958-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b958-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6b958-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b958-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b958-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b958-116">Not supported.</span></span>|
|<span data-ttu-id="6b958-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b958-117">Application</span></span>|<span data-ttu-id="6b958-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b958-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b958-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b958-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="6b958-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b958-120">Request headers</span></span>
|<span data-ttu-id="6b958-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6b958-121">Header</span></span>|<span data-ttu-id="6b958-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6b958-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b958-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b958-123">Authorization</span></span>|<span data-ttu-id="6b958-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b958-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b958-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6b958-125">Accept</span></span>|<span data-ttu-id="6b958-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b958-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b958-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b958-127">Request body</span></span>
<span data-ttu-id="6b958-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsUniversalAppXContainedApp.](../resources/intune-apps-windowsuniversalappxcontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b958-128">In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

<span data-ttu-id="6b958-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="6b958-129">The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

|<span data-ttu-id="6b958-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b958-130">Property</span></span>|<span data-ttu-id="6b958-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b958-131">Type</span></span>|<span data-ttu-id="6b958-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b958-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b958-133">id</span><span class="sxs-lookup"><span data-stu-id="6b958-133">id</span></span>|<span data-ttu-id="6b958-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b958-134">String</span></span>|<span data-ttu-id="6b958-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6b958-135">Key of the entity.</span></span> <span data-ttu-id="6b958-136">Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b958-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="6b958-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="6b958-137">appUserModelId</span></span>|<span data-ttu-id="6b958-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b958-138">String</span></span>|<span data-ttu-id="6b958-139">A ID do modelo de usuário do aplicativo contido de um aplicativo WindowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="6b958-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="6b958-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b958-140">Response</span></span>
<span data-ttu-id="6b958-141">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b958-141">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b958-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b958-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b958-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b958-143">Request</span></span>
<span data-ttu-id="6b958-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b958-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="6b958-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b958-145">Response</span></span>
<span data-ttu-id="6b958-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b958-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




