---
title: Atualizar microsoftStoreForBusinessContainedApp
description: Atualiza as propriedades de um objeto microsoftStoreForBusinessContainedApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6e0a6aac641687e343cd0c3e41fdbfd3b40acd6a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935388"
---
# <a name="update-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="05732-103">Atualizar microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="05732-103">Update microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="05732-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="05732-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05732-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="05732-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05732-106">Atualiza as propriedades de um objeto [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="05732-106">Update the properties of a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05732-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="05732-107">Prerequisites</span></span>
<span data-ttu-id="05732-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05732-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05732-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05732-110">Permission type</span></span>|<span data-ttu-id="05732-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="05732-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05732-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05732-112">Delegated (work or school account)</span></span>|<span data-ttu-id="05732-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05732-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="05732-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05732-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05732-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05732-115">Not supported.</span></span>|
|<span data-ttu-id="05732-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05732-116">Application</span></span>|<span data-ttu-id="05732-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05732-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05732-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05732-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="05732-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05732-119">Request headers</span></span>
|<span data-ttu-id="05732-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05732-120">Header</span></span>|<span data-ttu-id="05732-121">Valor</span><span class="sxs-lookup"><span data-stu-id="05732-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05732-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="05732-122">Authorization</span></span>|<span data-ttu-id="05732-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05732-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05732-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="05732-124">Accept</span></span>|<span data-ttu-id="05732-125">application/json</span><span class="sxs-lookup"><span data-stu-id="05732-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05732-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05732-126">Request body</span></span>
<span data-ttu-id="05732-127">No corpo da solicitação, forneça uma representação JSON do objeto [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="05732-127">In the request body, supply a JSON representation for the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

<span data-ttu-id="05732-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="05732-128">The following table shows the properties that are required when you create the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span></span>

|<span data-ttu-id="05732-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05732-129">Property</span></span>|<span data-ttu-id="05732-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="05732-130">Type</span></span>|<span data-ttu-id="05732-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="05732-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05732-132">id</span><span class="sxs-lookup"><span data-stu-id="05732-132">id</span></span>|<span data-ttu-id="05732-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05732-133">String</span></span>|<span data-ttu-id="05732-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="05732-134">Key of the entity.</span></span> <span data-ttu-id="05732-135">Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="05732-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="05732-136">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="05732-136">appUserModelId</span></span>|<span data-ttu-id="05732-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05732-137">String</span></span>|<span data-ttu-id="05732-138">A ID do modelo do usuário do aplicativo do aplicativo contido de um MicrosoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="05732-138">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="05732-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="05732-139">Response</span></span>
<span data-ttu-id="05732-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05732-140">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05732-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05732-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="05732-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05732-142">Request</span></span>
<span data-ttu-id="05732-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05732-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="05732-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="05732-144">Response</span></span>
<span data-ttu-id="05732-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05732-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 176

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "id": "bf1d79df-79df-bf1d-df79-1dbfdf791dbf",
  "appUserModelId": "App User Model Id value"
}
```




