---
title: Criar microsoftStoreForBusinessContainedApp
description: Criar um novo objeto microsoftStoreForBusinessContainedApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a358f8b9984b58502edb2c4e42297475530b241d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34974374"
---
# <a name="create-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="dd1a8-103">Criar microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="dd1a8-103">Create microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="dd1a8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dd1a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd1a8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dd1a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd1a8-106">Criar um novo objeto [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="dd1a8-106">Create a new [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd1a8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dd1a8-107">Prerequisites</span></span>
<span data-ttu-id="dd1a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd1a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd1a8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd1a8-110">Permission type</span></span>|<span data-ttu-id="dd1a8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dd1a8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd1a8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd1a8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dd1a8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd1a8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dd1a8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd1a8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd1a8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd1a8-115">Not supported.</span></span>|
|<span data-ttu-id="dd1a8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd1a8-116">Application</span></span>|<span data-ttu-id="dd1a8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd1a8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd1a8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd1a8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="dd1a8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd1a8-119">Request headers</span></span>
|<span data-ttu-id="dd1a8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dd1a8-120">Header</span></span>|<span data-ttu-id="dd1a8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dd1a8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd1a8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd1a8-122">Authorization</span></span>|<span data-ttu-id="dd1a8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd1a8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd1a8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dd1a8-124">Accept</span></span>|<span data-ttu-id="dd1a8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dd1a8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd1a8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd1a8-126">Request body</span></span>
<span data-ttu-id="dd1a8-127">No corpo da solicitação, forneça uma representação JSON do objeto microsoftStoreForBusinessContainedApp.</span><span class="sxs-lookup"><span data-stu-id="dd1a8-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessContainedApp object.</span></span>

<span data-ttu-id="dd1a8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar microsoftStoreForBusinessContainedApp.</span><span class="sxs-lookup"><span data-stu-id="dd1a8-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessContainedApp.</span></span>

|<span data-ttu-id="dd1a8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd1a8-129">Property</span></span>|<span data-ttu-id="dd1a8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd1a8-130">Type</span></span>|<span data-ttu-id="dd1a8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd1a8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd1a8-132">id</span><span class="sxs-lookup"><span data-stu-id="dd1a8-132">id</span></span>|<span data-ttu-id="dd1a8-133">String</span><span class="sxs-lookup"><span data-stu-id="dd1a8-133">String</span></span>|<span data-ttu-id="dd1a8-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dd1a8-134">Key of the entity.</span></span> <span data-ttu-id="dd1a8-135">Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="dd1a8-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="dd1a8-136">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="dd1a8-136">appUserModelId</span></span>|<span data-ttu-id="dd1a8-137">String</span><span class="sxs-lookup"><span data-stu-id="dd1a8-137">String</span></span>|<span data-ttu-id="dd1a8-138">A ID do modelo do usuário do aplicativo do aplicativo contido de um MicrosoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="dd1a8-138">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="dd1a8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd1a8-139">Response</span></span>
<span data-ttu-id="dd1a8-140">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd1a8-140">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd1a8-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd1a8-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd1a8-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd1a8-142">Request</span></span>
<span data-ttu-id="dd1a8-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd1a8-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="dd1a8-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd1a8-144">Response</span></span>
<span data-ttu-id="dd1a8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd1a8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





