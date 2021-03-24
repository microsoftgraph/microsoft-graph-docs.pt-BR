---
title: Atualizar microsoftStoreForBusinessContainedApp
description: Atualize as propriedades de um objeto microsoftStoreForBusinessContainedApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9062bb741bdb6c065129ab3b681cb4faed92e8e1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139920"
---
# <a name="update-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="c6773-103">Atualizar microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="c6773-103">Update microsoftStoreForBusinessContainedApp</span></span>

<span data-ttu-id="c6773-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6773-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6773-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c6773-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6773-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c6773-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6773-107">Atualize as propriedades de um [objeto microsoftStoreForBusinessContainedApp.](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6773-107">Update the properties of a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6773-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c6773-108">Prerequisites</span></span>
<span data-ttu-id="c6773-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6773-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6773-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6773-111">Permission type</span></span>|<span data-ttu-id="c6773-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6773-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6773-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6773-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c6773-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6773-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c6773-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6773-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6773-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6773-116">Not supported.</span></span>|
|<span data-ttu-id="c6773-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6773-117">Application</span></span>|<span data-ttu-id="c6773-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6773-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6773-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6773-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="c6773-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6773-120">Request headers</span></span>
|<span data-ttu-id="c6773-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c6773-121">Header</span></span>|<span data-ttu-id="c6773-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c6773-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6773-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6773-123">Authorization</span></span>|<span data-ttu-id="c6773-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6773-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6773-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c6773-125">Accept</span></span>|<span data-ttu-id="c6773-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c6773-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6773-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6773-127">Request body</span></span>
<span data-ttu-id="c6773-128">No corpo da solicitação, fornece uma representação JSON para o [objeto microsoftStoreForBusinessContainedApp.](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6773-128">In the request body, supply a JSON representation for the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

<span data-ttu-id="c6773-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6773-129">The following table shows the properties that are required when you create the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span></span>

|<span data-ttu-id="c6773-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6773-130">Property</span></span>|<span data-ttu-id="c6773-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6773-131">Type</span></span>|<span data-ttu-id="c6773-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6773-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6773-133">id</span><span class="sxs-lookup"><span data-stu-id="c6773-133">id</span></span>|<span data-ttu-id="c6773-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6773-134">String</span></span>|<span data-ttu-id="c6773-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c6773-135">Key of the entity.</span></span> <span data-ttu-id="c6773-136">Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6773-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="c6773-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="c6773-137">appUserModelId</span></span>|<span data-ttu-id="c6773-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6773-138">String</span></span>|<span data-ttu-id="c6773-139">A ID do modelo de usuário do aplicativo contido de um MicrosoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="c6773-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="c6773-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6773-140">Response</span></span>
<span data-ttu-id="c6773-141">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6773-141">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6773-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6773-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6773-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6773-143">Request</span></span>
<span data-ttu-id="c6773-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6773-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="c6773-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6773-145">Response</span></span>
<span data-ttu-id="c6773-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6773-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




