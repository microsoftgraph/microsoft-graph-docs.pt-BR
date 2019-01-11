---
title: Criar microsoftStoreForBusinessContainedApp
description: Crie um novo objeto de microsoftStoreForBusinessContainedApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ac782261c00008bf9b4ab552932f8f841a9965bc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843292"
---
# <a name="create-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="afbb4-103">Criar microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="afbb4-103">Create microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="afbb4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="afbb4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="afbb4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="afbb4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="afbb4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="afbb4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="afbb4-107">Crie um novo objeto de [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="afbb4-107">Create a new [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="afbb4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="afbb4-108">Prerequisites</span></span>
<span data-ttu-id="afbb4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afbb4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afbb4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="afbb4-111">Permission type</span></span>|<span data-ttu-id="afbb4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="afbb4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afbb4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="afbb4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="afbb4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afbb4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="afbb4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="afbb4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afbb4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afbb4-116">Not supported.</span></span>|
|<span data-ttu-id="afbb4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="afbb4-117">Application</span></span>|<span data-ttu-id="afbb4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afbb4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="afbb4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="afbb4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="afbb4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="afbb4-120">Request headers</span></span>
|<span data-ttu-id="afbb4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="afbb4-121">Header</span></span>|<span data-ttu-id="afbb4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="afbb4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afbb4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="afbb4-123">Authorization</span></span>|<span data-ttu-id="afbb4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="afbb4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afbb4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="afbb4-125">Accept</span></span>|<span data-ttu-id="afbb4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="afbb4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afbb4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="afbb4-127">Request body</span></span>
<span data-ttu-id="afbb4-128">No corpo da solicitação, fornece uma representação JSON para o objeto microsoftStoreForBusinessContainedApp.</span><span class="sxs-lookup"><span data-stu-id="afbb4-128">In the request body, supply a JSON representation for the microsoftStoreForBusinessContainedApp object.</span></span>

<span data-ttu-id="afbb4-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o microsoftStoreForBusinessContainedApp.</span><span class="sxs-lookup"><span data-stu-id="afbb4-129">The following table shows the properties that are required when you create the microsoftStoreForBusinessContainedApp.</span></span>

|<span data-ttu-id="afbb4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="afbb4-130">Property</span></span>|<span data-ttu-id="afbb4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="afbb4-131">Type</span></span>|<span data-ttu-id="afbb4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="afbb4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afbb4-133">id</span><span class="sxs-lookup"><span data-stu-id="afbb4-133">id</span></span>|<span data-ttu-id="afbb4-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afbb4-134">String</span></span>|<span data-ttu-id="afbb4-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="afbb4-135">Key of the entity.</span></span> <span data-ttu-id="afbb4-136">Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="afbb4-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="afbb4-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="afbb4-137">appUserModelId</span></span>|<span data-ttu-id="afbb4-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afbb4-138">String</span></span>|<span data-ttu-id="afbb4-139">A ID de modelo de usuário do aplicativo do aplicativo de um MicrosoftStoreForBusinessApp contido.</span><span class="sxs-lookup"><span data-stu-id="afbb4-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="afbb4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="afbb4-140">Response</span></span>
<span data-ttu-id="afbb4-141">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="afbb4-141">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afbb4-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="afbb4-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="afbb4-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="afbb4-143">Request</span></span>
<span data-ttu-id="afbb4-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="afbb4-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="afbb4-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="afbb4-145">Response</span></span>
<span data-ttu-id="afbb4-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="afbb4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





