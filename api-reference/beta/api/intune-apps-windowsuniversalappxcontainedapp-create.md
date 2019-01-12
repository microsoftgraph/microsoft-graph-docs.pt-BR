---
title: Criar windowsUniversalAppXContainedApp
description: Crie um novo objeto de windowsUniversalAppXContainedApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f0466628ed1b2e6f3e0e196498b7cef3bb9daf24
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920979"
---
# <a name="create-windowsuniversalappxcontainedapp"></a><span data-ttu-id="7833d-103">Criar windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="7833d-103">Create windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="7833d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7833d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7833d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7833d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7833d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7833d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7833d-107">Crie um novo objeto de [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="7833d-107">Create a new [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7833d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7833d-108">Prerequisites</span></span>
<span data-ttu-id="7833d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7833d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7833d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7833d-111">Permission type</span></span>|<span data-ttu-id="7833d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7833d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7833d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7833d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7833d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7833d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7833d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7833d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7833d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7833d-116">Not supported.</span></span>|
|<span data-ttu-id="7833d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7833d-117">Application</span></span>|<span data-ttu-id="7833d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7833d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7833d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7833d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="7833d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7833d-120">Request headers</span></span>
|<span data-ttu-id="7833d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7833d-121">Header</span></span>|<span data-ttu-id="7833d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7833d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7833d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7833d-123">Authorization</span></span>|<span data-ttu-id="7833d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7833d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7833d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7833d-125">Accept</span></span>|<span data-ttu-id="7833d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7833d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7833d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7833d-127">Request body</span></span>
<span data-ttu-id="7833d-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsUniversalAppXContainedApp.</span><span class="sxs-lookup"><span data-stu-id="7833d-128">In the request body, supply a JSON representation for the windowsUniversalAppXContainedApp object.</span></span>

<span data-ttu-id="7833d-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsUniversalAppXContainedApp.</span><span class="sxs-lookup"><span data-stu-id="7833d-129">The following table shows the properties that are required when you create the windowsUniversalAppXContainedApp.</span></span>

|<span data-ttu-id="7833d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7833d-130">Property</span></span>|<span data-ttu-id="7833d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7833d-131">Type</span></span>|<span data-ttu-id="7833d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7833d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7833d-133">id</span><span class="sxs-lookup"><span data-stu-id="7833d-133">id</span></span>|<span data-ttu-id="7833d-134">String</span><span class="sxs-lookup"><span data-stu-id="7833d-134">String</span></span>|<span data-ttu-id="7833d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7833d-135">Key of the entity.</span></span> <span data-ttu-id="7833d-136">Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="7833d-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="7833d-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="7833d-137">appUserModelId</span></span>|<span data-ttu-id="7833d-138">String</span><span class="sxs-lookup"><span data-stu-id="7833d-138">String</span></span>|<span data-ttu-id="7833d-139">A ID de modelo de usuário do aplicativo do aplicativo de um aplicativo WindowsUniversalAppX contido.</span><span class="sxs-lookup"><span data-stu-id="7833d-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="7833d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7833d-140">Response</span></span>
<span data-ttu-id="7833d-141">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7833d-141">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7833d-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7833d-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="7833d-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7833d-143">Request</span></span>
<span data-ttu-id="7833d-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7833d-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="7833d-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="7833d-145">Response</span></span>
<span data-ttu-id="7833d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7833d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





