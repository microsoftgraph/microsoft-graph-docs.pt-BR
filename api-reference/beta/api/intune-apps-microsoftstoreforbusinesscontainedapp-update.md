---
title: Atualizar microsoftStoreForBusinessContainedApp
description: Atualize as propriedades de um objeto microsoftStoreForBusinessContainedApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a1154555af19db7d56778d454cdc07ce647f324
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417193"
---
# <a name="update-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="07c07-103">Atualizar microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="07c07-103">Update microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="07c07-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="07c07-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="07c07-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="07c07-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07c07-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="07c07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07c07-107">Atualize as propriedades de um objeto [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="07c07-107">Update the properties of a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07c07-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="07c07-108">Prerequisites</span></span>
<span data-ttu-id="07c07-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="07c07-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="07c07-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07c07-111">Permission type</span></span>|<span data-ttu-id="07c07-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="07c07-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07c07-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07c07-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07c07-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07c07-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="07c07-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07c07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07c07-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07c07-116">Not supported.</span></span>|
|<span data-ttu-id="07c07-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07c07-117">Application</span></span>|<span data-ttu-id="07c07-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07c07-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07c07-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07c07-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="07c07-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07c07-120">Request headers</span></span>
|<span data-ttu-id="07c07-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07c07-121">Header</span></span>|<span data-ttu-id="07c07-122">Valor</span><span class="sxs-lookup"><span data-stu-id="07c07-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07c07-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="07c07-123">Authorization</span></span>|<span data-ttu-id="07c07-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07c07-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07c07-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="07c07-125">Accept</span></span>|<span data-ttu-id="07c07-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07c07-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07c07-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07c07-127">Request body</span></span>
<span data-ttu-id="07c07-128">No corpo da solicitação, fornece uma representação JSON para o objeto [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="07c07-128">In the request body, supply a JSON representation for the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

<span data-ttu-id="07c07-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="07c07-129">The following table shows the properties that are required when you create the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span></span>

|<span data-ttu-id="07c07-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07c07-130">Property</span></span>|<span data-ttu-id="07c07-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="07c07-131">Type</span></span>|<span data-ttu-id="07c07-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="07c07-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07c07-133">id</span><span class="sxs-lookup"><span data-stu-id="07c07-133">id</span></span>|<span data-ttu-id="07c07-134">String</span><span class="sxs-lookup"><span data-stu-id="07c07-134">String</span></span>|<span data-ttu-id="07c07-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="07c07-135">Key of the entity.</span></span> <span data-ttu-id="07c07-136">Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="07c07-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="07c07-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="07c07-137">appUserModelId</span></span>|<span data-ttu-id="07c07-138">String</span><span class="sxs-lookup"><span data-stu-id="07c07-138">String</span></span>|<span data-ttu-id="07c07-139">A ID de modelo de usuário do aplicativo do aplicativo de um MicrosoftStoreForBusinessApp contido.</span><span class="sxs-lookup"><span data-stu-id="07c07-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="07c07-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="07c07-140">Response</span></span>
<span data-ttu-id="07c07-141">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07c07-141">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07c07-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07c07-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="07c07-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07c07-143">Request</span></span>
<span data-ttu-id="07c07-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07c07-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="07c07-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="07c07-145">Response</span></span>
<span data-ttu-id="07c07-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07c07-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




