---
title: Atualizar microsoftStoreForBusinessContainedApp
description: Atualiza as propriedades de um objeto microsoftStoreForBusinessContainedApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca72c76c5f533f5194d4d8e0b0718e3f106c109f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34974283"
---
# <a name="update-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="adfeb-103">Atualizar microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="adfeb-103">Update microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="adfeb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="adfeb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="adfeb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="adfeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adfeb-106">Atualiza as propriedades de um objeto [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="adfeb-106">Update the properties of a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="adfeb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="adfeb-107">Prerequisites</span></span>
<span data-ttu-id="adfeb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adfeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adfeb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="adfeb-110">Permission type</span></span>|<span data-ttu-id="adfeb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="adfeb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adfeb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="adfeb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="adfeb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adfeb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="adfeb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="adfeb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adfeb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="adfeb-115">Not supported.</span></span>|
|<span data-ttu-id="adfeb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="adfeb-116">Application</span></span>|<span data-ttu-id="adfeb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="adfeb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="adfeb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="adfeb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="adfeb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="adfeb-119">Request headers</span></span>
|<span data-ttu-id="adfeb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="adfeb-120">Header</span></span>|<span data-ttu-id="adfeb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="adfeb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adfeb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="adfeb-122">Authorization</span></span>|<span data-ttu-id="adfeb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="adfeb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adfeb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="adfeb-124">Accept</span></span>|<span data-ttu-id="adfeb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="adfeb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adfeb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="adfeb-126">Request body</span></span>
<span data-ttu-id="adfeb-127">No corpo da solicitação, forneça uma representação JSON do objeto [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="adfeb-127">In the request body, supply a JSON representation for the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

<span data-ttu-id="adfeb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="adfeb-128">The following table shows the properties that are required when you create the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span></span>

|<span data-ttu-id="adfeb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="adfeb-129">Property</span></span>|<span data-ttu-id="adfeb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="adfeb-130">Type</span></span>|<span data-ttu-id="adfeb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="adfeb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adfeb-132">id</span><span class="sxs-lookup"><span data-stu-id="adfeb-132">id</span></span>|<span data-ttu-id="adfeb-133">String</span><span class="sxs-lookup"><span data-stu-id="adfeb-133">String</span></span>|<span data-ttu-id="adfeb-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="adfeb-134">Key of the entity.</span></span> <span data-ttu-id="adfeb-135">Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="adfeb-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="adfeb-136">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="adfeb-136">appUserModelId</span></span>|<span data-ttu-id="adfeb-137">String</span><span class="sxs-lookup"><span data-stu-id="adfeb-137">String</span></span>|<span data-ttu-id="adfeb-138">A ID do modelo do usuário do aplicativo do aplicativo contido de um MicrosoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="adfeb-138">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="adfeb-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="adfeb-139">Response</span></span>
<span data-ttu-id="adfeb-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="adfeb-140">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adfeb-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="adfeb-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="adfeb-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="adfeb-142">Request</span></span>
<span data-ttu-id="adfeb-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="adfeb-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="adfeb-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="adfeb-144">Response</span></span>
<span data-ttu-id="adfeb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="adfeb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





