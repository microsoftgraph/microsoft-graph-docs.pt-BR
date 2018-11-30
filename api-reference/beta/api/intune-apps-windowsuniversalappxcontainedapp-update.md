---
title: Atualizar windowsUniversalAppXContainedApp
description: Atualize as propriedades de um objeto windowsUniversalAppXContainedApp.
ms.openlocfilehash: 54ce98544de57e5f5ec296c73e8daed746969b76
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040965"
---
# <a name="update-windowsuniversalappxcontainedapp"></a><span data-ttu-id="f877f-103">Atualizar windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="f877f-103">Update windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="f877f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f877f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f877f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f877f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f877f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f877f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f877f-107">Atualize as propriedades de um objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f877f-107">Update the properties of a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f877f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f877f-108">Prerequisites</span></span>
<span data-ttu-id="f877f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f877f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f877f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f877f-111">Permission type</span></span>|<span data-ttu-id="f877f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f877f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f877f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f877f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f877f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f877f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f877f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f877f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f877f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f877f-116">Not supported.</span></span>|
|<span data-ttu-id="f877f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f877f-117">Application</span></span>|<span data-ttu-id="f877f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f877f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f877f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f877f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="f877f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f877f-120">Request headers</span></span>
|<span data-ttu-id="f877f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f877f-121">Header</span></span>|<span data-ttu-id="f877f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f877f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f877f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f877f-123">Authorization</span></span>|<span data-ttu-id="f877f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f877f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f877f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f877f-125">Accept</span></span>|<span data-ttu-id="f877f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f877f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f877f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f877f-127">Request body</span></span>
<span data-ttu-id="f877f-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f877f-128">In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

<span data-ttu-id="f877f-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="f877f-129">The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

|<span data-ttu-id="f877f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f877f-130">Property</span></span>|<span data-ttu-id="f877f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f877f-131">Type</span></span>|<span data-ttu-id="f877f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f877f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f877f-133">id</span><span class="sxs-lookup"><span data-stu-id="f877f-133">id</span></span>|<span data-ttu-id="f877f-134">String</span><span class="sxs-lookup"><span data-stu-id="f877f-134">String</span></span>|<span data-ttu-id="f877f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f877f-135">Key of the entity.</span></span> <span data-ttu-id="f877f-136">Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="f877f-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="f877f-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="f877f-137">appUserModelId</span></span>|<span data-ttu-id="f877f-138">String</span><span class="sxs-lookup"><span data-stu-id="f877f-138">String</span></span>|<span data-ttu-id="f877f-139">A ID de modelo de usuário do aplicativo do aplicativo de um aplicativo WindowsUniversalAppX contido.</span><span class="sxs-lookup"><span data-stu-id="f877f-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="f877f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f877f-140">Response</span></span>
<span data-ttu-id="f877f-141">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f877f-141">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f877f-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f877f-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="f877f-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f877f-143">Request</span></span>
<span data-ttu-id="f877f-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f877f-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 51

{
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="f877f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f877f-145">Response</span></span>
<span data-ttu-id="f877f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f877f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





