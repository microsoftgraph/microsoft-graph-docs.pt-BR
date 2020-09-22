---
title: Atualizar microsoftStoreForBusinessContainedApp
description: Atualiza as propriedades de um objeto microsoftStoreForBusinessContainedApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 623558c9fc0ddad8bed32eec2d33116cb842b3f3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47977604"
---
# <a name="update-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="e0226-103">Atualizar microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="e0226-103">Update microsoftStoreForBusinessContainedApp</span></span>

<span data-ttu-id="e0226-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0226-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0226-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e0226-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0226-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e0226-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0226-107">Atualiza as propriedades de um objeto [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e0226-107">Update the properties of a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0226-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e0226-108">Prerequisites</span></span>
<span data-ttu-id="e0226-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0226-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0226-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0226-111">Permission type</span></span>|<span data-ttu-id="e0226-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e0226-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0226-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0226-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0226-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0226-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e0226-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0226-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0226-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0226-116">Not supported.</span></span>|
|<span data-ttu-id="e0226-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0226-117">Application</span></span>|<span data-ttu-id="e0226-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0226-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0226-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0226-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="e0226-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0226-120">Request headers</span></span>
|<span data-ttu-id="e0226-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e0226-121">Header</span></span>|<span data-ttu-id="e0226-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e0226-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0226-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0226-123">Authorization</span></span>|<span data-ttu-id="e0226-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0226-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0226-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e0226-125">Accept</span></span>|<span data-ttu-id="e0226-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0226-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0226-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0226-127">Request body</span></span>
<span data-ttu-id="e0226-128">No corpo da solicitação, forneça uma representação JSON do objeto [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e0226-128">In the request body, supply a JSON representation for the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

<span data-ttu-id="e0226-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0226-129">The following table shows the properties that are required when you create the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span></span>

|<span data-ttu-id="e0226-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0226-130">Property</span></span>|<span data-ttu-id="e0226-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0226-131">Type</span></span>|<span data-ttu-id="e0226-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0226-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0226-133">id</span><span class="sxs-lookup"><span data-stu-id="e0226-133">id</span></span>|<span data-ttu-id="e0226-134">String</span><span class="sxs-lookup"><span data-stu-id="e0226-134">String</span></span>|<span data-ttu-id="e0226-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e0226-135">Key of the entity.</span></span> <span data-ttu-id="e0226-136">Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0226-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="e0226-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="e0226-137">appUserModelId</span></span>|<span data-ttu-id="e0226-138">String</span><span class="sxs-lookup"><span data-stu-id="e0226-138">String</span></span>|<span data-ttu-id="e0226-139">A ID do modelo do usuário do aplicativo do aplicativo contido de um MicrosoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="e0226-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="e0226-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0226-140">Response</span></span>
<span data-ttu-id="e0226-141">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0226-141">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0226-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0226-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0226-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0226-143">Request</span></span>
<span data-ttu-id="e0226-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0226-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="e0226-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0226-145">Response</span></span>
<span data-ttu-id="e0226-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0226-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






